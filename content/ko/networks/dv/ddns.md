---
linkTitle: ▪DDNS 설정
title: DDNS 설정 방법
# description:
type: docs
weight: 210
---

{{% pageinfo %}}

글. HL5KY

{{% /pageinfo %}}


▷ <b><span style="font-size:120%">DDNS의 필요성</span></b>

외부에서 집에 있는 AMBE서버, NoraVR서버, DVSwitch서버 등을 연결하려고 할때, 집에 연결된 인터넷의 IP주소를 알아야 한다. 숫자로 된 IP주소는 여러가지로 불편하므로 DDNS를 사용하는 것이 좋다. DDNS를 사용하면 다음과 같은 장점이 있다.

- 가정의 IP주소가 고정이 아니다.<br>
일반 가정에 주어지는 인터넷은 대부분 고정IP가 아니고 유동IP이다. (수시로 변경될 가능성이 있다) 고정IP는 신청도 쉽지 않고 사용료도 비싸다. 보다 간단한 방법인 DDNS를 사용하는 것이 편리하다.

- 숫자로 된 IP주소는 기억이 어렵다.<br>
IP주소는 기본적으로, 121.146.15.132 등과 같이 숫자로 되어 있어서 기억이 어렵다.<br>
네이버의 실제 IP주소는 210.89.164.90 이지만 편리한 DNS주소(www.naver.com)를 주로 사용한다.<br>
가정의 IP주소도 121.146.15.132 보다는 DDNS(hl5ky.iptime.org)를 사용하면 편리하다.
<br><br>

▷ <b><span style="font-size:120%">DDNS의 설정방법</span></b>

ipTIME 공유기를 기준으로 설명함.<br>

- 웹브라우저(익스플로러 또는 크롬)에서 공유기의 설정 페이지로 접속한다.  주소창에 "192.168.0.1"를 입력하고 엔터를 누른다.<br>

- 설정 페이지에서, [관리도구] - [고급설정] - [ 특수기능] - [DDNS설정] 메뉴로 접속한다.<br>
  초기 로그인 이름과 암호는 모두 admin<br>

- 우측에 내용을 입력하고, <DDNS등록>을 누른다.<br>
   <호스트이름> : 다른 사람과 중복되지 않아야 함. 일반적으로 호출부호를 사용.<br>
   <사용자ID> : 이메일주소를 입력한다.<br><br>

<img src="/networks/img/ddns_1.png" style="width:850px;height:600"><br><br>

등록후, [접속상태]에서 <정상등록>이라고 보이면 등록이 완료된 것이다.<br>
위와 같이 등록이 완료되면, DDNS주소는 "hl5ky.iptime.org"가 된다.<br>


▷ <b><span style="font-size:120%">휴대폰의 클라이언트 프로그램 설정</span></b>

NoraVR 클라이언트와 DVSwitch 클라이언트의 설정에서 주소입력난에 자신의 DDNS를 입력하여야 한다.<br>
예를 들어 아래와 같이 입력한다.<br>

<img src="/networks/img/ddns_2.png" style="width:600px;height:400"><br>