---
title: "Oracle JOB"
date: 2020-08-26 11:58:28 -0400
categories: update
---

# Oracle JOB
* job : job 번호로 다른 프로시저에서 호출될 수 있음
* what : 수행할 pl/sql or procedure or package 이름을 지정, 직접 수행하기를 원하는 sql문 적어도 됨
* next_date : 다음에 수행될 시간을 지정
* interval : 수행되는 주기를 지정, 초단위까지 지정가능
  * 10분 간격 : sysdate + 10/1440
  * 1시간 간격 : sysdate + 60/1440
  * 매일 오전 7시 : trunc(sysdate) + 1 + 7/24 ( 매일이므로 정해진 시간에 속함 )
* instance : 작업이 제출되어 졌을때, 어떤 instance 가 작업을 실행할지 지정합니다
* force : TRUE인 경우 모든 양의 정수는 작업 인스턴스로 허용됩니다. 이 값이 FALSE이면(FASE가 기본값 입니다.) 지정된 인스턴스가 실행되고 있어야 합니다. 그렇지 않으면 예외가 발생합니다.
