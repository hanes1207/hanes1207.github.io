# images 폴더 사용법

이 폴더에 사진/동영상을 넣으면 index.html에 자동으로 표시됩니다.
파일이 없으면 해당 자리는 자동으로 숨겨지므로(onerror), 일단 비어 있어도 페이지는 깨지지 않습니다.

## 프로필 사진
- `profile.jpg` — 상단 소개 옆에 들어갈 본인 사진 (세로형 권장, 예: 600x740px)

## 프로젝트 미디어 (예시 파일명, 원하는 대로 바꿔도 됨)
- `mdr_demo.mp4`, `mdr_1.jpg`        — LLM-guided robot
- `nubzuki_adventure.mp4`, `nubzuki_1.jpg`, `nubzuki_2.jpg` — Nubzuki's Adventure
- `imm_1.jpg`                        — IMM maneuver detection
- `han_1.jpg`                        — Pathway-aware HAN

## 추가 방법
- 사진:   index.html의 <div class="media"> 안에  <img src="images/파일명.jpg" alt="설명" onerror="this.style.display='none'">
- 동영상: <video src="images/파일명.mp4" controls preload="metadata" onerror="this.style.display='none'"></video>
- 유튜브: index.html의 .video-embed 주석 블록을 풀고 VIDEO_ID만 교체

> 큰 동영상은 GitHub Pages에 직접 올리면 무거우니, 유튜브 임베드를 추천합니다.
