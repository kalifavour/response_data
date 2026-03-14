# Encoding : EUC-KR

```python
import urllib.parse

data = {  # 사람이 볼수 있는 그대로!!
    "Choice_Date": "20240530",
    "Choice_course": "1",
    "Choice_Time": "0514",
    "Str_Course": "신어", 
    "Str_Hole": "18홀",  
    "Choice_hp": "010xxxxyyyy",
    "Course_Gubun": "M",
    "Lock_Serve_Sec": "2024-05-17 20:06:01.671504", 
    "Server_to_sec": "",
}

encoded = urllib.parse.urlencode(data, encoding='euc-kr').encode('ascii')

headers = {
    "Content-Type": "application/x-www-form-urlencoded; charset=EUC-KR"
}

session.post(url, data=encoded, headers=headers)
```