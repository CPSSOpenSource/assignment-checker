# 과제
- 이 기재된 조건을 만족하는 프로젝트를 만드시기 바랍니다. 조건은 아래와 같습니다.


- 다음과 같은 조건을 만족하는 모델을 클래스로 작성하고 데이터베이스에 마이그레이션 작업을 해주시기 바랍니다.
```
- 필드는 3개를 가짐
- 이름, 세부 정보, 점수
```
- http://localhost/main 에 접속하였을 때, hello world! 문장이 나올 수 있도록 설계하세요.
- http://lcoalhost/main/list 에 접속하였을 때, 다음과 같은 HTML 페이지가 나오도록 구현하셔야 합니다.
```html
<html>
!<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8" />
    <title>Main page</title>
</head>
<body>
    <p><a href="John">John</a>의 정보 (점수: 100, 메세지: perfect)</p>
    <p><a href="Amy">Amy</a>의 정보 (점수: 70, 메세지: good)</p>
    <p><a href="Ethan">Ethan</a>의 정보 (점수: 40, 메세지: need to more study)</p>
</body>
</html>
</html>
```

단, 아래와 같이 views.py에 작성하여 페이지 출력하도록 하며
아래 소스 코드처럼 3개의 객체를 만들어서 <code>data_list</code> 리스트 변수에 넣었다고 합니다. 
```python
def index(request):
    data_list = []
    data_list(Information(name="John", score=100, description="perfect"))
    data_list(Information(name="Amy", score=70, description="good"))
    data_list(Information(name="Ethan", score=40, description="need to more study"))
    # 작성해야 하는 부분
```
이 index 함수를 이용하여 http://lcoalhost/main/list 에 접속하였을 때 위에 기재된 html 소스 코드를 클라이언트가 받을 수 있도록
구현하시기 바랍니다.


- SSH를 이용하여 CPSS 과제 서버에 장고 서버를 돌리기 위해서 venv(Python Virtual Environment)를 만들고 pip을 최신 버전으로 업그레이드를 
하여 django 모듈을 설치하시기 바랍니다.

- SFTP를 이용하여 CPSS 과제 서버에 장로 프로젝트를 통째로 올려주시기 바랍니다. 

CPSS 과제 서버는 다음과 같습니다.
```
ip: a1.cpss.network
port: 22
username: 영어 이름 (만약, 이름이 홍길동이라면 gildong)
password: 학번 8자리
```

