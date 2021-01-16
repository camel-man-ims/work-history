🛸🌎🏴🏳🍌🍎

1. 아티스트 등록 🍌 UPDATE role ✔
2. 유저 권한 체크 ✔
3. 판매관리 🍌 GET ✔
🍎날짜 팬이름, 내용, 공개범위, 상태(요청,제작중,완료,취소) : 발송중 (X)🍎
4. 프로필 설정 🍌 프로필 정보 🎨ARTIST & USER🎨 GET ->
🍎프로필 사진, 이름, 닉네임, 소개, 분야, 취향분야🍎   ✔
5. 프로필 사진 바꾸기 🍌 UPDATE
6. 알림설정 🍌 UPDATE
7. 유저 -> 아티스트에게 요청 🍌 CREATE payment    ✔
8. 유저 로그인 했는지 확인 🍌 Auth CHECK ✔
9. user -> 🍌GET payment ( 유저 결제 관련 페이지 )    ✔
10. artist -> 🍌GET payment ( 아티스트 결제 관련 페이지 ) ✔
11. 아티스트 상태 변경 -> 🍌 UPDATE payment ( 거부도 포함 )
12. user 승인 -> 🍌 UPDATE payment
13. dotvideo 전송 -> send email / 직접전송 🍌 GET 고객 요청정보
14. 아티스트 🍌 GET 총 물감개수 ✔ ( = 유저 물감갯수. 19번이랑 동일 )
15. 아티스트 🍌 GET 정산가능한 물감개수 
16. 수익내역 ->  🍌GET 🍎 형태, 컨버스 이름, 고객이름, 물감개수, 보낸날짜 🍎
17. 정산내역 -> 🍌GET 🍎물감개수, 정산금액, 정산날짜🍎
18. 유저가 몇 번 보냈는지 체크    ✔
19. 유저 물감갯수 가져오기  ✔

🤡구현 하면서 추가해야 될 부분🤡
1. artist cash_need_amount update

🥽기획 건의사항🥽
1. 🍎날짜 팬이름, 내용, 공개범위, 상태(요청,제작중,완료,취소) : 발송중 (X)🍎 ✔
2. 한 아티스트에게 요청 보내는 횟수 제한 -> 최대 3회까지 ✔
3. payment 흐름?
4. user가 요청할 때 canvas? ✔
5. scale up - scale out 설명 ✔
6. 변환되는 화폐의 물가? paint cash 10000원 - 100페인트 100대1 ✔
--> 500페인트 ✔
7. 랜딩페이지 -> 프리티어 free tier ✔ 1GB 2gb 한달에 17000원?
8. 아티스트 paint_need_amount? -> 일단 아티스트한테 박아둠 :
canvas에 적혀있는것 ✔
9. paint -> BIgdecimal(소수점)  || Integer ✔
10. 정산가능한 물감개수?  --> 보류  2주뒤에 정산  ✔ 
11. 알람설정?  ---> ✔beta
12. 마이페이지 -> 고객 마이프로필?✔ 

canvas에 적혀있는것
paint 돈이 나가는거지
요청내용
받을 이메일(선택)
canvas


🏴  구현 남은 목록 🏴 : Canvas API , Search API

🏳 수정해야 할 API 목록 🏳

Update -> 수정된 값 바로 return 해주기
GET -> user정보 넣어주기, 댓글정보 같이 넣어주기
created_at , updated_at 시간 넣어주기

* 시간정보 수정 *

🌎구현해야 할 목록🌎

1. thumbnail 설정 - thumbnail 반환 - 영상 올라가면 동기적으로 반환이 되게
--> 다른 사이트들은 올리고 바로 재생이 되나?
2. https 적용
3. scale up 적용 ( auto scale up )
4. docker ci/cd를 통한 배포

5. 이메일 인증 - git merge ( 합치기 )

6. 내 활동
-> beta
내가 좋아요 누른 게시글
게시글 댓글
내 댓글 

🛸
1. Bearer token
2. 토큰 안 줬을 때 에러처리 할 수 있게

🌎구현해야 할 목록 LATER🌎
1. logging 작업
2. 결제모듈