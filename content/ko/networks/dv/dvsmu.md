---
linkTitle: ▪dvsMU
title: DVSwitch Multi User 프로그램 공개
# description:
type: docs
weight: 100
---

{{% pageinfo %}}

글. HL5KY (2020년 11월 27일)

{{% /pageinfo %}}


DVSwtich 서버를 직접 설치하지 못하는 친구들을 위해서 멀티 유저용 서버인 DVLink의 사용을 검토해 보았습니다. 그런데 메뉴의 구성이 너무 복잡하고 사용자의 관리도 쉽지가 않았으며, DVSwitch의 업그레이드를 반영하지 못하는 등 여러가지 문제가 있었습니다. 

고민 끝에 결국 저에게 맞는 별도의 프로그램을 작성하였습니다. 프로그램의 이름은 dvsMU (Multi User)이며 DVSwitch 서버에 추가하는 보조 프로그램입니다. 즉 DVSwitch와 함께 사용하는 프로그램입니다. 한국의 사용자에게만 제공하며 한국용 DVSwitch 이미지에는 이 기능을 포함하여 제공합니다.

이렇게 안정된 프로그램이 나오기까지 HL2DRY, DS5QDR 두 분의 꼼꼼한 테스트와 여러가지 좋은 의견이 큰 도움이 되었습니다. 깊은 감사의 말씀을 드립니다.

<img src="/networks/img/dvsmu.png" style="width:800px;height:600"><br><br>

### dvsMU의 특징
- 하나의 서버에 최고 40 명의 사용자를 추가할 수 있다.
- 전체 사용자의 호출부호, DMR ID, USRP Port 현황을 한 화면에서 볼 수 있다.
- 별도의 설치방법을 제공하므로 여러 가지 목적으로 사용이 가능하다.
- 각 사용자가 각자의 매크로를 사용할 수 있다.
- 각 사용자가 각자의 즐겨찾기를 관리할 수 있다.
- 추가사용자는 DMR만 가능하다.
- DVSwitch의 업그레이드를 반영할 수 있다.
- 업그레이드시 각 사용자의 정보는 자동으로 재설정된다.
- dvsMU의 업그레이드도 메뉴에서 가능하다.
- 시스템 최적화를 통해서 보다 안정된 시스템을 만들 수 있다.

상세한 내용은 {{< newtabref href="https://github.com/hl5ky/dvsmu/blob/main/README.md" title="dvsMU의 설명" >}} 참고

### dvsMU의 사용 방법
새롭게 DVSwitch를 사용할 경우 : dvs_v1.68 이미지에 dvsMU가 포함되어 있음<br>
이미 DVSwitch서버를 사용중인 경우 : 별도의 설치방법으로 추가 설치<br>
DVPi에 추가하여 사용하는 경우 : 별도의 설치방법으로 추가 설치<br>

### 새로운 이미지 및 사용설명서 다운로드 방법
DVSWitch 서버에 dvsMU를 포함하여 새로운 이미지를 만들었습니다. 사용설명서에도 새로운 내용을 추가하였음.<br>
https://drive.google.com/drive/u/2/folders/1ORv7ehiaA3olCU5YMU7j8d4y7i2xTj08

### dvsMU의 추가 설치 방법
현재 DVSwitch 또는 DVPi를 사용하는 경우에 아래와 같이 추가로 설치할 수 있습니다.<br>
사용설명서는 위의 다운로드 사이트에서 내려받을 수 있음.<br>
sudo wget https://github.com/hl5ky/dvsmu/raw/main/setup<br>
sudo chmod +x setup<br>
sudo ./setup<br>

### 오라클 클라우드에 설치시 필요한 추가 설정
- 로칼 시간 설정 (자동리부팅 등의 시간 설정시 로칼시간으로 입력)  https://blog.buffashe.com/2020/02/changing-ubuntu-timezone
- 디스크 SWAP 설정  https://yeon-kr.tistory.com/174
- 추가사용자의 포트 개방  https://kibua20.tistory.com/124<br>
   > 보안 정책 확인 : sudo iptables - -list<br>
   > 포트 개방 : sudo iptables -I INPUT 5 -i ens3 -p udp - -dport 50050 -m state - -state NEW,ESTABLISHED -j ACCEPT<br>
   > 방화벽 정책 저장 : sudo netfilter-persistent save
<br>

DVSwitch에 대한 내용은 {{< newtabref href="/networks/dv/dvswitch" title="DVSwitch 서버 공식 릴리즈" >}}를 참조하시기 바랍니다.<br>


