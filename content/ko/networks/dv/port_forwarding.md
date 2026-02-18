---
linkTitle: ▪포트포워딩
title: 포트포워딩 설정 방법
# description:
type: docs
weight: 220
---

{{% pageinfo %}}

글. HL5KY

{{% /pageinfo %}}


▷ <b><span style="font-size:120%">포트포워딩의 필요성</span></b>

외부에서 집에 있는 AMBE서버, NoraVR서버, DVSwitch서버 등을 연결하려고 할때,<br>
집에 있는 서버는 내부IP주소를 가지고 있기 때문에 직접 연결할 수가 없다.<br>
포트를 이용하여 연결해야 하는데, 공유기에서 포트를 개방해 주어야 한다.
<br><br>

▷ <b><span style="font-size:120%">포트포워딩의 설정방법</span></b>

ipTIME 공유기를 기준으로 설명함.<br>

- 웹브라우저(익스플로러 또는 크롬)에서 공유기의 설정 페이지로 접속한다.
- 주소창에 "192.168.0.1"를 입력하고 엔터를 누른다.
- 설정 페이지에서, [관리도구] - [고급설정] - [ NAT/라우터 관리] - [포트포워드 설정] 메뉴로 접속한다.
- 초기 로그인 이름과 암호는 모두 admin
- 우측 아래의 [새규칙추가]를 누르고, 내용을 입력한다.
- <규칙이름>은 아무 내용이나 가능함.
<br><br>

> NoraVR 서버가 다음과 같이 구성되었다면, 그림의 내용과 같이 설정함.<br>
- NoraVR의 내부IP주소 : 192.168.0.150<br>
- 프로토콜 : UDP<br>
- 포트번호 : 52161<br>

<img src="/networks/img/PortF_1.png" style="width:850px;height:600"><br><br>

> DVSwitch서버가 다음과 같이 구성되었다면, 그림의 내용과 같이 설정함.<br>
- DVSwitch서버의 내부IP주소 : 192.168.0.160
- 프로토콜 : UDP
- 포트번호 : 50000

<img src="/networks/img/PortF_2.png" style="width:600px;height:600"><br><br>