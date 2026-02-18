---
linkTitle: ▪PC로DMR수신
title: 컴퓨터만으로 DMR 수신 (BM의 새로운 Hoseline)
# description:
type: docs
weight: 120
---

{{% pageinfo %}}

글. HL5KY (2021년 6월 26일)

{{% /pageinfo %}}


Hoseline은 브랜드마이스터에서 제공하는 서비스로, 무전기가 없어도 인터넷의 웹브라우저를 통해서 DMR교신을 들을수 있는 서비스입니다. 이전에도 있던 기능이었지만, 시스템이 불안정해서 몇년전에 서비스를 중단하였다가 이번에 다시 내놓은 것입니다.

음질이 아주 좋아졌고, 여러 송신자의 음량을 평준화시켜서(Normalize) 들려주기 때문에 아주 편안하게 수신이 됩니다.

웹주소는 이전과 같습니다.
https://hose.brandmeister.network

크롬, 파이어폭스, 사파리 등의 웹브라우저에서 가능하고, 익스플로러에서는 작동하지 않습니다. 물론 모바일 장치에서도 가능합니다.

위의 웹주소로 연결하면 아래와 같은 화면이 보이며, 기능은 아래와 같습니다.
- 기본 화면에서는 tg90 ~ tg9999까지만 보여줌. (5자리 이상의 TG는 아래쪽에서 설명함)
- TG91에서 '0:42 ago'는 42초 전에 최종 송신이 되었다는 뜻.
- 적색으로 표시된 TG는 현재 송신중인 TG.
- 가장 먼저 송신이 시작된 TG의 송신음이 들리게 됨.
- TG에서 더블클릭하면 해당 TG만 수신됨.
- RegEx mode는 원하는 TG만 찾는 기능.

<img src="/networks/img/hoseline_1.jpeg" style="width:800px;height:600"><br>
<br>

오른쪽 위에 있는 PLAYER라는 글자위를 누르면 아래와 같은 화면이 보입니다. TG번호를 입력하여 추가할 수 있으며, 5자리 이상의 TG도 입력이 가능합니다. 입력한 TG중에서 먼저 송신하는 신호가 수신됩니다. 이렇게 입력한 TG의 내용은 저장이 되므로, 브라우저를 다시 시작하더라도 그대로 유지됩니다.<br>

<img src="/networks/img/hoseline_2.jpeg" style="width:350px;height:600"><br>
<br>

입력한 TG중에서 하나의 TG만 수신하려고 할때는, TG번호에 한번 클릭하면 적색으로 변하면서 그 TG만 수신됩니다.<br>
솔로모드를 해제하려면 다시 TG번호를 클릭하면 해제됩니다.<br>

<img src="/networks/img/hoseline_3.jpeg" style="width:350px;height:600"><br>
<br>

수신을 할때 레벨메타(VU메타)로 음의 세기를 표시합니다. 색상을 보고도 대략 크기를 판단할 수 있습니다.
- 오렌지색 : -30dB 이하
- 녹색 : -30 ~ 0 dB
- 적색 : 0 ~ +8dB<br>

<img src="/networks/img/hoseline_4.jpeg" style="width:350px;height:600"><br>