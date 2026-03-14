| comment                 | element             | nextMonth | CalDayClick  | Time (Booking)   | Confirm             |
|-------------------------|---------------------|-----------|--------------|------------------|---------------------|
|                         | clickTdId           |           | A20240421    | A20240421        | A20240421           |
| 토(sat)/일(hol)/평일('') 구분 | clickTdClass        |           | hol, sat, '' | hol              | hol                 |
| 작업 달                    | workMonth           | 202404    | 202404       | 202404           | 202404              |
| 부킹 원하는 날짜(클릭한 달력날짜)     | workDate            |           | 20240414     | 20240414         | 20240414            |
| 부킹 날짜 (위 칸과 동일)         | bookgDate           |           |              | 20240414         | 20240414            |
| 부킹 시간                   | bookgTime           |           |              | 1801             | 1801                |
| 부킹 코스                   | bookgCourse         |           | ALL          | 1:Ma, 2:Bl, 3:Os | 3                   |
|                         | searchTime          |           |              |                  |                     |
|                         | selfTYn             |           |              | N                | N                   |
|                         | selfRYn             |           |              |                  |                     |
|                         | temp001             |           |              |                  |                     |
|                         | bookgComment        |           |              |                  |                     |
|                         | memberCd            | 1f        | 1f           | 1f               | 1f                  |
|                         | temp007             |           |              |                  |                     |
|                         | agencyReservationYn | N         | N            | N                | N                   |
| 암호: 시간[예약]에 클릭마다 1씩증가   | certSeq             |           |              |                  | 2024040256720( + 1) |
| 매크로 막기 위한 숫자 입력         | certNoChk           |           |              |                  | 58                  |
|                         | agencyBookgName     |           |              |                  |                     |
|                         | agencyHp1           | 10        | 10           |                  |                     |
|                         | agencyHp2           |           |              |                  |                     |
|                         | agencyHp3           |           |              |                  |                     |
|                         | agreeYn             | Y         | Y            | Y                | Y                   |

- certSeq, certNoChk는 Time(Booking) 단계의 response에서 볼수있다. json형태로 들어옴.