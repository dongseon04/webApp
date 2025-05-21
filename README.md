# webApp
1. 새 폴더 만들고 터미널에 가상환경 만들기
`conda create -n webApp python=3.9`
![image](https://github.com/user-attachments/assets/35bafce9-6776-4519-a622-4a2a824773ae)
2. flask 프레임워크 설치
`pip install flask  `
3. app.py 새로운 파일 만들고 flask 구조 완성하기
- 아래는 Flask를 이용해 이름과 전화번호를 입력받아 addbook.txt 파일에 CSV 형식으로 저장하는 간단한 웹 애플리케이션 코드입니다. HTML 템플릿도 함께 포함되어 있습니다.
![image](https://github.com/user-attachments/assets/48d5bb02-5441-48f8-a1ee-36698bb1cf61)
4. index.html
![image](https://github.com/user-attachments/assets/4242d6f3-33c5-4576-aa89-5de75fc1854a)
5. 프로그램 실행
`python app.py`
- 브라우저에서 http://127.0.0.1:5000로 접속하여 이름과 전화번호를 입력하고 저장할 수 있습니다.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Address Book</title>
    <!--CSS 파일 연결-->
    <link rel="stylesheet" href="/static/css/style.css">
</head>
<body>
  <h1>Address Book</h1>
  <form action="/add" method="post">
      <label for="name" class="label-name">Name:</label>
      <input type="text" id="name" name="pyname" required>
      <br><br>
      <label for="phone">Phone:</label>
      <input type="text" id="phone" name="pyphone" required>
      <br><br>
      <button type="submit">Add Contact</button>
  </form>
</body>
</html>


