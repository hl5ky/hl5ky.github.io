---
linkTitle: ▪속도와해독도
title: 전신 속도와 해독도 (CT1BQH)
# description:
type: docs
weight: 142
---

{{% pageinfo %}}
2026년 7월 29일
{{% /pageinfo %}}

요즘 HamClock이 유행이다. 나는 HamClock을 사용하지 않고 있었는데, 어제 DS5TUK님의 도움으로 TUK님이 구축하신 서버에 접속하여 OpenHamClock이라는 프로그램을 사용할 수 있게 되었다.

HamClock에는 여러 가지 기능이 있는데, 그중에 VOACAP는 전파 상태 예측에 아주 편리하다. 유럽까지의 전파 상태를 알아보니 14MHz에서는 거의 아침 9시까지도 전파 상태가 괜찮은 것으로 나타난다. VOACAP은 현재의 전파 상태로 예측하는 것이 아니고 오랫동안 쌓인 데이타를 기준으로 분석하는 것이기 때문에 현재의 상태와는 차이가 있지만 큰 그림은 거의 비슷하다.

<img src="/recording/img/voacap_eu.png" style="width:700px;height:256"><br>

7시 30분에 기상하여 14MHz를 수신해 보니, 포르투칼국이 CQ를 내고 있었다. 프리픽스는 수신되는데 서픽스는 단점이 확실히 들리지 않아서 B(-...)인지 D(-..)인지 구분하기 어렵고, S(...)인지 H(....)인지 구분이 어려웠다.

<br>
<audio style="width: 100%; max-width: 850px; border: 1px solid black; border-radius: 20px; box-sizing: border-box; display: block; margin: 0 auto;" src="https://hl5ky-hp.pages.dev/HL5KY_CT1BQH_260729.mp3" controls></audio>
<br>
<br>

상대의 신호를 분석해 보니 단점의 길이가 약 33ms 정도다. 1200/단점길이(시간)=36.36. 즉 36wpm 정도의 속도로 송신한 것이다. 단파대의 교신으로는 빠른 속도다. 노이즈의 강도가 S3~4이고 신호는 S2~5 정도로 페이딩이 있는 상태여서 수신이 쉽지 않았다. 아마도 원거리 교신보다는 유럽 내의 교신을 기대하고 CQ를 낸 것으로 보인다.

(분석에 사용한 프로그램은 ocenaudio라는 오디오 편집 프로그램으로 무료다.)

통신에서의 기본은 신호의 상태가 좋지 않을 때는 정보의 속도를 낮추어야 한다. CW에서 속도가 빠르면 장단점의 구분, 특히 단점과 단점의 간격 구분이 어려워서 정확한 부호의 해독이 어렵다. CW뿐만 아니라 모든 통신이 마찬가지이며, 인간의 귀도 그렇고 컴퓨터도 속도가 빠르면 해독도가 떨어진다. FT-8은 속도가 일정하게 정해져 있지만, 대부분의 디지털 통신은 전파 상태에 따라서 같은 모드라도 속도 또는 밴드폭을 바꾸어서 교신할 수 있도록 다양한 변형 모드를 제공한다.

CW에서의 적정 속도는 노이즈와 실제 신호 크기의 차이(S/N비)에 의해서 결정된다. 7MHz 국내 교신이라면 S/N비가 워낙 크기 때문에 30~40wpm 이라도 큰 문제 없다. 원거리 교신에서는 대부분 S/N비가 낮기 때문에 25wpm 이내로 낮추는 것이 좋다. CT1BQH의 CQ는 36wpm의 속도이지만, 저는 23wpm으로 송신하였다. 나중에 상대도 속도를 조금 낮추어서 송신해 주었다.

아래의 교신 내용을 보면, 상대가 CQ를 낼 때 제가 상대의 호출부호를 잘 못 인식하고 호출하였다. 나중에 상대가 자신의 호출부호를 정정해 주어서 잘 못 수신한 것을 알 수 있었다. 이때는 확실히 수신했다는 것을 상대에게 인지시켜 주는 것이 좋다.


- CQ CQ CQ CT1BQS CT1DQS K
  (상대의 호출부호가 확실하지 않음)

- CQ CQ CQ CT1BQS CT1BQS K
  (호출부호를 이렇게 수신함)

- <span style="color:blue">HL5KY</span>

- HA?

- <span style="color:blue">HL5KY</span>

- HL?

- <span style="color:blue">HL5KY</span>

- HL5KY DE CT1BQH [BT] GE OM ES TNX FER CALL [BT] UR RST RST IS 559 55N QSB [BT] MY NAME NAME IS CARLOS CARLOS ES QTH QTH IS NR TOMAR NR TOMAR [BT] SO HW CPI? [AR] HL5KY DE CT1BQH [KN]

- <span style="color:blue">CT1BQS DE HL5KY   GM CARLOS   UR 55N 55N QSB   OP JOE JOE   PWR 5TT W   ES   4EL 4EL YAGI   HW?   CT1BQS DE HL5KY K</span><br>
   (여전히 상대의 호출부호를 CT1BQS로 알고 있음. 상대의 출력과 안테나가 궁금해서 이쪽의 정보를 먼저 알려줌.)

- HL5KY HL5KY DE CT1BQH H H CT1BQH [BT] SOLID CPI JOE   TNX FER RPRT ES INFO [BT] NW SIGS HV PEAKED 599 5NN IN QSB [BT] MY RIG IS IC7300 PWR IS 90 90 WATT ES ANT IS 6EL TRIBAND YAGI [BT] WX IS CLEAR ES TEMP NW IS 21C 21C [BT] QSL QSL VIA EQSL EQSL ES LOTW LOTW [BT] NW QRU SO JOE MNI TNX NICE QSO ES BCNU GL BEST 73 73 HAVE A NICE DAY GB [AR] HL5KY DE CT1BQH [SK] E E<br>
  (첫 부분에서 자신의 호출부호 끝글자가 H라고 여러번 말함)

- <span style="color:blue">R FB CT1BQH CFM CARLOS [BT] 2ND 2ND QSO HI [BT] HR WX FINE ES 25C 25C WARM [BT] TNX 2ND QSO 73 BCNU CT1BQH DE HL5KY [SK]</span><br>
  (호출부호를 잘 수신했음을 확인함)

- OK JOE THIS IS OUR 2ND QSO ?? FIRST ONE WAS BACK IN SEPTEMBER 2024 ?? [BT] SO AGN MNI TNX NICE QSO ES BCNU TAKE CARE ES BEST 73 73 GB JOE [AR] HL5KY DE CT1BQH [SK] E E

- <span style="color:blue">73 TU E E</span><br>

- E



