---
linkTitle: ▪NoraVR
title: NoraVR 가상리피터
# description:
type: docs
weight: 70
---

{{% pageinfo %}}

글. HL5KY (2019년 10월 3일)

{{% /pageinfo %}}

▷ <b><span style="font-size:120%">NoraVR이란</span></b>

NoraVR(Nora Virtual Repeater)은 NoraGateway를 이용한 인터넷상의 가상리피터입니다. NoraVR 역시 AMBE보코더를 사용하여 만든 서버이므로 NoraVR서버라고도 부릅니다. 일반리피터는 무전기로 연결을 하지만, NoraVR은 안드로이드장치로 연결합니다. 이때 안드로이드장치에는 클라이언트 프로그램을 설치합니다.
 
<img src="/networks/img/noravr_1.jpeg" style="width:550px;height:600"><br>

NoraVR서버는 AMBE를 사용하는 AMBE서버와도 유사점이 많고 Peanut과도 혼동이 될수 있습니다. 각각의 기능을 비교하여 아래의 표로 정리하였습니다.


<img src="/networks/img/noravr_2.jpeg" style="width:500px;height:600"><br>

NoraVR의 가장 큰 특징은 여러사람이 동시에 사용할수 있고, 리플렉터를 자유롭게 변경할수 있다는 것입니다. 물론 연결된 사람이 각각 다른 리플렉터를 사용하지는 못하고 동일한 리플렉터를 사용해야 합니다. 리피터를 공유하는 개념입니다.
<br><br>

▷ <b><span style="font-size:120%">NoraGateway란</span></b>

NoraGateway는 일본의 JI1ROJ가 만든 프로그램으로 리피터와 컨트롤 프로그램을 함께 가지고 있습니다. pi-star와 비슷한 개념의 소프트웨어입니다. 일본의 햄들은 리피터를 통해 서로 교신을 하지만, 리피터를 통해서 리플렉터를 연결할수 없습니다. 또한 외국의 핫스팟을 구입하면 리플렉터는 연결할수 있지만 일본의 리피터를 연결할 수가 없습니다. 이런 문제점을 해결하기 위해서 개인이 만든 프로그램이 NoraGateway입니다. 일본내 리피터도 사용이 가능하고, 리플렉터도 연결할수 있습니다.

D-star만 가능하지만, 여러 가지 다양한 형태로 사용이 가능합니다. DVMEGA나 MMDVM보드를 연결할수도 있고, 일본판 BlueDV앱도 있습니다. 모두 NoraGateway를 사용합니다. 이런 다양한 사용방법중의 하나가 NoraVR입니다.
<br><br>

▷ <b><span style="font-size:120%">NoraVR의 사용예</span></b>

개인적으로 NoraVR을 구축하고, 안드로이드 클라이언트를 이용하여 혼자만 사용할수도 있지만, NoraVR을 공개하여 주변의 여러사람이 함께 사용할수도 있습니다. 또는 클럽국의 호출부호로 NoraVR을 구축하고 여러사람이 함께 사용할수도 있습니다.

D-star무전기나 핫스팟을 가지지 않은 사람들이 D-star를 경험할수 있기 때문에 D-star사용자를 늘릴수 있는 좋은 방법이라고 생각합니다. 더구나 XRF071등을 사용할때는 D-star등록도 필요하지 않으므로 안드로이드장치에 앱만 설치하면 됩니다.
<br><br>

▷ <b><span style="font-size:120%">NoraVR의 문제점</span></b>

일본이 아닌 외국에서 사용할때의 문제점입니다. 기본 프로그램은 JARL서버를 연결하도록 되어 있습니다. 하지만 외국 호출부호로는 JARL의 D-star서버에 등록을 할수가 없어서 JARL서버의 여러 가지 기능을 사용하지 못합니다. 게다가 JARL서버에 등록하지 않은 외국국이 계속 JARL서버로 접속하면 D-star등록(US-Trust의 등록)을 취소하도록 조치를 취할수도 있습니다.

이러한 문제로 인해 NoraVR을 국내에 소개하지 못하고 있다가, 일본햄들의 도움으로 국외에서도 사용이 가능한 NoraVR 이미지파일을 만들게 되었습니다.
<br><br>

▷ <b><span style="font-size:120%">NoraVR 서버의 구축방법</span></b>

2가지 방법이 있습니다.
1. 라즈베리파이 + ThumbDV (또는 PAMBE보드) : 1대의 라즈베리파이 사용
2. 라스베리파이 + AMBE서버 : 2대의 라즈베리파이 사용

상세한 내용은 첨부파일 (NoraVR서버_설치방법.pdf)을 참조하시기 바랍니다.

* PAMBE보드 또는 PAMBE서버인 경우, version2보드를 사용해야 합니다. 기존의 version1의 회로를 조금만 변경하면 version2로 바꿀수 있습니다. 참고로 현재 국내에 있는 PAMBE서버는 대부분 version1입니다.

PAMBE보드_버전2_개조방법.pdf (아래의 다운로드 페이지 참조)
<br><br>

▷ <b><span style="font-size:120%">NoraVR 클라이언트 프로그램 설치 및 사용방법</span></b>

안드로이드용 프로그램인 NoraVR클라이언트의 설치 및 사용방법은 첨부파일 (NoraVR클라이언트_사용방법.pdf) 참조.
<br><br>

▷ <b><span style="font-size:120%">프로그램 다운로드 사이트</span></b>

{{< newtabref href="https://drive.google.com/open?id=1ORv7ehiaA3olCU5YMU7j8d4y7i2xTj08" title="서버이미지파일 및 안드로이드용 클라이언트 프로그램 다운로드 사이트" >}} 새창에서 열기<br>
실제 설치는 상세 설명서를 참조하시기 바랍니다.

끝으로 도움을 주신 분들께 감사드립니다.<br>
JI1ROJ, JR1OFP, JR2XKN/HL2, JH1BLT








