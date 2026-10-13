# 싹딜 인터넷 — 민트 모션 리디자인 v2

압축을 풀고 index.html을 브라우저로 열면 됩니다. 설치나 빌드는 필요 없습니다. fonts와 assets 폴더를 함께 유지해 주세요.

## 변경

- 민트 #54E4BF / 딥그린 #007B61 / 어두운 그린 #172D27을 적용했습니다.
- 통신사별 최대 혜택 비교 영역과 연결된 선택 로직을 제거했습니다. 첫 화면 다음에 바로 상담 영역이 이어집니다.
- 선물·와이파이 공유기·금화 3D 이미지를 새로 생성했습니다.
- 와이파이, 선물, 대화, 확인 SVG 아이콘을 직접 작성했습니다.
- 첫 화면 부유 효과, 신호 애니메이션, 스크롤 진행 표시, 신청 절차 아이콘 반응, 버튼 호버와 FAQ 펼침 효과를 추가했습니다.
- 움직임 멈춤/재생과 prefers-reduced-motion 설정을 지원합니다.
- 원본 최대 52만원 예시, 상담 폼, 동의 안내, 신청 절차, FAQ를 유지했습니다. 실제 개인정보를 저장·전송하지 않습니다.

## 검수

1440px 데스크톱, 768px 태블릿, 390px 및 320px 모바일에서 가로 넘침을 확인했습니다. 이미지 로드, 모션 일시정지, 상담 체험 제출, JavaScript 문법, 자산 경로, 비교 영역 제거, 스크롤 진행률과 스크롤이 없는 경우를 확인했습니다.

GitHub 업로드 및 공개 배포는 하지 않았습니다.

## 디자인 참고

- https://www.behance.net/gallery/177448421/Contents-Design-Portfolio-2023
- https://1666-3048.com/

## 이미지 제작

기본 내장 imagegen 도구로 생성했습니다. 최종 자산은 assets/hero-mint-v2.png이며, 아래 프롬프트를 사용했습니다.

Use case: stylized-concept. Asset type: transparent hero illustration for Korean internet signup landing page. Create a premium playful 3D composition: a large floating ivory gift box with vivid mint green satin ribbon, its lid hovering slightly open, a compact white wifi router with two antennas beside it, three glossy gold coins rising around it, a mint wireless signal above. Polished soft clay and satin materials, sophisticated commercial render, mint #18c99c, ivory, gold. Three quarter view, strong dimensionality, objects clearly separated from background, balanced square composition with generous padding, no text, no logos, no background, genuine transparent alpha. The gift box should dominate but router clearly visible. Ready for CSS floating animation.

## v3 색감 수정
네이비·블루·시안 그라데이션, 도트 패턴, 반짝임과 유리 오브젝트를 추가했습니다. 민트 포인트와 기존 모션·상담 기능은 유지합니다. 추가 레퍼런스: https://rkdid500.github.io/landing-page/
데스크톱 1440px 및 모바일 390px·320px에서 가로 넘침을 확인했습니다.

## v4 첨부 레퍼런스 팔레트
배경 #082B46, 포인트 #00D6B5로 통일했습니다. 강한 블루 그라데이션·도트·반짝임을 덜어내고 선물 뒤 민트빛을 적용했습니다. 기존 금액·문구·모션과 기능은 유지합니다. 모바일 390px와 데스크톱에서 화면을 확인했습니다.

## v5 하단 정렬과 장식
말풍선·아이콘·혜택 배지의 기울기를 제거했습니다. 상담 영역 도트와 대화 연결선, 폼 상단 민트 라인, 신청 단계 연결선과 아이콘 이중 테두리, FAQ 패널을 추가했습니다. 데스크톱·모바일의 정렬과 가로 넘침을 확인했습니다.

## v6 이모지와 선물 패키지 구성
상담·신청 절차·FAQ에 컬러 이모지를 사용하고 리본 장식과 부드러운 말풍선을 적용했습니다. 기존 문구·금액·기능을 유지합니다. 이모지 모양은 운영체제에 따라 조금씩 다릅니다. 데스크톱과 모바일 390px에서 가로 넘침을 확인했습니다.

## v7 하단 색감
메인 영역은 유지하고 상담 배경·버튼을 밝은 민트로, 답변 말풍선을 노랑으로 변경했습니다. 신청 절차에는 민트·노랑·하늘색을 적용했습니다. 모바일과 데스크톱 배치를 확인했습니다.

## v8 스크롤 애니메이션
상담·신청 절차·FAQ의 제목과 내용이 화면 진입 시 순서대로 나타납니다. 한 번만 재생하며 움직임 멈춤·동작 줄이기·키보드 포커스·IntersectionObserver 미지원 환경을 고려했습니다. 기본 상태에서는 콘텐츠가 보이고 애니메이션 준비가 완료된 경우에만 효과가 적용됩니다.
