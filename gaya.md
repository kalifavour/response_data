# Request site
```python
Host : https://www.gayacc.com
URL = {
	"getSession": "/main_new.php",
	"login": "/member/login.update2.php",
	"viewCal": "/reserve.php?location=01", # 정규 18홀 인터넷예약
	"dayClick": "/modules/ReserveSchedule/ifm_Reserve_Checking.php",  # 달력날짜 클릭
	"timeClick": "/modules/ReserveSchedule/ifm_Reserve_SPselect.php", # 티 타임 클릭
	"confirm": "/modules/ReserveSchedule/ifm_Reserve_Confirm.php" # 부킹 확정
}
```

# Data
| Page          | DATA (신어:1, 낙동:2, 김해:3, 가락:5)                                                      |   
|---------------|------------------------------------------------------------------------------------------|
| 0. Login      | reurl=main_new.php                                                                       |   
|               | login_Page=/main_new.php                                                                 |   
|               | mem=nmem (비회원) , mem=mem(회원)                                                         |   
|               | mb_id=010xxxxyyyy # 회원번호(회원), 전화번호(비회원)                                       |   
|               | mb_pw=xxxx # 네자리숫자                                                                   |   
|               | x=28                                                                                     |   
|               | y=23                                                                                     |   
| 1. Resv (GET) | ( X )                                                                                    |   
| 2. Cal_Click  | Day_Choice_dtn=20240530                                                                  |   
|               | check_Day=143697319                                                                      |   
|               | Day_WTYPE=0                                                                              |   
|               | NINE_HOLE=                                                                               |   
|               | Day_Daekiyn=N                                                                            |   
|               | Course_Gubun=M                                                                           |   
| 3. Time_Click | Choice_SPDate=20240530                                                                   |   
|               | Choice_course=1 #1,2,3,5                                                                 |   
|               | Day_WTYPE=0                                                                              |   
|               | NINE_HOLE=                                                                               |   
|               | Str_Hole=18홀                                                                            |   
|               | Str_Course=1 # 1,2,3,5!!! 3, 4 단계에서 값이 다름 !!!                                     |   
|               | Choice_Time=0514                                                                         |   
|               | Course_Gubun=M                                                                           |   
| 4. Confirm    | Choice_Date=20240530                                                                     |   
|               | Choice_course=1 # 1,2,3,5                                                                |   
|               | Choice_Time=0514                                                                         |   
|               | Str_Course=신어 # 3, 4 단계에서 값이 다름 !!!                                              |   
|               | Str_Hole=18홀                                                                            |   
|               | Choice_hp=010xxxxyyyy #전화번호                                                           |   
|               | Course_Gubun=M                                                                           |   
|               | Lock_Serve_Sec=2024-05-17 20:06:01.671504                                                |   
|               | Server_to_sec=                                                                           |   
|               | imageField2.x=21                                                                         |   
|               | imageField2.y=9                                                                          |   

# Data detail
| element        | 신어                                                              | 낙동          | 김해         | 가락         |
|----------------|-------------------------------------------------|--------------|--------------|--------------|
| x,y            | ![login](images/login_button.jpg)51 x 50 이내                     |              |              |              |
| check_Day      | 123456789(key) + 20250125(부킹날짜)                               |              |              |              |
| Day_WTYPE      | 평일:0, 토요일:2, 일요일 or 공휴일:1, 특별한 일요일:3 ( 검증 필요! ) |              |              |              |
| Choice_course  | 1                                                                | 2            | 3            | 5            |
| Str_Course     | 1 (3단계)                                                         | 2           | 3            | 5            |
|                | 신어 ( 4단계)                                                     | 낙동         | 김해         | 가락         |
| Str_Hole       | 18홀                                                             |              |              |              |
| Course_Gubun   | M                                                                | M            | M            | M            |
| Lock_Serve_Sec | 2024-05-14 10:13:38.537623                                       |              |              |              |
|                | datetime.now().strftime('%Y-%m-%d %H:%M:%S.%f')                  |              |              |              |
| imageField2.x  | ![login](images/reserve_button.png)34 x 22 이내                  |              |              |              |
| imageField2.y  |                                                                  |              |              |              |
