## 정적 웹 페이지 (Static Web Page)

- 서버(웹 서버, Web Server)에 **미리 저장된 파일**(HTML 파일, 이미지, JavaScript 파일 등)이 그대로 전달되는 웹 페이지
- 서버는 사용자가 요청(Request)에 해당하는 저장된 웹 페이지를 보냄
- 사용자는 서버에 저장된 데이터가 변경되지 않는 한 고정된 웹 페이지를 보게 됨

<img src="https://t1.daumcdn.net/cfile/tistory/24148634579822C52B"/>

## 동적 웹 페이지 (Dynamic Web Page)

- 서버(웹 서버, Web Server)에 있는 데이터들을 스크립트에 의해 **가공처리한 후 생성**되어 전달되는 웹 페이지
- 서버는 사용자의 요청(Request)을 해석하여 데이터를 가공한 후 생성됭되는 웹 페이지를 보냄
- 사용자는 상황, 시간, 요청 등에 따라 달라지는 웹 페이지를 보게 됨

<img src="http://i1.wp.com/lh3.googleusercontent.com/-1jVzhuqATjw/Vqd54V1mrtI/AAAAAAAAACc/Cjt-etlXrHc/w720-o/dynamic-web.png?w=734&ssl=1"/>

## 정적 웹 페이지 vs 동적 웹 페이지

<img src="http://i0.wp.com/lh3.googleusercontent.com/-mFaOm0EGIvA/VqeJYe_b_yI/AAAAAAAAADA/FDiCN9Zp_hg/w720-o/static-vs-dynamic-web-inside.png?w=734&ssl=1"/>

- **정적 웹 페이지 장점**
    - 빠르다 : 요청에 대한 파일만 전송하면 되기 때문에 추가적인 작업이 없음
    - 비용이 적다 : 마찬가지로 웹 서버만 구축하면 됨
- **정적 웹 페이지 단점**
    - 서비스가 한정적이다 : 저장된 정보만 보여줄 수 있음
    - 관리가 힘들다 : 추가/수정/삭제의 작업 모두 수동
- **동적 웹 페이지 장점**
    - 서비스가 다양하다 : 다양한 정보를 조합하여 동적으로 생성하여 제공 가능
    - 관리가 쉽다 : 웹 사이트 구조에 따라서 추가/수정/삭제 등의 작업이 용이
- **동적 웹 페이지 단점**
    - 상대적으로 느리다 : 사용자에게 웹 페이지를 전달하기 전에 처리하는 작업이 필요
    - 추가 비용이 든다 : 웹 서버외에 추가적으로 처리를 위한 어플리케이션 서버(Web Application Server)가 필요