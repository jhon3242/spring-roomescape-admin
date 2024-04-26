# 기능 구현 목록
## step1
- [X] : localhost:8080/admin 요청 시 어드민 메인 페이지가 응답해야한다.

## step2
- [X] : /admin/reservation 요청 시 예약 관리 페이지가 응답해야한다.
- [X] : API 명세에 따라 예약 목록 조회 API 를 구현한다.

## step3
- [X] : 예약 추가 API 구현한다.
- [X] : 예약 취소 API 구현한다.

## step4
- [X] : 데이터베이스 설정 정보를 추가한다.
- [X] : DB에 연결해 테이블에 접근할 수 있다.

## step5
- [X] : 예약 추가 이후 데이터베이스 쿼리를 통해 추가된 예약을 확인할 수 있다.

## step6
- [X] : 데이터베이스를 활용하여 예약을 추가할 수 있다.
- [X] : 데이터베이스를 활용하여 데이터 삭제할 수 있다.

## step7
- [X] : 시간을 추가할 수 있다.
  - [X] : 응답으로 id, startAt 을 Body 에 담아서 반환한다.
  - [X] : DB 시간 테이블에 추가한다. 
- [X] : 시간을 조회할 수 있다.
- [X] : 시간을 삭제할 수 있다.
  - [X] : 응답으로 200 코드를 반환한다.

## step8
- [X] : 예약 기능에서 시간을 시간 테이블에 저장된 값만 선택할 수 있도록 수정한다.
- [X] : 변경된 API 명세 반영한다.
- [X] : 예약 페이지 파일을 변경한다. reservation-legacy.html -> reservation.html  
- [X] : 외래키 지정을 통해 reservation 테이블과 reservation_time 테이블의 관계를 설정한다.
- [X] : 예약 클래스 시간 타입을 String 에서 ReservationTime으로 변경한다.
- [X] : 예약 추가 시, 시간을 문자열(ex. "10:00") 형태로 입력하던 부분을 ReservationTime의 식별자(ex. 1)로 수정한다.
- [X] : 예약 조회 시, ReservationTime 정보도 함께 조회하도록 수정한다.

## step9
- [X] : ReservationsController 가 JdbcTemplate 를 모르도록 한다.

## step10
- [ ] : console view 를 구현한다.
- [ ] : console view 에 대응되는 컨트롤러를 구현한다. 