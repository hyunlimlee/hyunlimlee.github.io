---
layout: post
title: CW 레이다 실험 첫단계
subtitle: 졸업학기 프로젝트를 준비하며
categories: 25Capstone
tags: [project, tech]
banner:
  image: /assets/images/post_image/25_capstone_1.jpg
  opacity: 0.618
  background: "#000"
  height: "100vh"
  min_height: "38vh"
  heading_style: "font-size: 4.25em; font-weight: bold; text-decoration: underline"
  subheading_style: "color: gold"
---

## 25.11.24
**오늘은 Pluto SDR을 사용해 CW 레이다 실험을 진행했습니다.**<br>
<br>
Pluto SDR 사용을 위한 초기 설정으로 다음 두 가지가 있는데요,<br>
<br>
***1. 드라이버 설치하기***<br>
***2. 운용 주파수 늘리기(필요시)***<br>
<br>
이 있습니다.
<br>
Pluto SDR이 기본적으로 제공하는 주파수 제한 범위는 3.5 GHz 이하로 낮기 때문에 내부 해킹을 통해 늘려야 하는데요, SDR 내부에 접속하는 방법은 공식 문서에서 쉽게 확인할 수 있습니다.


👇 코드는 아래 포스트에서 확인하실 수 있어용 👇
<br>
[💻 <span style="color: #4374D9">실험 코드 보러가기</span>](/python/code/2025/11/24/radar_code.html)

어쨌든 드라이버 설치도 완료했고, 운용 주파수 범위도 늘렸습니다.
<br>
그러나 가장 중요한 것은 ***<span style="color: #FF007F">실제로 제가 보유한 Pluto가 CW 레이다용으로 사용할 수 있냐</span>***의 여부겠죠!
<br>
최종적으로는 제가 직접 설계한 2X2 uniform patch array antenna를 Pluto에 연결해 실험을 진행하지만, 아직 해당 안테나 설계가 제대로 되지 않았기 때문에 작년에 설계했던 planar LPDA를 사용했습니다.
<br>
-  <span style="color: #4374D9">**사용한 LPDA 동작 주파수: 2.2 ~ 8.5 GHz**</span>
<br>
해당 안테나와 gemini님이 주신 코드를 사용해 실험한 결과, 다음과 같은 spectrogram이 등장했습니다.
