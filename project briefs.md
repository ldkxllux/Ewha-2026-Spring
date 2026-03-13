# 2026 Spring 전체 프로젝트 리스트

| 팀번호 | 팀명 | 트랙 | 프로젝트명 |
|:------:|------|:----:|------------|
| [1](#team-1) | 이사장님 | 연구 | 기후·기상 데이터 환경에서 멀티모달 모델의 성능 향상을 위한 도메인 적응 기법 연구 |
| [2](#team-2) | Sudo | 산학 | HealthMate AI: 나만을 위한 AI 건강 비서 |
| [3](#team-3) | 할루캐쳐 | 연구 | Alltology |
| [5](#team-5) | 규교굥 | 산학 | 평범한 골동품 가게 운영 시뮬레이션에서 금지된 상자를 열며 공포 게임으로 전환되는 생성형 AI NPC 기반 게임 |
| [6](#team-6) | Greenfield | 산학 | 스토리 기반 관광 활성화 프로젝트 |
| [7](#team-7) | reverdir | 산학 | 게임형 독서 기록 서비스 |
| [8](#team-8) | 하면된다 | 산학 | Vintic |
| [9](#team-9) | Cloud9 | 산학 | 퀀트 전략 실시간 상태 모니터링 및 이상 징후 탐지 시스템 |
| [10](#team-10) | 212223 | 산학 | AI Tasker |
| [11](#team-11) | 알고리듬 |  |  |
| [12](#team-12) | 404 | 산학 | 여성 1인 여행자를 위한 세이프티 가이드 서비스 제공 시스템 |
| [13](#team-13) | Semicolone; | 산학 | AI 자서전 |
| [14](#team-14) | def | 연구 | Agent AI 추론을 위한 메모리 효율 최적화 |
| [15](#team-15) | 햄부기 | 연구 | Split-Computing Vision Inference System |
| [16](#team-16) | 퓨터 | 산학|  CharacterAI |
| [17](#team-17) | SPY | 산학 | AI 기반 음악 추천 어플리케이션 |
| [18](#team-18) | 디바트(deep-art) |  |  |
| [19](#team-19) | Logue |  |  |

---

<a id="team-1"></a>
## Team 1 이사장님

| 항목 | 내용 |
|------|------|
| 프로젝트명 | 기후·기상 데이터 환경에서 멀티모달 모델의 성능 향상을 위한 도메인 적응 기법 연구 |
| 트랙 | 연구 |
| 팀명 | 이사장님 |
| 팀구성 | 설영은, 신지민, 윤희서 |
| 팀지도교수 | 황의원 교수님 |
| 무엇을 만들고자 하는가 | 본 연구의 목표는 위성 이미지, 기상 관측 데이터, 수치예보 데이터 등 다양한 모달리티의 기상 데이터를 통합적으로 학습할 수 있는 멀티모달 도메인 적응 기반 날씨 예측 모델을 구축하는 것이다. 이를 통해 서로 다른 지역 및 데이터 수집 환경에서도 안정적으로 동작할 수 있는 domain generalization 능력을 갖춘 기상 예측 시스템을 개발하고자 한다. |
| 고객 (누구를 위해) | 본 연구는 기상 데이터 기반 예측 모델을 연구 및 개발하는 연구자와 기상 서비스 개발자를 주요 대상으로 하며, 궁극적으로는 정확하고 신뢰성 높은 날씨 예측 정보를 필요로 하는 일반 사용자 및 산업 분야에 기여하는 것을 목표로 한다. |
| Pain Point (해결할 문제) | 기상 데이터는 지역, 센서 장비, 관측 환경 등에 따라 데이터 분포가 상이하게 나타나는 특성을 가지며, 이러한 도메인 간 분포 차이는 학습된 모델이 새로운 환경에서 적용될 때 성능 저하를 유발하는 주요 원인이 된다. 특히 위성 영상, 기상 센서 데이터, 수치예보 데이터 등 서로 다른 모달리티를 활용하는 경우 데이터 간 표현 차이로 인해 모델의 일반화 성능이 제한되는 문제가 존재한다. 본 연구는 이러한 멀티모달 기상 데이터 환경에서 발생하는 도메인 불일치 문제를 해결하는 것을 목표로 한다. |
| 사용 기술 | 본 연구에서는 PyTorch 기반 딥러닝 프레임워크를 활용하여 multimodal representation learning을 수행하고, 도메인 간 분포 정렬을 위한 도메인 적응 기법을 적용하고자 한다. 또한 기상 데이터에 대해서는 LightGBM, XGBoost와 같은 트리 기반 ensemble 모델을 활용하여 베이스라인 모델을 구축하고, 딥러닝 기반 모델과의 성능 비교 및 하이브리드 모델 구조를 탐색한다. |
| 기대 효과 | 데이터 수집 환경이나 지역적 특성에 따른 도메인 차이에도 불구하고 안정적인 예측 성능을 확보할 수 있으며, 다양한 환경에서 활용 가능한 기상 예측 모델을 구축할 수 있다. 이는 기존 기상 예측 모델의 적용 범위를 확장하고, 실제 환경에서의 모델 신뢰도를 향상시키는 데 기여할 것으로 기대된다. |
| GitHub Repo | [https://github.com/chairwomans/chairwomans-capstone](https://github.com/chairwomans/chairwomans-capstone) |
| Team Ground Rule | [Team Ground Rule](https://github.com/chairwomans/chairwomans-capstone/blob/main/Team_Ground_Rule.md) |
| 최종수정일 | 2026-03-10 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-2"></a>
## Team 2 Sudo

| 항목 | 내용 |
|------|------|
| 프로젝트명 | HealthMate AI: 나만을 위한 AI 건강 비서 |
| 트랙 | 산학 |
| 팀명 | Sudo |
| 팀구성 | 최지수, 박서연, 신수빈 |
| 팀지도교수 |  |
| 무엇을 만들고자 하는가 | - 초개인화 건강 프로필 시스템: 키, 몸무게, 나이, 성별, 질환 정보(고혈압, 당뇨 등)를 기반으로 사용자 고유의 건강 프로필을 생성하고, 이를 바탕으로 식단과 운동 계획을 지속적으로 정밀 조정하는 AI 엔진.<br>- 이미지 스캔 기반 식단 기록기: 음식 사진을 촬영하면 AI가 자동으로 음식 종류를 인식하여 식단을 등록하고, 사용자의 선호도 피드백을 누적하여 추천 품질을 지속 개선.<br>- 맞춤 운동 코칭 기능: 사용자의 체력 수준과 운동 후 피드백(아픈 부위, 강도)을 반영하여 다음 운동 계획을 실시간으로 재조정하는 개인 트레이너 역할.<br>- 통합 건강 일정 관리: 병원 예약, 건강검진, 운동 일정을 하나의 앱에서 관리하고 알림을 제공하는 캘린더 기능. <br>- AI 챗봇 상담: 사용자의 기록된 건강 데이터를 기반으로 맥락을 이해한 맞춤형 건강 조언과 Q&A를 제공하는 대화형 AI 비서.<br>- 헬스 포인트 시스템: 식단 기록, 운동 목표 달성, 일정 수행 완료 시 포인트를 지급하고, 이를 프리미엄 AI 분석 기능 및 추가 서비스 이용권으로 교환하는 참여 보상 체계. |
| 고객 (누구를 위해) | - 바쁜 현대인 및 1인 가구: 식단·운동·병원 일정을 각각 다른 앱으로 관리해야 하는 불편함을 느끼며, 하나의 통합된 건강 관리 도구를 필요로 하는 사용자. <br>- 만성질환 보유자 및 건강 관리 입문자: 고혈압, 당뇨 등 특정 질환에 맞는 식단과 운동이 무엇인지 전문 지식 없이도 안전하게 안내받고 싶은 사용자. <br>- 건강에 관심은 있지만 지속하지 못하는 사람: 동기 부족으로 건강 관리 루틴을 꾸준히 유지하기 어려운 사용자로, 포인트 보상 등 게임 요소를 통해 참여를 이어갈 수 있는 동기를 필요로 하는 사람. |
| Pain Point (해결할 문제) | - 건강 관리 도구의 파편화: 식단 앱, 운동 앱, 병원 예약 앱 등이 분리되어 있어 통합적인 건강 관리가 어렵고 관리 피로도가 높은 문제를 하나의 앱으로 해결. <br>- 개인화 부재: 기존 건강 앱들은 일반적인 정보만 제공하고 사용자 개인의 질환·체력·선호도를 반영한 맞춤 추천이 이루어지지 않는 문제를 AI 기반 프로필 학습으로 해결. <br>- 지속 참여 동기 부족: 건강 관리가 의무처럼 느껴져 장기적인 루틴 형성에 실패하는 문제를, 포인트 적립 및 보상 시스템으로 습관 형성을 유도하여 해결. |
| 사용 기술 | - AI 추천 엔진 (LLM + 규칙 기반 필터링): 사용자의 건강 프로필과 누적 피드백 데이터를 결합하여 식단 및 운동을 추천하는 하이브리드 AI 모델로 개인화 정밀도를 높임.<br>- 이미지 인식 (Vision AI / YOLOv 계열): 음식 사진에서 식품 종류와 대략적인 양을 자동 감지하여 식단 기록 과정을 간소화하고 칼로리 등 영양소 정보와 연계.<br>- Framework: 고성능 백엔드(FastAPI 또는 Spring Boot)와 Flutter를 이용한 iOS·Android 크로스 플랫폼 앱 구축으로 접근성을 확보. <br>- Data: 공공데이터포털의 식품영양성분 DB 및 의료기관 정보 API를 연동하여 정확한 영양·의료 정보를 실시간 반영.<br>- 알림 시스템: FCM(Firebase Cloud Messaging)을 활용하여 운동·식단·병원 일정 알림을 적시에 푸시 발송. |
| 기대 효과 | - 건강 관리 습관의 내재화: 포인트 보상과 지속적인 맞춤 피드백으로 단기적 다짐이 아닌 장기적 건강 루틴으로 정착을 유도.<br>- 질환 예방 및 자기 인식 향상: 꾸준한 식단·운동 기록이 축적되면 사용자 스스로 생활 패턴의 문제를 인지하고 조기에 개선할 수 있는 환경 제공.<br>- 의료비 절감 잠재력: 예방 중심의 건강 관리 습관 형성으로 불필요한 병원 방문과 만성질환 악화를 줄여 개인 및 사회적 의료 비용 절감에 기여.<br>- 데이터 기반 서비스 고도화: 사용자 피드백 데이터가 누적될수록 추천 알고리즘이 정교해지고, 향후 스마트워치 연동·AI 건강 리포트 등 프리미엄 기능 확장의 기반이 됨. |
| GitHub Repo | [https://github.com/CSE-Sudo-26/sudo-capstone-project](https://github.com/CSE-Sudo-26/sudo-capstone-project) |
| Team Ground Rule | [Team Ground Rule](https://github.com/CSE-Sudo-26/sudo-capstone-project/blob/main/Team_Ground_Rule.md) |
| 최종수정일 | 2026-03-13 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-3"></a>
## Team 3 할루캐쳐

| 항목 | 내용 |
|------|------|
| 프로젝트명 | Alltology |
| 트랙 | 연구 |
| 팀명 | 할루캐쳐 |
| 팀구성 | 박세령, 이다영, 손현경 |
| 팀지도교수 | 황의원 교수님 |
| 무엇을 만들고자 하는가 | 기존 모델과 온톨로지가 탑재된 모델의 성능(정확도) 비교한 연구논문 |
| 고객 (누구를 위해) | LLM 모델의 답변 정확도 향상 |
| Pain Point (해결할 문제) | 할루시네이션을 비롯한 정확도 문제를 개선하기 위해서 |
| 사용 기술 | 온톨로지 |
| 기대 효과 | 미디어 분야의 LLM 모델의 답변 정확도 향상 (헐루시네이션 감소 효과) |
| GitHub Repo | [https://github.com/Ontology0/Graduation-Project](https://github.com/Ontology0/Graduation-Project) |
| Team Ground Rule |  [Team Ground Rule](https://github.com/ontology0/Graduation-Project/blob/main/Team_Ground_Rule.md) |
| 최종수정일 | 2026/03/11 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-5"></a>
## Team 5 규교굥

| 항목 | 내용 |
|------|------|
| 프로젝트명 | Do Not Open This Box. |
| 트랙 | 산학 |
| 팀명 | 규교굥 |
| 팀구성 | 정혜교, 윤민주, 박남규 |
| 팀지도교수 | 미정 |
| 무엇을 만들고자 하는가 | 판도라의 상자를 모티브로 한 3D 공포 게임. 주인공은 돌아가신 할머니가 운영하시던 골동품 가게를 물려받아 운영하게 된다. 플레이어는 손님에게 물건을 판매하고 가게를 청소하는 등 가게 운영 시뮬레이션을 즐길 수 있다. 하지만 가게에 있는 어떤 상자를 발견하고 나서부터 기이현상이 발생한다. |
| 고객 (누구를 위해) | 평소 PC를 이용해 공포, 시뮬레이션 등의 게임을 즐겨하는 사람들과 영상 플랫폼을 이용해 이러한 게임들과 관련된 콘텐츠를 즐기는 사람들. |
| Pain Point (해결할 문제) | 기존의 '8번 출구'나 '발디의 수학교실'과 같은 심리적인 공포의 재미를 유지하되, 플레이어가 NPC와 선택지로만 대화하는 것이 아닌, AI NPC인 손님과 타이핑으로 대화하며 플레이어가 실제 그 상황에 몰입하고 더 극대화된 공포를 느낄 수 있도록 하는 것이 목표이다. |
| 사용 기술 | 유니티, 생성형 AI |
| 기대 효과 | 플레이어는 다양한 방식으로 심리적 공포를 느낄 수 있다. 게임의 배경이나 분위기, 기이한 현상, 손님들의 기괴한 대사를 통해 점진적으로 공포를 느낄 수 있고, 그 공포가 극에 달했을 때 주인공의 숨겨진 이야기를 통해 반전을 경험할 수 있다. |
| GitHub Repo | [https://github.com/muffinhead03/Start2026_1](https://github.com/muffinhead03/Start2026_1) |
| Team Ground Rule | https://github.com/muffinhead03/Start2026_1/blob/main/Team_Ground_Rule.md |
| 최종수정일 | 2026.03.10 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-6"></a>
## Team 6 Greenfield

| 항목 | 내용 |
|------|------|
| 프로젝트명 | 스토리 기반 관광 활성화 프로젝트 |
| 트랙 | 산학 |
| 팀명 | Greenfield |
| 팀구성 | 최준희, 권은재, 김재희 |
| 팀지도교수 |  |
| 무엇을 만들고자 하는가 | 스토리 콘텐츠 제공, 스토리 기반 장소 관광, 다국어 콘텐츠 |
| 고객 (누구를 위해) | 한국 문화를 경험하고 싶은 외국인 관광객<br>역사 기반 여행을 원하는 국내 관광객<br>역사와 문화 콘텐츠에 관심 있는 사용자 |
| Pain Point (해결할 문제) | - 관광지의 스토리 전달 부족<br>- 역사 정보를 흥미롭게 전달하는 방식 부족<br>- 외국인 관광객의 한국 역사 이해 및 관광 접근성 부족<br>- 학생들이 실제 역사 장소를 체험하며 학습할 기회 부족<br><br>스토리를 중심으로 역사 장소를 연결하여 외국인과 학생 모두가 한국 역사를 쉽게 이해하고 직접 체험할 수 있는 몰입형 문화관광 경험을 제공하는 것을 목표 |
| 사용 기술 | **프론트엔드**<br><br>- React.js, 영상 및 이미지 콘텐츠 UI 구성<br><br>**백엔드**<br><br>- Node.js , MySQL<br><br>**데이터 수집**<br><br>- 관광지 텍스트 데이터 분석, 역사 관련 이미지 및 영상<br><br>**AI 및 추천 시스템**<br><br>- 스토리 기반 관광 코스 추천 알고리즘, LLM 기반 역사 요약 및 다국어 번역 |
| 기대 효과 | 스토리 기반 접근을 통해 외국인과 국내 사용자 모두가 한국 역사를 쉽게 이해하고 실제 역사 장소를 체험하도록 유도하여 문화관광 참여도와 관광 활성화를 동시에 높이기 |
| GitHub Repo | [https://github.com/greenfield-2026-capstone/greenfield-project](https://github.com/greenfield-2026-capstone/greenfield-project) |
| Team Ground Rule | https://github.com/greenfield-2026-capstone/greenfield-project/blob/main/Team_Ground_Rule.md |
| 최종수정일 | 2026.3.10 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-7"></a>
## Team 7 reverdir

| 항목 | 내용 |
|------|------|
| 프로젝트명 | 게임형 독서 기록 서비스 |
| 트랙 | 산학 |
| 팀명 | reverdir |
| 팀구성 | 전채연, Lyu, Dongying, 이은효 |
| 팀지도교수 | 미정 |
| 무엇을 만들고자 하는가 | 사람들이 독서에 재미를 붙일 수 있게 하는 기록용 어플 |
| 고객 (누구를 위해) | 독서를 재미있게 습관화하고 싶은 사람을 위해 |
| Pain Point (해결할 문제) | 기존의 독서 앱 기록 과정의 단조로움. 번거로운 기록 과정 |
| 사용 기술 | Front (React) / Back (Spring Boot) |
| 기대 효과 | 게임 요소를 통한 재미있는 독서 경험을 제공하고, 기록 관리 편의성을 증진함 |
| GitHub Repo | [https://github.com/team-capstone-reverdir-2026/reverdir_repo](https://github.com/team-capstone-reverdir-2026/reverdir_repo) |
| Team Ground Rule | https://github.com/eunhyo019/reverdir_repo/blob/main/Team_Ground_Rule.md |
| 최종수정일 |  |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-8"></a>
## Team 8 하면된다

| 항목 | 내용 |
|------|------|
| 프로젝트명 | Vintic |
| 트랙 | 산학 |
| 팀명 | 하면된다 |
| 팀구성 | 김수연, 이예주, 조채윤 |
| 팀지도교수 | 오세은 교수님 |
| 무엇을 만들고자 하는가 | AI 기반 가격 검증과 정시 경매 시스템으로 정보 비대칭과 탐색 피로를 해결하는 빈티지 거래 플랫폼 |
| 고객 (누구를 위해) | 빈티지 거래 플랫폼 이용자 |
| Pain Point (해결할 문제) | (1) 가격 정보의 불균형: 판매자가 상품 가격을 임의로 책정하는 경우가 많아, 구매자가 적정 가격을 판단하기 어려운 구조</br>(2) 구매자의 탐색 피로: 원하는 매물의 업로드 시점을 알기 어려워, 사용자가 플랫폼에 반복적으로 접속하며 무한 스크롤링을 지속하는 문제</br>(3) 판매글 노출의 비효율: 게시글이 업로드 시점에 따라 쉽게 묻혀, 판매자가 동일한 글을 반복 업로드해야 하는 비효율 |
| 사용 기술 | Vision AI(FastAPI+상용 API), Spring, React 등 |
| 기대 효과 | (1) 상품별 AI 측정가와 판매자 희망가 병기를 통한 가격 판단 기준 제공</br>(2) AI 측정가와 희망가 차이 제한을 통한 가격 신뢰도 향상</br>(3) 특정 시각 일괄 경매 방식을 통한 구매자 탐색 피로 완화 및 판매자 노출 기회의 공정성 확보 |
| GitHub Repo | [https://github.com/hamyeon/Team-Hamyeon](https://github.com/hamyeon/Team-Hamyeon) |
| Team Ground Rule | [Team Grouond Rule](https://github.com/hamyeon/Team-Hamyeon/blob/main/Team_Ground_Rule.md) |
| 최종수정일 | 2026.03.12 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-9"></a>
## Team 9 Cloud9

| 항목 | 내용 |
|------|------|
| 프로젝트명 | 퀀트 전략 상태 모니터링 및 이상 징후 탐지 시스템 |
| 트랙 | 산학 |
| 팀명 | Cloud9 |
| 팀구성 | 박나림, 임도경, 최은우 |
| 팀지도교수 | 컨택중 |
| 무엇을 만들고자 하는가 | 퀀트 전략 실시간 상태 모니터링 및 이상 징후 탐지 시스템 |
| 고객 (누구를 위해) | 개인 자동매매 투자자 |
| Pain Point (해결할 문제) | 여러 퀀트 전략을 동시에 운용할 경우, 이상 상황이 발생했을 때 어떤 전략에서 문제가 생겼는지 빠르게 확인하기 어렵다는 문제가 있다. 본 프로젝트는 전략별 상태를 실시간으로 모니터링하고 이상 징후를 탐지하여, 이를 대시보드로 시각화해 효율적인 대응을 가능하게 한다. |
| 사용 기술 | Front(React, Recharts, WebSocket client), Back(Python, FastAPI, SQLAlchemy, WebSocket), AI(Pandas, NumPy)  |
| 기대 효과 | 손실 최소화 |
| GitHub Repo | [https://github.com/Cloud9-capstone-2026](https://github.com/Cloud9-capstone-2026) |
| Team Ground Rule | [Team Ground Rule](https://github.com/Cloud9-capstone-2026/cloud9/blob/main/Team_Ground_Rule.md) |
| 최종수정일 | 2026.03.12 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-10"></a>
## Team 10 212223

| 항목 | 내용 |
|------|------|
| 프로젝트명 | AI Tasker |
| 트랙 | 산학 |
| 팀명 | 212223 |
| 팀구성 | 고윤진(2176018), 김나현(2276040), 이유진(2376218) |
| 팀지도교수 | 심재형 교수님 |
| 무엇을 만들고자 하는가 | 사용자가 프롬프트를 입력하면 각 AI 모델(GPT-4, Gemini, Claude 등)의 최적화된 프롬프트를 추천 후 그에 따른 예상 비용을 실시간으로 계산하고 비교하는 웹 서비스 |
| 고객 (누구를 위해) | Ai api를 사용하는 학생 및 개발자, 스타트업 등 비용에 민감한 사용자 |
| Pain Point (해결할 문제) | AI 프롬프트 작성 미숙으로 인한 과다한 비용 청구 |
| 사용 기술 | Tailwind, Next.js, FastAPI, tiktoken,LangChain,LLMLingua,Firebase Firestore |
| 기대 효과 | AI 사용성 계선 및 비용 감소 |
| GitHub Repo | [https://github.com/0727n1122-beep/graduationproject/tree/main](https://github.com/0727n1122-beep/graduationproject/tree/main) |
| Team Ground Rule | [Team Ground Rule](https://github.com/0727n1122-beep/graduationproject/blob/main/Team_Ground_Rule.md) |
| 최종수정일 | 03.12 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-11"></a>
## Team 11 알고리듬

| 항목 | 내용 |
|------|------|
| 프로젝트명 | SpeedSchedule: AI 기반 인력 운영 최적화를 위한 지능형 스케줄링 및 시프트 관리 웹 플랫폼 |
| 트랙 | 산학 |
| 팀명 | 알고리듬 |
| 팀구성 | PM / 조상은 / 컴퓨터공학과 / 2376273 <br> FE&Design / 정지유 / 국제사무학과 / 2416023 <br> BE&AI / 이시은 / 컴퓨터공학과 / 2466044 |
| 팀지도교수 | Contacting ...  |
| 무엇을 만들고자 하는가 | AI 기반 인력 운영 최적화를 위한 지능형 스케줄링 및 시프트 관리 웹 플랫폼.<br>교내의 복잡한 수업 시간표와 감독 배정 업무를 데이터 기반으로 자동화하며, 실시간 수정이 가능한 인터렉티브 캘린더와 결원 발생기 대리 근무자를 매칭해주는 기능까지 통합된 관리 솔루션. |
| 고객 (누구를 위해) | 학교 현장의 행정 관리자와 교사 |
| Pain Point (해결할 문제) | 기존 시스템은 AI 최적화가 없는 단순 알고리즘이라 교사 개개인의 선호도나 숙련도 반영이 불가능함. 이로 인해 관리자가 엑셀로 2차 수동 수정을 거치는 등 행정력이 낭비됨. <br> 또한 가나다순/ 고정 순번제 배정은 특정 인원에게 업무가 쏠리는 불균형을 초래하여 조직 내 공정성 시비와 만족도 저하를 일으킴. |
| 사용 기술 | AI : 딥러닝 기반 스케줄 최적화 알고리즘 (PyTorch / TensorFlow) <br> FE : React, Vite, Axios, Vercel, ESLint <br> BE : SpringBoot 3, MySQL, Hibernate(JPA), Docker, Gradle <br> DevOps : Docker, GitHub Action <br> Infra : AWS EC2 (Amazon Linux), AWS RDS
| 기대 효과 | 스케줄링 업무 자동화를 통한 행정 비용 절감 및 운영 효율성 극대화. <br> 데이터 기반의 객관적 배정 시스템을 통한 운영의 투명성 확보. <br> 교사 업무 만족도 향상 및 조직 내 인력 운영 효율성 극대화.  |
| GitHub Repo | [https://github.com/speedSchedule/AlgoRhythm.git](https://github.com/speedSchedule/AlgoRhythm.git) |
| Team Ground Rule | https://github.com/speedSchedule/AlgoRhythm/blob/main/Team_Ground_Rule.md |
| 최종수정일 | 2025/03/10 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-12"></a>
## Team 12 404

| 항목 | 내용 |
|------|------|
| 프로젝트명 | 여성 1인 여행자를 위한 세이프티 가이드 서비스 제공 시스템 |
| 트랙 | 산학 |
| 팀명 | 404 |
| 팀구성 | 이아림, 노유나, 이채원  |
| 팀지도교수 |  |
| 무엇을 만들고자 하는가 | 여성 혼자 여행하는 사람들을 위한 안전 중심 여행 플랫폼을 개발하고자 한다. 여성 사용자들이 직접 작성한 안전 리뷰 데이터를 기반으로 여행지의 안전도를 지도에 표시하고, 이를 활용해 안전한 여행 경로와 맛집 및 관광 코스를 추천한다. 또한 같은 지역을 여행하는 여성들 간 동행 매칭 기능을 제공하여 안전하고 편안한 여행 환경을 만드는 것을 목표로 한다. |
| 고객 (누구를 위해) | 20대 초반 여성교환 학생, 사회초년생 여성 직장인(20대 중후반) |
| Pain Point (해결할 문제) | 여성의 안전 정보 부족과 혼자 여행할 때의 불안감 |
| 사용 기술 | 프론트엔드 웹 개발 기술, 백엔드 서버 및 데이터베이스 기술을 기반으로 구현하며, 사용자 리뷰 데이터를 분석하여 여행지 안전도를 평가하고 여행 코스를 추천하기 위한 AI 기반 데이터 분석 기술을 활용한다. |
| 기대 효과 | 여성 1인 여행자가 안전하고 효율적으로 여행을 계획할 수 있고, 여성의 이동권과 안전권을 기술적으로 보장한다. |
| GitHub Repo | [https://github.com/capstone-team404](https://github.com/capstone-team404) |
| Team Ground Rule | [https://github.com/iinge/Ewha-2026-Spring/blob/main/Team_Ground_Rule.md |
| 최종수정일 | 26.03.11 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---
<a id="team-13"></a>
## Team 13 Semicolone;

| 항목 | 내용 |
|------|------|
| 프로젝트명 | 자서전 |
| 트랙 | 산학 |
| 팀명 | Semicolone; |
| 팀구성 | 신지원, 이채원, 윤현진 |
| 팀지도교수 |  |
| 무엇을 만들고자 하는가 | 본 서비스는 사용자가 남긴 일상 기록 데이터를 AI가 분석하여 개인의 삶을 정리하고 자서전 형태로 생성하는 AI 기반 라이프 로그 플랫폼이다. 사용자는 매일 간단한 기록만 남기면 되고, AI는 이를 분석하여 감정 변화, 삶의 패턴, 주요 사건, 인간관계 변화 등을 추적한다. 이렇게 축적된 데이터를 기반으로 AI는 사용자의 삶을 하나의 이야기 구조로 정리하고 디지털 자서전 형태의 콘텐츠를 생성한다. 또한 사용자는 단순히 기록을 남기는 것을 넘어 자신의 감정 패턴, 생활 패턴, 관심사 변화 등을 데이터 기반으로 분석하여 확인할 수 있으며, 자신의 삶을 통계와 스토리 형태로 돌아보는 경험을 할 수 있다. |
| 고객 (누구를 위해) | 본 서비스의 주요 고객은 자신의 삶을 기록하고 돌아보고 싶어하는 사람들이다. 특히 자기 성찰과 기록에 관심이 있는 대학생 및 20대, 일기나 기록을 남기고 싶지만 꾸준히 지속하지 못하는 사람들, 자신의 감정 변화나 삶의 패턴을 분석적으로 이해하고 싶은 사용자들이 주요 타겟이 된다. 또한 개인의 경험과 기록을 의미 있는 콘텐츠로 남기고 싶은 사람들에게도 유용한 서비스가 될 수 있다. |
| Pain Point (해결할 문제) | 많은 사람들이 자신의 삶을 기록하고 싶어 하지만 실제로는 꾸준히 기록을 유지하기 어렵다. 일기를 쓰더라도 시간이 지나면 다시 읽지 않는 경우가 많고, 단순 기록 형태로 남기 때문에 자신의 삶을 객관적으로 분석하거나 의미 있게 정리하기 어렵다. 또한 사람들은 자신의 감정 변화나 삶의 패턴을 데이터 관점에서 이해할 기회를 거의 가지지 못한다. 결과적으로 개인의 경험과 감정은 단편적인 기록으로 남거나 시간이 지나면서 잊혀지는 경우가 많다. |
| 사용 기술 | 본 서비스는 자연어 처리 기반 감정 분석 기술을 활용하여 사용자의 기록 데이터를 분석한다. 또한 텍스트 데이터 패턴 분석을 통해 반복되는 주제와 주요 사건을 추출하고 키워드 분석을 통해 사용자 삶의 주요 관심사를 파악한다. 이후 스토리 생성 모델을 활용하여 기록 데이터를 하나의 이야기 구조로 정리하여 자서전 형태의 콘텐츠를 생성한다. 이러한 기술을 통해 단순한 기록 데이터를 개인의 삶을 해석하는 콘텐츠로 변환할 수 있다. |
| 기대 효과 | 본 서비스를 통해 사용자는 자신의 삶을 꾸준히 기록하고 돌아볼 수 있으며 자신의 감정 변화와 경험을 데이터 기반으로 분석할 수 있다. 또한 개인의 일상 기록이 단순한 데이터로 남는 것이 아니라 하나의 이야기 형태의 콘텐츠로 정리되어 보존된다. 이를 통해 사용자는 자신의 삶을 더 깊이 이해할 수 있고 시간이 지나도 자신의 경험과 기억을 의미 있게 돌아볼 수 있게 된다. |
| GitHub Repo | [https://github.com/Semicolone](https://github.com/Semicolone) |
| Team Ground Rule | [https://github.com/Semicolone/start/blob/main/Team_Ground_Rule.md](https://github.com/Semicolone/start/blob/main/Team_Ground_Rule.md) |
| 최종수정일 | 2026.03.11. |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---



<a id="team-14"></a>
## Team 14 def

| 항목 | 내용 |
|------|------|
| 프로젝트명 |  |
| 트랙 | 연구 |
| 팀명 | def |
| 팀구성 | 서혜원, 신은서, 이재린 |
| 팀지도교수 | 심재형 교수님 |
| 무엇을 만들고자 하는가 | - 로컬 워크로드를 분석하고 병목을 스스로 해결하는 에이전트 기반 최적화 프레임워크 설계 및 구현<br>- Experimental Evaluation (논문 핵심): 최적화 적용 전/후의 성능(TPS, Latency, Energy Efficiency) 비교 데이터와 다양한 워크로드 시나리오(단일 추론 vs 멀티태스킹)에서의 자원 효율성 검증 보고서 |
| 고객 (누구를 위해) | - Agent AI 시스템 설계자 및 연구자: 클라우드 의존도를 낮추고 로컬 기기(Edge Device)의 하드웨어 잠재력을 끝까지 끌어올려야 하는 엔지니어<br>- Agent AI 사용자: 외부 클라우드 서버에 데이터를 보내지 않고, Mac mini 같은 로컬 기기에서 개인화된 AI 모델을 안전하게 돌리고 싶은 개인 및 기업 |
| Pain Point (해결할 문제) | - 리소스 고갈:LLM(거대언어모델) 실행 시 메모리 점유율이 급증하여 시스템이 멈추거나 느려지는 현상<br>- 예측 불가능한 병목(Dynamic Bottleneck):워크로드의 성격(연산 중심 vs 메모리 중심)에 따라 시스템의 어느 부분에서 병목이 생길지 실시간으로 파악하기 어려움<br>- 메모리 고갈(Memory Issue):특히 LLM 구동 시 제한된 통합 메모리(Unified Memory) 용량을 초과할 때 생기는 다양한 문제점 |
| 사용 기술 | - Agentic Monitoring Loop : 에이전트가 시스템 API를 통해 CPU/GPU 등 점유율 및 전력 소모량을 실시간 관찰하고 대응 전략을 결정<br>- 현재 실행 중인 워크로드에 대한 실시간으로 분류하는 분석 알고리즘 |
| 기대 효과 | - 효율성 극대화:동일 하드웨어 대비 AI 추론 성능(Throughput) 및 응답 속도(Latency)의 유의미한 향상.<br>- 시스템 안정성:메모리 이슈로 인한 시스템 다운 방지 및 멀티태스킹 환경에서의 부드러운 사용자 경험 유지.<br>- 에너지 효율: 불필요한 연산 낭비를 줄여 전력 소모 최적화 및 발열 제어 |
| GitHub Repo | [https://github.com/capstone-2026-ewha/def](https://github.com/capstone-2026-ewha/def) |
| Team Ground Rule | [https://github.com/capstone-2026-ewha/def/blob/main/Team_Ground_Rule.md](https://github.com/capstone-2026-ewha/def/blob/main/Team_Ground_Rule.md) |
| 최종수정일 | 2026-3-11 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-15"></a>
## Team 15 햄부기

| 항목 | 내용 |
|------|------|
| 프로젝트명 | Split-Computing Vision Inference System |
| 트랙 | 연구 |
| 팀명 | 햄부기 |
| 팀구성 | 신성현, 송영채, 장수연 |
| 팀지도교수 | 심재형 |
| 무엇을 만들고자 하는가 | 엣지 장치와 클라우드 서버가 협력하여 이미지를 빠르게 분석하는 분산 AI 추론 시스템 |
| 고객 (누구를 위해) | AI 기반 서비스를 개발하는 학생 팀 및 연구 프로젝트 수행자를 위해 |
| Pain Point (해결할 문제) | 엣지 장치에서 AI 모델을 실행할 때 발생하는 높은 연산 부담과 네트워크 지연 문제를 해결하기 위해 |
| 사용 기술 | Computer Vision 모델과 Edge–Cloud Split Inference 기술을 사용하여 일부 연산은 엣지에서, 나머지는 클라우드에서 처리하는 방식 사용 |
| 기대 효과 | AI 추론 속도를 개선하고 네트워크 사용량을 줄이며, 제한된 연산 자원을 가진 장치에서도 효율적인 AI 서비스가 가능해진다 |
| GitHub Repo | [https://github.com/Ewha-Capstone-Project/Hambugy.git](https://github.com/Ewha-Capstone-Project/Hambugy.git) |
| Team Ground Rule | [https://github.com/Ewha-Capstone-Project/Hambugy/blob/main/Team_Ground_Rule.md](https://github.com/Ewha-Capstone-Project/Hambugy/blob/main/Team_Ground_Rule.md) |
| 최종수정일 | 26/03/10 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-16"></a>
## Team 16 퓨터

| 항목 | 내용 |
|------|------|
| 프로젝트명 | CharacterAI  |
| 트랙 | 산학 |
| 팀명 | 퓨터 |
| 팀구성 | 김민주, 백은혜, 이찬희, 최윤서  |
| 팀지도교수 | 심재형 |
| 무엇을 만들고자 하는가 | 사용자와 대화할수록 성격이 변화하는 AI 캐릭터 기반 영어 회화 학습 서비스 |
| 고객 (누구를 위해) | 영어 회화를 재미있게 꾸준히 학습하고 싶은 10~20대 사용자 |
| Pain Point (해결할 문제) | 기존 영어 학습 앱은 고정된 응답으로 흥미가 금방 떨어지고 지속 사용이 어려움 |
| 사용 기술 | LLM API, RAG (벡터 DB), Reddit/YouTube API, Rive 애니메이션, Next.js, FastAPI |
| 기대 효과 | 캐릭터와의 정서적 유대감 형성으로 학습 지속률 향상, 최신 슬랭 기반 실용 영어 습득 |
| GitHub Repo | [https://github.com/puter8/capstone](https://github.com/puter8/capstone) |
| Team Ground Rule | https://github.com/puter8/Ewha-2026-Spring/blob/main/Team_Ground_Rule.md |
| 최종수정일 | 2026.03.12 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-17"></a>
## Team 17 SPY

| 항목 | 내용 |
|------|------|
| 프로젝트명 | AI 기반 음악 추천 어플리케이션 |
| 트랙 | 산학 |
| 팀명 | SPY |
| 팀구성 | 신희조, 윤수연, 박은수 |
| 팀지도교수 |  |
| 무엇을 만들고자 하는가 | 기분이나 감정이나 취향을 넣으면 음악을 추천해주는 어플 |
| 고객 (누구를 위해) | 음악을 좋아하는 사람 |
| Pain Point (해결할 문제) | 듣고 싶은 음악만 듣게 됨 |
| 사용 기술 | Spotify Web API (곡 정보)<br>OpenAI API (추천 이유 생성)<br>YouTube Data API (뮤직 영상) |
| 기대 효과 | 듣지 못했던 음악을 들을 수 있음, 듣고 싶은 음악을 찾아다니는 번거로움을 해소할 수 있음 |
| GitHub Repo | [https://github.com/SPY-capstone-2026/SPY-capstoneREPO](https://github.com/SPY-capstone-2026/SPY-capstoneREPO) |
| Team Ground Rule | https://github.com/SPY-capstone-2026/SPY-capstoneREPO/blob/main/Team_Ground_Rule.md |
| 최종수정일 | 2026.03.11 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-18"></a>
## Team 18 디바트(deep-art)

| 항목 | 내용 |
|------|------|
| 프로젝트명 | AI 기반 오디오 도슨트 자동 제작 서비스 |
| 트랙 | 연구 |
| 팀명 | 디바트(deep-art) |
| 팀구성 | 최현서, 이나겸, 김나경 |
| 팀지도교수 |  |
| 무엇을 만들고자 하는가 | 전시 정보를 입력하면 AI가 도슨트 설명을 생성하고 음성으로 변환해주는 AI 기반 오디오 도슨트 자동 제작 서비스 |
| 고객 (누구를 위해) | 전시 기획자 및 전시 콘텐츠 제작자 |
| Pain Point (해결할 문제) | 전시에서 활용되는 오디오 도슨트는 제작에 시간과 비용이 많이 들기 때문에, 소규모 전시나 개인 전시에서는 제작이 어려운 경우가 많다. 이러한 문제를 해결하기 위해 오디오 도슨트를 간편하게 제작할 수 있는 방법을 제공하고자 한다. |
| 사용 기술 | LLM 기반 콘텐츠 생성, RAG 기반 전시 정보 활용, 음성 합성(TTS) 기술 |
| 기대 효과 | 전시 기획자가 전시 주제, 전시물 설명, 요청 사항 등을 입력하면 AI가 도슨트 설명을 생성하고 이를 음성으로 변환하여 오디오 도슨트로 활용 가능한 음성 파일을 자동으로 제작할 수 있다. 이를 통해 오디오 도슨트 제작 비용과 시간을 크게 줄이고, 더 많은 전시에서 오디오 도슨트를 활용할 수 있다. |
| GitHub Repo | [https://github.com/ewha-deep-art/deep-art](https://github.com/ewha-deep-art/deep-art) |
| Team Ground Rule | [https://github.com/ewha-deep-art/deep-art/blob/main/Team_Ground_Rule.md](https://github.com/ewha-deep-art/deep-art/blob/main/Team_Ground_Rule.md) |
| 최종수정일 | 2026.03.10 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-19"></a>
## Team 19 Logue

| 항목 | 내용 |
|------|------|
| 프로젝트명 |  |
| 트랙 |  |
| 팀명 | Logue |
| 팀구성 |  |
| 팀지도교수 |  |
| 무엇을 만들고자 하는가 | 자연어 질문만으로 데이터베이스에서 필요한 정보를 조회할 수 있는 데이터 분석 인터페이스 |
| 고객 (누구를 위해) | 데이터 기반 의사결정을 해야 하지만 SQL이나 데이터 조회가 어려운 기획자·마케터 |
| Pain Point (해결할 문제) | 비즈니스 데이터를 확인할 때 개발자에게 쿼리를 요청해야 하는 의존성과 분석 지연 문제를 해결 |
| 사용 기술 | LLM 기반 Text-to-SQL, 데이터베이스 스키마 이해, 자연어 질의 처리 기술을 사용 |
| 기대 효과 | 비개발자도 즉시 데이터를 탐색하고 빠르게 의사결정을 내릴 수 있게 됨. |
| GitHub Repo | [https://github.com/26-ewha-capstone-logue](https://github.com/26-ewha-capstone-logue) |
| Team Ground Rule |  |
| 최종수정일 |  |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---
