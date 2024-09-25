---
linkTitle: 450도 로테이터 프로그램
title: 450도까지 지원이 가능한 로테이터 컨트롤 프로그램
# description:
type: docs
weight: 30
---

{{% pageinfo %}}
HL5KY (2024년 9월 25일)
{{% /pageinfo %}}


Kenpro와 Yaesu 로테이터는 대부분 450도까지 회전이 가능합니다. 360도에서 멈추는 것이 아니고, 추가로 90도 더 회전이 되어서 총 450도 회전이 되는 것입니다.

우리나라에서 원거리 교신을 많이 하는 대상은 유럽과 북미입니다. 유럽은 대략 330도, 북미는 대략 30도 정도가 됩니다. 만약 360도만 회전하는 로테이터를 사용한다면 아래 그림의 왼쪽과 같이 회전하는 각도가 큽니다. 450도 회전이 가능한 로테이터는 회전하는 각도가 훨씬 작습니다.

<img src="/etc/img/Rotor_1.png" style="width:400px;height:256"><br><br>

대부분의 Kenpro와 Yaesu 로테이터는 450도를 지원하기 때문에 컨트롤러의 CW/CCW 버튼으로 위와 같이 사용하실겁니다.

그런데, 리모트 상황과 같이 컨트롤러를 직접 사용하지 못하는 경우라면,

컴퓨터를 사용하여 프로그램으로 로테이터를 컨트롤 해야 합니다. PstRotator, HRD, N1MM, ERC 등 여러가지 프로그램이 있지만 아쉽게도 450도를 제대로 지원하지 않습니다. 되긴되는데 50% 아쉽습니다.

다행히 KK5JY라는 분이 만든 프로그램을 보니 상당히 직관적으로 만들었고 소스까지 공개해 두었더군요. 물론 이것도 360도밖에 지원하지 않지만 소스가 있으니 변경이 가능합니다.

제가 프로그램을 만질 실력은 되지 않아서, 변경을 원하는 내용을 설계해서 DS5TUK님께 부탁하여 450도까지 지원하는 형태로 변경하였습니다.<br><br>

<img src="/etc/img/Rotor_2.png" style="width:400px;height:256"><br><br>

필요한 분은 아래의 두 파일을 원하는 폴더에 저장하고 실행하시면 됩니다.


<div class="button_cont">
   <a class="example_d" href="/etc/img/RotorCraft.exe">
    RotorCraft.exe
   </a>
</div>

<br>

<div class="button_cont">
   <a class="example_d" href="/etc/img/AppIcon.ico">
    AppIcon.ico
   </a>
</div>
<br>
<br>
■ 사용방법
<br>
설정<br>
Configure에서 Port와 Speed를 설정하고, Connect를 눌러서 연결한다.<br><br>

회전 (4가지 방법)<br>
1. 원형 그림에서 원하는 각도에 마우스를 올리면 그림과 같이 각도값이 나온다. 더블클릭하면 회전함.<br>
   (각도가 작은 방향으로 회전함)
2. <<는 CCW, >>는 CW를 나타냄. 마우스를 누르고 있는 동안 회전함.
3. 6개의 지정 각도 회전함. 위의 STOP을 누르면 중단됨.
4. Preset Targets. 각도값을 입력하고, Go를 누르면 회전함. 위의 STOP를 누르면 중단됨.
<br><br>

■ 참고<br>
1. 컴퓨터의 프로그램으로 컨트롤 하기 위해서는 인터페이스가 필요함.
2. 인터페이스는 시리얼포트 또는 가상 포트 지원 형태가 되어야 함.
3. 서버가 내장된 형태의 인터페이스에는 맞지 않음.
4. Kenpro 또는 Yaesu의 GS-232B 프로토콜만 지원함.

