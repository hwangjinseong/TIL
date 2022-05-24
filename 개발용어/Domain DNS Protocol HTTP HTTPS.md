# 도메인

## 도메인이란?

인터넷에 연결된 컴퓨터를 사람이 쉽게 기억하고 입력할 수 있도록 문자(영문 한글)로 만든 인터넷 주소(URL)입니다.

## **도메인 체계**

도메인은 “.”또는 루트(root)라 불리는 도메인 이하에 아래 그림과 같이 역트리(Inverted tree)구조로 구성되어 있다. 아래와 같이 3단계로 구분된다.

<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Fca0rKb%2FbtrgCE2Hhu6%2FrS3sgqr50V0VyXthdd7Td0%2Fimg.gif">

### **1단계 : 최상위 도메인(TLD, Top-Level Domain)**

도메인 레벨 중에 가장 높은 단계에 있는 도메인이다. 7 개의 일반도메인(com, net, org, edu,, gov, mil, int)과 + 190여개의 국가 도메인(kr, de, jp)으로 구성되어 있다.

1단계 도메인은 도메인의 목적, 종류, 국기를 나타낸다. 최상위 도메인의 형태에 따라 도메인 네임 체계와 등록 원칙이 다를 수 있다.

### **2단계 : 차상위 도메인(SLD, Second-Level Domain)**

도메인의 이름을 등록한 조직을 나타낸다. 예를 들어, 단과 대학과 학술 시설은 ac, 회사는 co와 같은 형태를 가지고 있다.

### **3단계 : 도메인 이름(Domain Name)**

자주 볼 수 있는 naver, google, daum과 같이 우리가 임의로 지정할 수 있는 자율적인 이름을 의미한다.



# DNS(Domain Name System)

## **DNS이란?**

도메인을 도메인이 올라가 있는 웹 서버의 IP로 연결하는 시스템. 웹페이지에 접속하기 위해 필요한 IP를 일일이 챙길 필요 없이 도메인과 IP를 변환해주는 역할을 한다.

### **DNS 하는 일**

DNS는 Domain Name System의 줄임말로, 데이터베이스 시스템이다.호스트의 도메인 이름을 IP 주소로 변환하거나 반대의 경우를 수행할 수 있도록 개발된 데이터베이스 시스템이다.

DNS는 범국제적 단위로 웹사이트의 IP 주소와 도메인 주소를 이어주는 환경/시스템이다.

### **DNS 처리 순서**

브라우저의 검색창에 naver.com을 입력한다.이 요청은 DNS에서 IP 주소(125.209.222.142)를 찾는다.그리고 이 IP 주소에 해당하는 웹 서버로 요청을 전달하여 클라이언트와 서버가 통신할 수 있도록 한다.


# 프**로토콜(Protocol)**

## 프로토콜이란?

컴퓨터나 서버, 통신 장비 등 장치 사이에서 서로 통신하기 위해 미리 정해놓은 규칙이다.

*(TCP/IP, HTTPS, HTTP 등이 모두 인터넷 프로토콜이다.)*

## **프로토콜의 기본 요소**

- **구문(Syntax)** : 전송하고자 하는 데이터의 형식(Format), 부호화(Coding), 신호 레벨(Signal Level) 등을 규정
- **의미(Semantics)** : 두 기기 간의 효율적이고 정확한 정보 전송을 위한 협조 사항과 오류 관리를 위한 제어 정보를 규정
- **시간(Timing)** : 두 기기 간의 통신 속도, 메시지의 순서 제어 등을 규정

## 프로토콜 종류

- 계층: 응용

       프로토콜: HTTP, SMTP, FTP, Telnet

- 계층: 표현

       프로토콜: ASCII, MPEG, JPEG, MIDI

- 계층: 세션

       프로토콜: NetBIOS, SAP, SDP, NWLink

- 계층: 전송

       프로토콜: TCP, UDP, SPX

- 계층: 네트워크

       프로토콜: IP, IPX

- 계층: 데이터 링크

       프로토콜: Ethernet, Token Ring, FDDI, Apple Talk

## **프로토콜의 기능**

- 단편화(Fragmentation)와 재합성(Assembly)

      단편화 : 송신 측에서는 긴 데이터 블록을 손쉽게 전송할 수 있도록 크기가 똑같은 작은 블록으로 나누어 전송

      재합성 : 수신 측에서 쪼개진 작은 데이터 블록을 재합성하여 원래의 메시지로 복원하는 기능

- 캡슐화(Encapsulation)각 프로토콜에 적합한 데이터 블록을 만들려고 데이터에 정보를 추가하는 것플래그, 주소, 제어 정보, 오류 검출 부호 등을 부착하는 기능이다.
- 연결 제어(Connection Control)비연결 데이터 전송(데이터그램)과 연결 위주 데이터 전송(가상회선)을 위한 통신로를 개설·유지·종결하는 기능이다.
- 흐름 제어(Flow Control)데이터양이나 통신속도 등이 수신 측의 처리 능력을 초과하지 않도록 조정하는 기능이다.
- 오류 제어(Error Control)데이터 전송 중 발생할 수 있는 오류나 착오 등을 검출하고 정정하는 기능이다.
- 순서 결정(Sequencing)연결 위주의 데이터를 전송할 때 송신 측이 보내는 데이터 단위 순서대로 수신 측에 전달하는 기능이다.
- 주소 설정(Addressing)발생지, 목적지 등의 주소를 명기하여 데이터를 정확하게 전달하는 기능이다.
- 동기화(Synchronization)두 통신 객체의 상태(시작, 종류, 검사 등)를 일치시키는 기능이다.
- 다중화(Multiplexing)하나의 통신로를 여러 개로 나누거나 회선 여러 개를 하나의 통신로로 변환시켜 다수의 가입자가 동시에 사할 수 있도록 하는 기능이다.
- 전송 서비스(Transmission Service)통신 객체를 사용하기 쉽도록 별도로 추가 서비스(패리티 검사, 보안도, 서비스 등급, 우선순위 등)를 제공하는 기능이다.



# HTTP, HTTPS

## **HTTP**

HTTP는 하이퍼 텍스트 전송 프로토콜의(Hypertext Transfer Protocol)의 약자이다. 웹 상에서 클라이언트와 서버 간에 요청(request) 및 응답(response)으로 정보(데이터)를 주고 받을 수 있는 프로토콜이다. OSI 7계층 중 응용(Application) 계층의 프로토콜로 TCP/IP 위에서 작동한다. TCP와 UDP를 사용하며, 80번 포트를 사용한다.

## **HTTPS**

HTTPS는 하이퍼 텍스트 전송 프로토콜 보안(Hypertext Transfer Protocol Secure)의 약자이다. 일반 HTTP 프로토콜의 문제점은 서버에서부터 브라우저로 전송되는 정보가 암호화되지 않아 데이터가 쉽게 도난당할 수 있다는다는 점이었다. 

HTTPS 프로토콜은 HTTP + 암호화 + 증명서 + 완전성 ****으로 HTTP의 보안적 약점을 보완한 프로토콜이다.

HTTPS는 기본 TCP/IP 포트로 ****443번 포트를 사용한다. HTTPS는 소켓 통신에서 일반 텍스트를 이용하는 대신에, 웹 상에서 정보를 암호화하는 SSL이나 TLS 프로토콜을 통해 세션 데이터를 암호화한다. 

SSL(Secure Socket Layer)은 서버와 브라우저 사이에 안전하게 암호화된 연결을 만들 수 있게 도와주고, 서버 브라우저가 민감한 정보를 주고받을 때 중간에 정보를 도난당하는 것을 막아준다. 

TLS(Transport Layer Security) 프로토콜은 SSL 프로토콜에서 발전한 것이다.

<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Fbrx6RF%2FbtrhetkVuNI%2F8ZWO3bctHfRohzKZo8wd9k%2Fimg.png">

## HTTP 상태코드

- **1xx(정보)**
- **2xx(성공)**
- **3xx(리다이렉션)**
- **4xx(클라이언트 오류)**
- **5xx(서버 오류)**