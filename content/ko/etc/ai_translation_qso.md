---
linkTitle: ▪통역QSO
title: AI를 통역을 이용한 QSO
# description:
type: docs
weight: 40
---

{{% pageinfo %}}

2026년 9월 1일

{{% /pageinfo %}}


아마추어 무선에서도 이제 AI의 통역 기능을 이용하는 시대가 되었다. 지난 한 달간 일본, 아르헨티나의 햄과 함께 이와 관련한 실험을 했다. 결과는 생각보다 상당히 괜찮았다. 물론 통신방식에 따라 다소 차이는 있다.

바로 본론으로 들어가겠다.

### 1. 수신한 소리를 AI로 통역

<div style="text-align: center; margin: 20px 0;">
<img src="../img/ai_qso_1.png" alt="Signal waveform" style="width: 100%; max-width: 850px; height: auto; border: 1px solid #000; border-radius: 5px; box-sizing: border-box;">
</div>

SSB에서는 SN비가 좋지 않으면 통역이 쉽지 않다. SN비 20dB 이상의 신호에 나쁘지 않은 음질로 나오는 경우 통역이 되지만 여전히 불안정하다. 향후 DSP의 발전과 함께 개선이 되겠지만 근본적인 한계가 있다.

FreeDV에서는 잡음이 없기 때문에 상당히 잘 된다.  이것도 역시 음질의 영향을 많이 받는다. FreeDV는 SN비 -2dB 이상이면 해독이 되지만 안정적인 통역을 위해서는 0dB 이상이 좋다. 0dB면 SSB에서는 알아듣기 힘든 신호다.

DMR 등의 DV 통신에서도 FreeDV와 비슷하다. 역시 음질이 중요하다.

결론은, '1의 방식으로는 쉽지 않다'이다.



### 2. 수신한 소리를 AI로 번역하여 화면에 표시

<div style="text-align: center; margin: 20px 0;">
<img src="../img/ai_qso_2.png" alt="Signal waveform" style="width: 100%; max-width: 850px; height: auto; border: 1px solid #000; border-radius: 5px; box-sizing: border-box;">
</div>

위의 1과 거의 비슷하다.

DV 통신에서 PC를 사용할 경우 2의 방식은 아주 편리하다. 한 가지 문제는, 화면에 나오는 내용이 문장을 만들다가 말이 안되면 없어지고 다시 번역을 시작하는 경우가 많아서 화면의 내용을 따라잡기가 불편하다. 하지만 내용을 이해하는데는 거의 문제가 없다.



### 3. 송신자의 목소리를 AI로 통역하여 송신

<div style="text-align: center; margin: 20px 0;">
<img src="../img/ai_qso_3.png" alt="Signal waveform" style="width: 100%; max-width: 850px; height: auto; border: 1px solid #000; border-radius: 5px; box-sizing: border-box;">
</div>

가장 효율이 좋으며 음질에도 크게 좌우되지 않는다. 현재 교신하고 있는 방법이다. 송신하기 전에 이미 외국어로 바꾸어서 무전기로 입력되기 때문에, SSB든 FreeDV든 일반적인 교신이 되는 상태이면 이 방법으로도 교신이 된다.

다만 문제는, 법적인 문제다. 허가받은 운용자의 목소리가 아니고 AI의 목소리가 송신기로 나가는 것이니 문제가 될 수 있다. 하지만 구더기 무서워서 새로운 기술에 대한 호기심을 멈출 수는 없어서 일단 시도하고 있다.

아래는 위 3의 방식으로 교신한 일본햄과 아르헨티나햄의 7MHz FeeDV 녹음 파일이다. 본인들의 목소리가 아니고 AI의 목소리다. 마지막에 파이널 인사하는 부분은 본인들 목소리다. FreeDV라서 잡음없이 깨끗하다.

JA4CXX  (일본어 - AI - 스페인어 - 송신) 녹음 시작 부분<br>
LU5DKI  (스페인어 - AI - 일본어 - 송신) 녹음 4:00분 부터<br>
본인들의 목소리 - 녹음 7:30분 부터<br>

<br>
<div style="text-align: left; margin: 10px 0;">
<div style="display: inline-block; width: 100%; max-width: 850px; border: 1px solid #000; border-radius: 20px; overflow: hidden; vertical-align: middle; box-sizing: border-box;">
<audio controls style="width: 100%; display: block;">
<source src="https://hl5ky-hp.pages.dev/freedv_ja4cxx_lu5dki.mp3" type="audio/mpeg">
</audio>
</div>
</div>
<br>

호출부호를 얘기할 때는 AI가 통역을 잘 못하기 때문에 아주 이상하다. 대화도 해당 언어의 원어민이 들으면 다소 부자연스러울 수는 있다. 이것은 본래의 언어로 얼마나 잘 말하느냐에 달려 있다. 우리가 그냥 말할 때는 완전한 문장을 만들지 않고 말하는 경우가 많아서 통역도 부자연스러울 수밖에 없다. 그렇지만 서로 내용을 이해하는데는 별 문제가 없다.

내가 일본햄과 교신할 때 한국어로 말하고 AI가 통역했는데, 깊이있는 기술적인 문제도 대화에 전혀 어려움이 없었다. 나는 많은 부분을 컴퓨터로 처리했기 때문에 상대의 송신음밖에 녹음을 못했다. 아래는 그 일부이다. 상당히 젊은 목소리다.^ 역시 FreeDV라서 음이 아주 깨끗하다.

<br>
<div style="text-align: left; margin: 10px 0;">
<div style="display: inline-block; width: 100%; max-width: 850px; border: 1px solid #000; border-radius: 20px; overflow: hidden; vertical-align: middle; box-sizing: border-box;">
<audio controls style="width: 100%; display: block;">
<source src="https://hl5ky-hp.pages.dev/freedv_ja4cxx.mp3" type="audio/mpeg">
</audio>
</div>
</div>
<br>


AI는 무료인 '구글 번역'을 사용했다. 안드로이드에는 '번역'이라는 이름의 앱이다. PC에서는 ' http://translate.google.co.kr '로 연결하면 바로 사용이 가능하다. 유료앱에 비해서 기능은 좀 떨어지지만 통역 품질은 충분하다.

휴대폰에서 말을 하고 동시에 통역이 되어서 소리가 나오게 하려면, 선이 있는 이어폰 또는 블루투스 이어폰을 사용해야 한다. 그냥 스피커로 듣는 상태에서는 동시 통역을 제공하지 않는다. 그래서 무전기 또는 컴퓨터와 연결할 때는 선을 이용하거나 오디오 블루투스 동글을 이용한다.

JA4CXX는 80세, LU5DKI는 78세이다. 놀랍지 않은가.  주변을 둘러보면 '나이 들고 재미있는 거리가 없다'고 하는 푸념이 많은데 우리 햄들은 재미있는 거리가 널려 있다. 새로운 기술, 많이들 즐기시고 연구도 하시고 많이 알려주시기 바란다.
