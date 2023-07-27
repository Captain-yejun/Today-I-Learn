## vue의 router
- 페이지 간 이동을 위한 라이브러리 : url 변경 시, 변경된 영역에 컴포넌트를 갱신

- router 폴더에서 컴포넌트에 대한 url을 지정하여 페이지 이동을 가능하게 만듬
 
![image](https://github.com/bjsystems/rnd/assets/121341413/0ea354e2-e579-4f75-a088-3cbb0e1e2c93)

- path가 /login으로 지정되있는 컴포넌트를 클릭하게 되면, 해당 페이지로 이동하면서 url 변경

![image](https://github.com/bjsystems/rnd/assets/121341413/7e42e9a7-90b4-485f-8e27-a5e4dd6ff6e9)

<br>

💡 **그 외 기능**
- 라우터 파라미터, 쿼리, 와일드카드 ex) detail/:idx 와 같이 idx 파라미터를 받아 상세정보 출력

- 네비게이션 컨트롤 ex) $router.push/go/back 등으로 특정 페이지로 이동

<br>

## Node의 router
- 클라이언트의 요청 경로(path)를 보고, 이를 서버 내에서 처리할 수 있는 곳으로 전달한다.
ex) 클라이언트가 /detail 경로로 요청을 보낸다면, 서버는 이에 대한 응답 처리를 하는 함수쪽으로 전달

<hr>

💡 **동작 과정**

1. 클라이언트가 url 접근 시 해당 페이지에서 서버쪽으로 요청 경로를 전송
ex) LoginPage.vue에서는 서버쪽 ~~~이런 경로를 확인해주세요. 
<br>

![image](https://github.com/bjsystems/rnd/assets/121341413/f2bfe6b2-1732-4843-83a0-2afc405d6615)
<br>

2. 서버쪽에서 요청이 들어온 경로에서 기능 수행
ex) LoginPage.vue에서 요청하는 /users/login 경로를 서버에서 수행 
<br>

![image](https://github.com/bjsystems/rnd/assets/121341413/d51cd89d-eb8c-440a-a473-93f27179d22f)

<hr>

✔ **정리**
- vue : 페이지 컴포넌트에 클라이언트가 접근이 가능하도록 경로를 설정

- node : 클라이언트가 접근한 경로의 컴포넌트에서 기능적인 부분에 대해 경로를 주면, node에서 해당 경로에 맞는 기능 수행



