# 2026 Spring 전체 프로젝트 리스트 

| 팀번호 | 팀명 | 트랙 | 프로젝트명 |
|:------:|------|:----:|------------|
| [1](#team-1) | 이사장님 | 연구 | 테스트 이미지의 도메인을 자동으로 파악해 텍스트와 이미지 임베딩을 동적으로 재조합함으로써 도메인 변화에도 정확한 CLIP 기반 Zero-Shot 이미지 분류 연구 |
| [2](#team-2) | Sudo | 산학 | HealthMate AI: 불규칙한 생활 속 2030을 위한 고혈압·당뇨 위험군 대상 식단 인식·코칭 통합 헬스케어 플랫폼 |
| [3](#team-3) | Alltology | 연구 | 검색 결과와 내부 지식이 충돌할 때: Preference Learning(DPO+LoRA) 기반 RAG Knowledge Conflict 해결 연구 |
| [5](#team-5) | 규교굥 | 산학 | On-device 로컬 LLM 기술을 사용하여 플레이어 맞춤형 힌트를 실시간으로 제공하는 1인칭 3D 공포 방탈출 게임 |
| [6](#team-6) | Greenfield | 산학 | 	AI 역사 인물 인터랙션과 다국어 스토리 콘텐츠 기반 역사 관광 활성화 웹 플랫폼 |
| [7](#team-7) | reverdir | 산학 | 익명 매칭, 질문, 미션, 쪽지 상호작용을 통해 사람들 사이의 자연스러운 관계 형성과 친밀감 형성을 돕는 마니또 기반 소셜 게임 플랫폼 |
| [8](#team-8) | 하면된다 | 산학 | AI 기반 가격 검증과 정시 경매 시스템으로 정보 비대칭과 탐색 피로를 해결하는 빈티지 거래 플랫폼 |
| [9](#team-9) | Cloud9 | 산학 | 반복적인 손실을 겪는 개인 주식 투자자를 위한 AI 기반 매매 행동 분석 및 맞춤형 투자 습관 개선 플랫폼 |
| [10](#team-10) | 212223 | 산학 | 프롬프트 자동 최적화 기반 LLM API 비용 실시간 비교 웹 서비스 |
| [11](#team-11) | 알고리듬 | 산학 |  SpeedSchedule: 인력 운영 최적화를 위한 AI 스케줄링 및 시간표 관리 웹 플랫폼 |
| [12](#team-12) | 404 | 산학 | 여성 1인 여행자를 위해, AI 기반 안전 분석으로 정보 공백을 해결하고 안전 경로를 추천하는 지도 서비스 |
| [13](#team-13) | Semicolone; | 산학 | AI 질문을 ‘기억되는 인사이트’로 바꿔주는 개인 지식 관리 플랫폼 |
| [14](#team-14) | def | 연구 | 코딩 에이전트를 위한 AST 기반 kv 재사용 추론 최적화 |
| [15](#team-15) | 햄부기 | 연구 | 엣지 디바이스 배포를 위한 Vision Foundation Model의 2:4 구조적 희소성 성능 분석 및 추론 파이프라인 구축 |
| [16](#team-16) | 퓨터 | 산학 | 대화 진행에 따라 성격이 변하는 AI 캐릭터와의 정서적 유대감 기반 영어 회화 학습 지속 서비스 |
| [17](#team-17) | SPY | 산학 | Moni: AI 기반 소비 예측과 맞춤형 챌린지를 결합한 개인화 소비 코칭 서비스 |
| [18](#team-18) | 디바트(deep-art) | 연구 | 철새 이동 경로 예측 모델과 설명 가능한 AI(XAI)를 사용하여 전시 관람객에게 AI의 추론 과정에 대한 시각적 경험을 제공하는 인터랙티브 미디어아트 설치 작품 |
| [19](#team-19) | Logue | 산학 | 자연어 기반 데이터 분석 질의를 통해 조직의 데이터 접근성과 의사결정 속도를 향상시키는 AI 기반 데이터 분석 웹 인터페이스, Logue |

---

<a id="team-1"></a>
## Team 1 이사장님

| 항목 | 내용 |
| --- | --- |
| 프로젝트명 | 테스트 이미지의 도메인을 자동으로 파악해 텍스트와 이미지 임베딩을 동적으로 재조합함으로써 도메인 변화에도 정확한 CLIP 기반 Zero-Shot 이미지 분류 연구 |
| 서비스명(브랜드) | DoFit |
| 트랙 | 연구 |
| 팀명 | 이사장님 |
| 팀구성 | 설영은, 신지민, 윤희서 |
| 팀지도교수 | 황의원 교수님 |
| 무엇을 만들고자 하는가 | CLIP(Contrastive Language–Image Pre-training)은 이미지와 텍스트를 함께 이해하는 멀티모달 AI 모델이다. 그런데 기존 방식은 스케치든 실사든 항상 똑같은 고정 클래스 대표 벡터로 비교하기 때문에, 테스트 이미지의 도메인이 학습 분포와 달라지는 순간(domain shift) 이미지-텍스트 정렬이 어긋나 분류 성능이 급락한다.<br><br>이를 해결하기 위해, 테스트 이미지가 들어오는 순간 **추가 학습 없이** 다음 세 단계를 수행하는 Test-Time Domain Adaptation 시스템을 만들고자 한다.<br><br>1. **MTA**: 원본 이미지 1장으로부터 Stable Diffusion V2(63장) + RandomCrop(64장) = 총 128장의 augmented view를 생성하고, MeanShift 기반 MTA로 outlier를 자동 제거하여 robust한 이미지 임베딩 'm*'을 획득한다.<br>2. **도메인 자동 추정**: m*와 도메인 프롬프트 임베딩 간 코사인 유사도를 계산하고, 도메인별 가중치를 확률적으로 추정한다.<br>3. **동적 임베딩 재조합**: 추정된 도메인 가중치를 **텍스트 임베딩**(클래스 템플릿 가중 평균)과 **이미지 임베딩**(Linear Projection 후 도메인 hint token 삽입)에 동시에 적용해 해당 도메인에 최적화된 비교 기준을 실시간으로 생성한다. |
| 고객 (누구를 위해) | 스케치, 회화, 위성사진, 의료 이미지처럼 학습 데이터와 도메인이 다른(domain shift가 발생하는) 이미지를 분류해야 하는데, 매번 새로 fine-tuning하기엔 데이터도 없고 비용도 부담스러운 연구자 및 ML 엔지니어<br><br>예상 타겟:<br>• 의료 AI: 기기·병원마다 영상 스타일이 달라 재학습 부담 → 재학습 없이 변화에 즉시 대응, 진단 분류 정확도 유지<br>• 자율주행: 날씨·시간대 변화에 지속 대응 필요 → 실시간 Domain Shift 대응, 운행 정확도 확보<br>• 스마트팩토리: 조명·카메라 교체 시마다 재학습 비용 발생 → 교체 시 발생하는 재학습 비용 제거, 즉시 투입 가능<br>• 게임/콘텐츠: 실사/카툰/픽셀 등 다양한 아트 스타일 혼재 → 혼재된 아트 스타일 자동 분류, 라벨링 비용 절감 |
| Pain Point (해결할 문제) | 멀티모달 데이터는 도메인 차이(domain shift)가 발생하면 테스트 성능이 크게 저하된다. 특히 CLIP과 같은 Vision-Language Model(VLM)은 Zero-Shot downstream task 환경에서 학습 도메인과 테스트 도메인이 달라지는 순간 이미지-텍스트 간 정렬이 어긋나 분류 성능이 떨어진다. 기존의 멀티모달 도메인 적응(domain adaptation) 방식은 추가 학습 데이터나 fine-tuning이 필요해 비효율적이고 성능 향상도 제한적이다. 이를 해결하기 위해 별도의 재학습 없이 테스트 시점에서만 도메인을 자동으로 감지하고 적응하는 Test-Time Domain Adaptation 방식이 필요하다. |
| 사용 기술 | 본 연구에서는 다음과 같은 기술을 활용한다.<br><br>- **Vision-Language Model (CLIP ViT-B/32 기반)**: 이미지와 텍스트를 각각 인코딩한 뒤, 공통 임베딩 공간에서 비교하는 멀티모달 모델<br>- **MTA (MeanShift for Test-Time Augmentation)**: 128장의 augmented view에서 MeanShift 알고리즘으로 outlier를 자동 제거하고 robust한 이미지 임베딩 m*를 획득하는 기법<br>- **Test-Time Domain Adaptation (Training-Free)**: 역전파 없이 테스트 단계에서만 도메인을 자동 추정하여 텍스트·이미지 임베딩을 동적으로 재조합하는 기법.<br>- **Stable Diffusion V2**: 테스트 이미지로부터 도메인 다양성을 확보한 augmented view를 생성하는 이미지 증강 모델<br>- **Linear Projection (768d → 512d)**: 도메인 힌트가 반영된 ViT 출력 임베딩을 텍스트 임베딩과의 유사도 계산을 위해 차원을 맞추는 레이어<br>- **Deep Learning Framework (PyTorch)**: 모델 실험 및 환경 구축<br><br>기존 CLIP의 고정 평균 프롬프트 앙상블을 베이스라인으로 설정하고, 도메인 가중 동적 임베딩 재조합 방식과의 성능을 비교하여 domain shift 환경에서의 성능 개선 여부를 분석한다. |
| 개발환경 | 1. Client 디바이스: PC(Windows, Mac) 및 GPU 서버 기반 연구 환경(Google Colab)<br>2. 딥러닝 프레임워크: Python/PyTorch/CUDA 기반 GPU 환경<br>3. 데이터셋: Domain Generalization 표준 벤치마크 (PACS) + ImageNet 계열 5종(ImageNet, ImageNet-A, ImageNet-V2, ImageNet-R, ImageNet-Sketch) + 특정 도메인 10종(SUN397, Aircraft, EuroSAT, StanfordCars, Food101, OxfordPets, Flower102, Caltech101, DTD, UCF101)<br>4. 활용 모델: CLIP 기반 Vision-Language Model<br>5. 사전학습 모델: CLIP pretrained model (ViT 기반)<br>6. 라이브러리: NumPy, Pandas, Matplotlib, TensorBoard 등<br>7. 이미지 증강: Stable Diffusion V2, RandomCrop |
| 사용하는 소프트웨어 URL | 1. CLIP 공식 코드베이스: https://github.com/openai/CLIP<br>2. DiffTPT 코드베이스: https://github.com/chunmeifeng/DiffTPT<br>3. MTA 코드베이스: https://github.com/MaxZanella/MTA<br>4. ImageNet 데이터셋: https://www.image-net.org<br>5. PACS 데이터셋:  https://huggingface.co/datasets/flwrlabs/pacs <br>6. HuggingFace (사전학습 모델 허브): https://huggingface.co |
| 기대 효과 | 본 연구를 통해 다음과 같은 효과를 기대한다.<br><br>- **Domain Shift 강건성 향상**: 스케치, 회화, 위성사진 등 다양한 도메인 변화 환경에서도 CLIP 기반 Zero-Shot 분류 정확도를 개선한다.<br>- **Training-Free 적응**: 역전파(역전파 기반 프롬프트 튜닝인 TPT 대비) 없이 테스트 시점에서만 동작하므로, 추가 학습 데이터나 GPU 학습 비용 없이 새로운 도메인에 즉시 적용 가능하다.<br>- **텍스트·이미지 임베딩 동시 적응**: 기존 연구들이 텍스트 임베딩만 조정하는 것과 달리, 텍스트와 이미지 임베딩 양쪽을 동일한 도메인 가중치로 동시에 재조합함으로써 이미지-텍스트 정렬 품질을 높인다.<br>- **방법론 확장 가능성**: 제안하는 test-time domain adaptation 방법론은 멀티모달 모델의 domain shift 문제를 다루는 다양한 downstream task로 확장될 수 있으며, 데이터 확보가 어려운 특수 도메인(의료, 위성, 산업용 이미지 등)에서의 멀티모달 AI 활용 가능성을 확대할 것으로 기대된다. |
| GitHub Repo | [https://github.com/chairwomans/chairwomans-capstone](https://github.com/chairwomans/chairwomans-capstone) |
| Team Ground Rule | [Team Ground Rule](https://github.com/chairwomans/chairwomans-capstone/blob/main/docs/Team_Ground_Rule.md) |
| 최종수정일 | 2026-06-02 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-2"></a>
## Team 2 Sudo

| 항목 | 내용 |
|------|------|
| 프로젝트명 | HealthMate AI: 불규칙한 생활 속 2030을 위한 고혈압·당뇨 위험군 대상 식단 인식·코칭 통합 헬스케어 플랫폼 |
| 서비스명(브랜드) | 온케어 (On-Care) |
| 트랙 | 산학 |
| 팀명 | Sudo |
| 팀구성 | 최지수, 박서연, 신수빈 |
| 팀지도교수 | 황의원 교수님 |
| 무엇을 만들고자 하는가 | 불규칙한 생활 습관으로 인해 고혈압·당뇨 위험이 높아진 2030세대를 위한 통합 헬스케어 모바일 플랫폼 On-Care를 개발한다. 음식 사진 한 장으로 식단 기록 과정을 간소화하고, 사용자의 누적 건강 데이터를 바탕으로 맞춤형 코칭을 제공하는 것이 핵심 목표다. 식단 기록, 운동 관리, 건강 일정, AI 상담, 헬스장 탐색, 트레이너 연동, 활동 보상을 하나의 앱에서 관리할 수 있도록 구성한다. |
| 고객 (누구를 위해) | **1차 타깃**: 불규칙한 식사, 운동 부족, 가족력 등으로 인해 고혈압·당뇨 위험 관리가 필요한 2030세대. 건강 관리의 필요성은 인식하지만 복잡한 기록 방식과 파편화된 서비스 때문에 지속적인 실천에 어려움을 느끼는 사용자.<br>**2차 타깃**: 이용자의 건강 데이터를 효율적으로 파악하고 맞춤형 운동 지도를 제공하고자 하는 헬스 트레이너 및 헬스장 운영자. |
| Pain Point (해결할 문제) | **① 식단 기록의 높은 진입 장벽**: 기존 앱은 음식명 검색, 섭취량 입력, 바코드 스캔 등 수동 기록 방식에 의존하여 사용자가 식단 기록을 꾸준히 유지하기 어렵다.<br>**② 기록과 행동 변화의 단절**: 식단과 운동 데이터를 입력하더라도 누적 이력을 반영한 구체적인 피드백이 부족하여 사용자가 무엇을 개선해야 하는지 파악하기 어렵다.<br>**③ 질환 특화 개인화 부족**: 기존 서비스는 체중 감량과 칼로리 관리에 집중되어 있어 나트륨 섭취, GI 분류, 불규칙한 식사 패턴 등 고혈압·당뇨 위험군에게 필요한 관리 요소를 충분히 반영하지 못한다.<br>**④ 파편화된 건강 관리**: 식단, 운동, 병원 일정, 건강 상담, 헬스장 탐색 기능이 여러 서비스에 분리되어 있어 데이터의 연속성이 낮고 앱 전환 과정에서 이탈이 발생한다.<br>**⑤ 온라인 기록과 오프라인 실천의 분리**: 앱에서 기록한 건강 데이터가 실제 운동 지도와 연결되지 않아 트레이너 상담 시 사용자가 직접 정보를 설명하거나 수기로 전달해야 한다.<br>**⑥ 지속적인 참여 동기 부족**: 단기 목표를 달성한 이후에도 기록과 운동을 지속하도록 유도하는 연속 달성 보상과 활동 포인트 체계가 부족하다. |
| 사용 기술 | **현재 MVP 개발**: Flutter 3.x, Dart, Riverpod, GoRouter, Drift.<br>**백엔드 도입 예정**: FastAPI, MySQL, Docker, GitHub Actions, JWT 인증.<br>**AI/ML 파이프라인 도입 예정**: YOLOv8, Gemini Vision API, GPT-4o, LangChain, Pinecone, PyTorch.<br>**외부 API 연동 예정**: Firebase Cloud Messaging, 카카오맵 API, 공공데이터포털 식품영양성분 DB. |
| 개발환경 | **모바일 개발**: Flutter 3.x, Dart SDK, Android Studio, VS Code.<br>**백엔드 개발 예정 환경**: Python, FastAPI, MySQL, Docker.<br>**AI 모델 연동 예정 환경**: YOLOv8, Gemini Vision API, GPT-4o, LangChain, Pinecone, PyTorch.<br>**버전 관리 및 협업**: Git, GitHub, GitHub Issues, Pull Requests, GitHub Actions. |
| 사용하는 소프트웨어 URL | -Flutter: https://flutter.dev<br> -FastAPI: https://fastapi.tiangolo.com<br> -YOLOv8 (Ultralytics): https://github.com/ultralytics/ultralytics<br> -Google Gemini API: https://ai.google.dev<br> -OpenAI GPT-4o: https://openai.com<br> -LangChain: https://www.langchain.com<br> -Pinecone: https://www.pinecone.io<br> -Firebase FCM: https://firebase.google.com<br> -카카오맵 API: https://apis.map.kakao.com<br> -공공데이터포털 식품영양성분 DB: https://www.data.go.kr<br> -AWS (EC2 · RDS): https://aws.amazon.com<br> -Docker: https://www.docker.com |
| 기대 효과 | **① 식단 기록 부담 감소**: 음식명과 섭취량을 직접 입력하는 과정을 사진 촬영 중심으로 단순화하여 식단 기록의 진입 장벽을 낮춘다.<br>**② 개인 맞춤형 행동 변화 유도**: 단편적인 칼로리 알림이 아니라 사용자의 누적 식단, 운동, 건강 기록을 반영한 조언을 제공하여 구체적인 개선 행동을 유도한다.<br>**③ 2030 만성질환 위험 관리 지원**: 고혈압·당뇨 위험과 관련된 생활 습관을 조기에 인지하고 관리할 수 있도록 돕는다.<br>**④ 건강 관리 경험 통합**: 식단, 운동, 일정, AI 상담, 헬스장 탐색을 하나의 앱에서 관리하여 데이터 연속성을 확보한다.<br>**⑤ 온라인 기록과 오프라인 실천 연결**: 트레이너 연동을 통해 앱 안의 건강 기록이 실제 운동 지도에 활용될 수 있도록 한다.<br>**⑥ 장기적인 건강 관리 습관 형성**: 포인트와 Streak 보상을 통해 지속적인 기록과 운동 실천을 유도한다. |
| GitHub Repo | [https://github.com/CSE-Sudo-26/sudo-capstone-project](https://github.com/CSE-Sudo-26/sudo-capstone-project) |
| Team Ground Rule | [Team Ground Rule](https://github.com/CSE-Sudo-26/sudo-capstone-project/blob/main/docs/Team_Ground_Rule.md) |
| 최종수정일 | 2026-06-03 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-3"></a>
## Team 3 Alltology

| 항목 | 내용 |
|------|------|
| 프로젝트명 | 검색 결과와 내부 지식이 충돌할 때: Preference Learning 기반 RAG 정렬 연구 (Conflict-Aware PA-RAG) |
| 서비스명(브랜드) | Alltology |
| 트랙 | 연구 |
| 팀명 | Alltology |
| 팀구성 | 박세령, 손현경, 이다영 |
| 팀지도교수 | 황의원 교수님 |
| 무엇을 만들고자 하는가 | RAG(Retrieval-Augmented Generation)에서 검색된 외부 문서와 LLM 내부 학습 지식이 서로 다른 답을 가리키는 **Knowledge Conflict** 상황을 DPO(Direct Preference Optimization) + LoRA로 해결하는 연구.<br><br>기업 사내 문서 검색, 법률 정보 RAG, 의료 가이드라인 챗봇처럼 정보 버전이 자주 바뀌고 오답의 파급 효과가 큰 도메인에서, AI가 최신 외부 문서를 올바르게 우선하도록 **Preference Learning으로 conflict 처리 능력을 내재화**한다.<br><br>PA-RAG(Preference-Aligned RAG)를 베이스로 삼아, informativeness·robustness·citation quality 외에 **context–memory conflict 해결**을 명시적 정렬 축으로 추가하는 것이 핵심 기여다. |
| 고객 (누구를 위해) | - **1차 타겟**: 사내 RAG 시스템, 법률 정보 챗봇, 의료 가이드라인 검색 등 정보 버전이 자주 바뀌고 knowledge conflict가 치명적인 도메인의 AI 시스템 개발자 및 ML 연구자.<br>- **2차 타겟**: 오래된 학습 지식과 최신 검색 문서 사이의 충돌로 신뢰성 문제를 겪고 있는 RAG 기반 서비스 운영자. |
| Pain Point (해결할 문제) | ① **RAG의 구버전 지식 고집**: 검색된 최신 문서가 있어도 LLM이 학습 당시 습득한 구버전 지식을 고집해 오답 생성. 예) 2024년 개정된 사내 재택근무 정책 질문에 2022년 정책을 답하는 상황.<br>② **신뢰 불가 문서 맹신**: 반대로 부정확하거나 outdated된 검색 문서를 무비판적으로 따르는 문제.<br>③ **기존 PA-RAG의 한계**: informativeness·robustness·citation을 다루지만 context–memory conflict를 명시적 정렬 축으로 다루지 않음.<br>④ **프롬프트의 한계**: 프롬프트 수준의 conflict-aware 지시는 효과가 있으나(파일럿 실험: 거짓 문서 거부율 75%→100%), 모델에 내재화되지 않아 도메인 일반화에 한계. |
| 사용 기술 | **AI/학습**: PyTorch, HuggingFace Transformers, LoRA/PEFT, DPO/TRL, Llama 3.1-8B<br>**RAG/검색**: FAISS (벡터 스토어), Sentence-Transformers (임베딩), Anthropic Claude API (생성)<br>**데모/배포**: Gradio (HuggingFace Spaces 인터랙티브 데모), Python Telegram Bot (Railway 서버 배포), FastAPI<br>**실험/평가**: ClashEval, WikiContradict (평가 벤치마크 후보), LLM-as-a-judge |
| 개발환경 | OS: macOS / Linux (Google Colab GPU 환경)<br>언어: Python 3.10+<br>AI 학습: Google Colab (A100/T4 GPU), HuggingFace Hub (사전학습 모델)<br>RAG 파이프라인: 로컬 MPS (Apple Silicon) / Colab<br>데모 배포: HuggingFace Spaces (Gradio), Railway (텔레그램 봇)<br>버전 관리: Git / GitHub, GitHub Actions, PR 기반 코드 리뷰 |
| 사용하는 소프트웨어 URL | - 인터랙티브 데모: https://huggingface.co/spaces/ponyo03/conflict-aware-rag-demo<br>- 연구 사이트: http://alltology.zapto.org<br>- PyTorch: https://pytorch.org<br>- PEFT/LoRA: https://github.com/huggingface/peft<br>- TRL/DPO: https://github.com/huggingface/trl<br>- FAISS: https://github.com/facebookresearch/faiss<br>- Sentence-Transformers: https://www.sbert.net<br>- Llama 3.1: https://llama.meta.com<br>- Gradio: https://www.gradio.app<br>- Railway: https://railway.app |
| 기대 효과 | ① **conflict 처리 능력 정량화**: 파일럿 실험(gpt-4o-mini)에서 Conflict-Aware Prompting이 거짓 문서 거부율을 75%→100%로 향상. Llama 3.1-8B에서의 gap 측정 및 DPO+LoRA 학습 효과 검증.<br>② **내재화를 통한 일반화**: 프롬프트 의존 없이 모델 자체가 conflict를 인식·해결하도록 학습, 도메인 일반화 성능 향상 기대.<br>③ **실용적 적용 가능성 제시**: 기업 문서 검색·의료·법률처럼 정보 버전이 중요한 도메인 RAG 시스템의 신뢰성 및 안전성 향상에 기여.<br>④ **PA-RAG 확장**: 기존 PA-RAG 정렬 기준(informativeness·robustness·citation)에 knowledge conflict 처리를 추가하는 새로운 정렬 축 제안. |
| GitHub Repo | [https://github.com/Ontology0/Graduation-Project](https://github.com/Ontology0/Graduation-Project) |
| Team Ground Rule | [Team Ground Rule](https://github.com/Ontology0/Graduation-Project/blob/dev/course/team_ground_rule.md) |
| 최종수정일 | 2026.06.01 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-5"></a>
## Team 5 규교굥

| 항목 | 내용 |
|------|------|
| 프로젝트명 | On-device 로컬 LLM 기술을 사용하여 플레이어 맞춤형 힌트를 실시간으로 제공하는 1인칭 3D 공포 방탈출 게임 |
| 서비스명(브랜드) | Do Not Open This Box |
| 트랙 | 산학 |
| 팀명 | 규교굥 |
| 팀구성 | 정혜교, 윤민주, 박남규 |
| 팀지도교수 | 윤명국 교수님 |
| 무엇을 만들고자 하는가 | 6개의 방을 순차적으로 탈출하는 3D 1인칭 공포 방탈출 게임. 각 씬마다 고유한 실내 공간에서 단서를 수집하고 추리하여 탈출 아이템을 찾아 상자에 넣으면 탈출구가 열린다.막혔을 때는 무전기를 통해 On-device LLM(Ollama)에 힌트를 요청할 수 있으며, LLM은 플레이어의 물음을 토대로 맞춤형 힌트를 제공한다(씬당 2회 사용 가능). |
| 고객 (누구를 위해) | 방탈출·퍼즐 게임을 즐기지만 난이도에 막혀 중도 포기한 경험이 있는 PC 게이머, 호러 게임 콘텐츠를 즐기는 영상 플랫폼 이용자 |
| Pain Point (해결할 문제) | 방탈출 게임을 플레이하다 너무 어려워 포기하는 유저가 많다. 특히 스토리 중심 게임에서 특정 단계에 막히면 외부 공략을 찾게 되어 몰입이 깨진다. 기존 게임은 플레이어의 현재 상황을 반영한 맞춤형 힌트를 제공하지 못한다. 본 프로젝트는 On-device LLM을 통해 플레이어의 물음을 토대로 맞춤형 힌트를 게임 내에서 바로 제공함으로써, 이탈 없이 자연스럽게 플레이를 이어갈 수 있도록 한다. |
| 사용 기술 | 유니티 3D, Ollama |
| 개발환경 | 1. Client 디바이스: PC (Windows, Mac)<br>2. FE: Unity, Blender, Clip studio<br>3. BE: 초기에는 Standalone 형태로 개발 후, 필요 시 FastAPI 기반 서버 연동 예정<br>4. DB: 초기에는 로컬 데이터 저장 방식을 고려하고 있으며, 필요 시 MySQL 도입 예정<br>5. 특별한 라이브러리: Unity URP/2D Light, TextMeshPro, JsonUtility, Custom Render Feature, Shader Graph, Post Processing, Cinemachine<br>6. API Call 서비스:  Ollama 4B 기반 로컬 LLM
| 사용하는 소프트웨어 URL | unity.com / blender.org / ollama.com
| 기대 효과 | 플레이어는 공포 분위기 속 추리·탐색의 긴장감을 즐기는 동시에, On-device LLM 기반 맞춤형 힌트로 게임 흐름을 끊지 않고 자연스럽게 진행할 수 있다. 외부 서버 없이 로컬에서 실행되어 API 비용이 없으므로 플레이어가 비용을 부담할 필요가 없으며, 또한 플레이어마다 다른 맥락 기반 힌트 경험을 제공한다. |
| GitHub Repo | [https://github.com/muffinhead03/Start2026_1](https://github.com/muffinhead03/Start2026_1) |
| Team Ground Rule | https://github.com/muffinhead03/Start2026_1/blob/main/Team_Ground_Rule.md |
| 최종수정일 | 2026.05.01 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-6"></a>
## Team 6 Greenfield

| 항목 | 내용 |
|------|------|
| 프로젝트명 | 역사 스토리 콘텐츠와 역사 인물 챗봇을 활용한 관광 탐색 웹 플랫폼 |
| 서비스명(브랜드) | Histour |
| 트랙 | 산학 |
| 팀명 | Greenfield |
| 팀구성 | 최준희, 권은재, 김재희 |
| 팀지도교수 | 박현석 |
| 무엇을 만들고자 하는가 | 사용자에게 AI 기반 역사 스토리 콘텐츠(텍스트, 영상)와 역사 인물 챗봇과의 대화 기능을 제공하여 역사에 흥미를 느낄 수 있도록 유도한 후, 위 콘텐츠들과 관련한 관광지를 추천하여 대한민국 관광을 활성화할 수 있는 웹 플랫폼을 만들고자 한다. |
| 고객 (누구를 위해) | 역사에 큰 관심은 없지만 재미있는 콘텐츠에는 반응하는 20~30대 사용자<br>여행을 계획 중이거나, 새로운 여행지를 찾고 싶은 사용자<br>한국 문화를 경험해 보고 싶은 외국인<br>기존 관광 정보 서비스에 흥미를 느끼지 못한 사용자 |
| Pain Point (해결할 문제) | - 역사 정보를 흥미롭게 전달하는 매체 부족<br>- 외국인 관광객의 한국 역사 이해 및 관광 접근성 부족<br>- 학생들이 실제 역사 장소를 체험하며 학습할 기회 부족<br><br>스토리를 중심으로 역사 장소를 연결하여 외국인과 학생 모두가 한국 역사를 쉽게 이해하고 직접 체험할 수 있는 몰입형 문화관광 경험을 제공하는 것을 목표 |
| 사용 기술 | **프론트엔드**<br><br>- Next.js, React, TypeScript, Tailwind CSS, Kakao Maps API<br><br>**백엔드**<br><br>- Node.js , MySQL, FastAPI<br><br>**데이터 수집**<br><br>- 관광지 위치, 관광지 관련 이미지 및 텍스트 데이터 분석<br><br>**AI 및 추천 시스템**<br><br>- 스토리 기반 관광 코스 추천 알고리즘, LLM 기반 역사 요약 및 다국어 번역 |
| 개발환경 | 1. Client 디바이스를 PC로 제공<br>2. FE는 Next.js(React), TypeScript 사용<br>3. BE는 FastAPI 사용<br>4. DB는 PostgreSQL 사용<br>5. 사용하는 특별한 라이브러리는 FE ( Tailwind CSS, TanStack Query, Leaflet) / BE ( SQLAlchemy, Pydantic, Uvicorn) 사용<br>6. API Call로 사용할 서비스는 OpenAI 사용
| 사용하는 소프트웨어 URL | 1. Client 디바이스를 PC로 제공<br>2. FE는 Next.js(React), TypeScript 사용<br>3. BE는 FastAPI 사용<br>4. DB는 PostgreSQL 사용<br>5. 사용하는 특별한 라이브러리는 FE ( Tailwind CSS, TanStack Query, Leaflet) / BE ( SQLAlchemy, Pydantic, Uvicorn) 사용<br>6. API Call로 사용할 서비스는 OpenAI 사용
| 기대 효과 | 모두가 쉽게 이해하고 직접 체험할 수 있는 몰입형 문화 관광 경험을 제공하여 한국 역사에 대한 사람들의 관심과 흥미를 유도한다. 또한 이에 따른 한국 관광지 활성화를 목표로 한다. |
| GitHub Repo | [https://github.com/greenfield-2026-capstone/greenfield-project](https://github.com/greenfield-2026-capstone/greenfield-project) |
| Team Ground Rule | https://github.com/greenfield-2026-capstone/greenfield-project/blob/main/Team_Ground_Rule.md |
| 최종수정일 | 2026.4.12 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-7"></a>
## Team 7 reverdir

| 항목 | 내용 |
|------|------|
| 프로젝트명 | 익명 매칭, 질문, 미션, 쪽지 상호작용을 통해 사람들 사이의 자연스러운 관계 형성과 친밀감 형성을 돕는 마니또 기반 소셜 게임 플랫폼 |
| 서비스명(브랜드) | 또마니또(ToManito) |
| 트랙 | 산학 |
| 팀명 | reverdir |
| 팀구성 | 전채연, Lyu Dongying, 이은효 |
| 팀지도교수 | 이미정 교수님 |
| 무엇을 만들고자 하는가 | 또마니또(To-Manito)는 사람들 사이의 자연스러운 관계 형성과 친밀감 형성을 돕기 위해 설계된 익명 기반 소셜 게임 플랫폼입니다.<br>사람들은 새로운 모임에 참여하거나 여러 사람과 함께 시간을 보내더라도 서로를 알아갈 계기를 찾지 못해 어색함을 느끼는 경우가 많습니다. 또한 기존의 마니또 이벤트는 짧은 기간 동안의 재미를 제공하는 데 그치는 경우가 많아, 참여자 간 지속적인 상호작용이나 관계 형성으로 이어지지 못하는 한계가 있습니다.<br>또마니또는 이러한 문제를 해결하기 위해 관계가 자연스럽게 시작되고 이어질 수 있는 게임 경험을 제공합니다. 참가자는 익명 마니또 매칭을 통해 부담 없이 상대에게 관심을 가질 수 있으며, 질문, 미션, 익명 쪽지와 같은 다양한 상호작용을 통해 서로를 조금씩 알아가게 됩니다. 이러한 과정은 자연스러운 대화의 소재를 제공하고, 참여자들이 상대에 대한 관심과 호기심을 바탕으로 관계를 형성할 수 있도록 돕습니다. 또한 게임 종료 후에는 AI 기반 결과 리포트를 제공하여 참여 경험을 재미있는 콘텐츠로 남길 수 있도록 하였습니다. 참가자들은 서로의 결과를 공유하며 추가적인 대화를 나누고, 함께했던 경험을 추억으로 회고할 수 있습니다.<br>이를 통해 또마니또는 단발성 이벤트를 넘어 반복적으로 즐기고 싶은 관계 경험을 만드는 것을 목표로 합니다. |
| 고객 (누구를 위해) | 또마니또의 주요 고객은 학교, 동아리, 학회, 프로젝트 팀, 직장 조직, 친구 모임 등 여러 사람이 함께 활동하는 소규모 그룹입니다.<br>특히 구성원 간 관계를 더욱 가깝게 만들고 싶거나, 새로운 구성원들과 자연스럽게 친해질 계기를 만들고 싶은 모임에 적합합니다.<br>새 학기 OT나 MT와 같이 처음 만난 사람들이 어색함을 해소해야 하는 상황부터, 이미 알고 지내는 친구나 팀원들이 서로에 대해 몰랐던 모습을 발견하고 더욱 친밀해지고 싶은 상황까지 다양한 환경에서 활용할 수 있습니다.<br>또한 마니또 이벤트를 운영하는 것을 넘어, 구성원들이 함께 즐기고 기억할 수 있는 특별한 경험을 만들고 싶은 사용자들을 주요 대상으로 합니다. |
| Pain Point (해결할 문제) | 1. 사람들은 함께 있어도 서로를 알아갈 기회가 부족합니다.<br>새로운 모임이나 단체 활동에서는 구성원들이 같은 공간에 있더라도 자연스럽게 대화를 시작하거나 서로를 알아갈 계기를 만들기 어렵습니다. 그 결과 어색한 분위기가 오래 지속되거나 일부 사람들끼리만 교류하게 되는 경우가 많습니다.<br><br>2. 기존 마니또 이벤트는 관계 형성 경험으로 이어지기 어렵습니다.<br>기존 마니또는 선물 교환이나 정체 공개에 초점이 맞춰져 있어 이벤트 자체는 재미있지만, 참여자 간 지속적인 상호작용을 유도하기에는 한계가 있습니다. 이벤트가 끝난 뒤에는 특별한 관계 변화 없이 마무리되는 경우도 많습니다.<br><br>3. 참여를 지속할 수 있는 동기가 부족합니다.<br>기존 마니또에서는 게임 기간 동안 참여자들이 꾸준히 활동할 이유가 부족합니다. 시간이 지날수록 관심과 참여도가 감소하며, 일부 참가자만 적극적으로 참여하게 되는 문제가 발생합니다.<br><br>4. 함께한 경험이 자연스럽게 사라집니다.<br>이벤트 기간 동안의 상호작용과 재미있는 순간들은 대부분 기록으로 남지 않고 잊히게 됩니다. 참가자들이 경험을 되돌아보거나 서로 공유하며 대화를 이어갈 수 있는 장치도 부족합니다.<br><br>또마니또는 익명 매칭, 질문, 미션, 쪽지, AI 결과 리포트를 통해 이러한 문제를 해결하고, 사람들이 서로를 알아가고 가까워지는 과정을 하나의 즐거운 게임 경험으로 제공하고자 합니다. |
| 사용 기술 | FE: Flutter (Dart) 기반 크로스 플랫폼 모바일 UI 구현<br>BE: Spring Boot (Java) 기반 REST API 서버 및 게임 로직 처리<br>DB: PostgreSQL (관계형 데이터 구조 및 게임 상태 관리)<br>Auth: JWT 기반 사용자 인증 및 세션 관리<br>AI: Gemini 3.1 Flash API 기반 사용자 활동 데이터 분석 및 결과 리포트 생성<br>Architecture: 클라이언트-서버 구조 기반 비동기 게임 흐름 처리 |
| 개발환경 | Client: Flutter (Android / Web 대응)<br>Backend: Spring Boot 기반 REST API<br>Database: PostgreSQL<br>Build / Deploy: Render (Backend), Vercel (Frontend)<br>Version Control: GitHub |
| 사용하는 소프트웨어 URL | Flutter: https://flutter.dev<br>Spring Boot: https://spring.io/projects/spring-boot<br>PostgreSQL: https://www.postgresql.org<br>Gemini API: https://ai.google.dev<br>Render: https://render.com<br>Vercel: https://vercel.com |
| 기대 효과 | 또마니또를 통해 사용자는 마니또 이벤트를 단순한 과제가 아니라, 함께 참여하며 자연스럽게 즐기는 경험으로 느낄 수 있습니다.<br>익명 기반의 매칭과 질문, 미션 등의 요소는 대화가 생기게 되는 상황을 제공합니다.<br>이벤트가 진행되는 동안 사용자는 서로를 조금씩 알아가고, 이전보다 자연스럽게 관계를 이어가게 됩니다. 또한 종료 이후에는 AI 기반 결과 리포트를 통해 각자의 참여 경험을 가볍게 공유하고 이야기할 수 있으며, 이 과정에서 단순한 종료가 아니라 대화가 다시 시작되는 계기가 만들어집니다.<br>결과적으로 또마니또는 마니또 이벤트를 끝나는 활동이 아니라, 함께한 시간을 다시 이야기하게 되는 경험으로 확장시키는 것을 목표로 합니다. |
| GitHub Repo | [https://github.com/team-capstone-reverdir-2026/reverdir_repo](https://github.com/team-capstone-reverdir-2026/reverdir_repo) |
| Team Ground Rule | https://github.com/team-capstone-reverdir-2026/reverdir_repo/blob/main/Team_Ground_Rule.md |
| 최종수정일 | 2026.06.03 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-8"></a>
## Team 8 하면된다

| 항목 | 내용 |
|------|------|
| 프로젝트명 | AI 기반 가격 검증과 정시 경매 시스템으로 정보 비대칭과 탐색 피로를 해결하는 빈티지 거래 플랫폼 |
| 서비스명(브랜드) | Vintic |
| 트랙 | 산학 |
| 팀명 | 하면된다 |
| 팀구성 | 김수연, 이예주, 조채윤 |
| 팀지도교수 | 오세은 교수님 |
| 무엇을 만들고자 하는가 | 판매자가 제시한 가격이 적절한지 AI가 함께 검증하고, 구매자는 정해진 시간에 열리는 경매를 통해 상품을 효율적으로 탐색할 수 있도록 하여, 빈티지 거래 과정에서 발생하는 가격 판단의 어려움과 무한 탐색의 피로를 줄이는 플랫폼을 구현합니다. |
| 고객 (누구를 위해) | 빈티지 거래 플랫폼 이용자 |
| Pain Point (해결할 문제) | (1) 가격 정보의 불균형: 판매자가 상품 가격을 임의로 책정하는 경우가 많아, 구매자가 적정 가격을 판단하기 어려운 구조</br>(2) 구매자의 탐색 피로: 원하는 매물의 업로드 시점을 알기 어려워, 사용자가 플랫폼에 반복적으로 접속하며 무한 스크롤링을 지속하는 문제</br>(3) 판매글 노출의 비효율: 게시글이 업로드 시점에 따라 쉽게 묻혀, 판매자가 동일한 글을 반복 업로드해야 하는 비효율 |
| 사용 기술 | Vision AI(FastAPI+상용 API), Spring, React 등 |
| 개발환경 | 1.Client Device: Wep App<br>2.FE(Web)<br>Core: React, TypeScript, Next.js<br>State Management: TanStack Query, Zustand<br>Styling: Emotion<br>CI/CD: GitHub Actions<br>3.BE:SpringBoot,docker<br>4.DB:MySQL<br>5.BE:Spring Data JPA,Spring WebSockets FE:Emotion,TanStack Query,Zustand<br>6.API Call 서비스:OpenAI API(GPT-4o Vision)
| 사용하는 소프트웨어 URL | 1.Client Device: Wep App<br>2.FE(Web)<br>Core: React, TypeScript, Next.js<br>State Management: TanStack Query, Zustand<br>Styling: Emotion<br>CI/CD: GitHub Actions<br>3.BE:SpringBoot,docker<br>4.DB:MySQL<br>5.BE:Spring Data JPA,Spring WebSockets FE:Emotion,TanStack Query,Zustand<br>6.API Call 서비스:OpenAI API(GPT-4o Vision)
| 기대 효과 | (1) 상품별 AI 측정가와 판매자 희망가 병기를 통한 가격 판단 기준 제공</br>(2) AI 측정가와 희망가 차이 제한을 통한 가격 신뢰도 향상</br>(3) 특정 시각 일괄 경매 방식을 통한 구매자 탐색 피로 완화 및 판매자 노출 기회의 공정성 확보 |
| GitHub Repo | [https://github.com/hamyeon/Team-Hamyeon](https://github.com/hamyeon/Team-Hamyeon) |
| Team Ground Rule | [Team Grouond Rule](https://github.com/hamyeon/Team-Hamyeon/blob/main/Team_Ground_Rule.md) |
| 최종수정일 | 2026.03.16 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-9"></a>
## Team 9 Cloud9

| 항목 | 내용 |
|------|------|
| 프로젝트명 | 반복적인 손실을 겪는 개인 주식 투자자를 위한 AI 기반 매매 행동 분석 및 맞춤형 투자 습관 개선 플랫폼 |
| 서비스명(브랜드) | Canary |
| 트랙 | 산학 |
| 팀명 | Cloud9 |
| 팀구성 | 박나림, 임도경, 최은우 |
| 팀지도교수 | 이민수 |
| 무엇을 만들고자 하는가 | 개인 주식 투자자의 매매 로그를 AI로 분석하여 비이성적 매매 패턴을 자동 탐지하고, 손실의 원인을 데이터 기반으로 설명하여 투자자 스스로 자신의 매매 패턴을 인지할 수 있도록 돕는 매매 행동 분석 플랫폼 |
| 고객 (누구를 위해) | 반복적인 손실을 겪는 일반 개인 투자자. 2020년 이후 국내 개인 투자자 수가 역대 최고치를 기록하고 있으나, 대다수가 감정 기반 매매를 반복하며 손실을 겪고 있음|
| Pain Point (해결할 문제) | 기존 금융 서비스는 종목 추천, 시장 분석 등 '무엇을 살지'에만 집중할 뿐, 투자자가 '왜 반복해서 잃는지'에 대한 원인 분석이 전무함. 투자자 본인도 인지하지 못하는 비이성적 매매 패턴을 객관적인 데이터로 진단하고 분석하는 서비스가 국내에는 존재하지 않음. |
| 사용 기술 | Front(React, Recharts), Back(Python, FastAPI, SQLAlchemy), AI(PyTorch, Integrated Gradients, Scikit-learn, Pandas, NumPy)  |
| 개발환경 | 1. Client 디바이스 - PC, Mobile Web <br> 2. FE - React(javascript), Recharts <br> 3. BE - FastAPI <br> 4. DB - PostgreSQL <br> 5. (BE) - Pandas/NumPy, Scikit-learn, PyTorch, Integrated Gradients
| 사용하는 소프트웨어 URL | 1. Client 디바이스 - PC, Mobile Web <br> 2. FE - React(javascript), Recharts <br> 3. BE - FastAPI <br> 4. DB - PostgreSQL <br> 5. (BE) - Pandas/NumPy, Scikit-learn, PyTorch, Integrated Gradients
| 기대 효과 | 투자자 본인도 인지하지 못했던 비이성적 매매 행동을 데이터로 직면하게 하여 손실 원인을 스스로 이해하고 투자 습관을 개선할 수 있도록 지원. 장기적으로 개인 투자자의 실질적인 손실 방어 및 건전한 투자 습관 형성에 기여 |
| GitHub Repo | https://github.com/Cloud9-capstone-2026/cloud9 |
| Team Ground Rule | [Team Ground Rule](https://github.com/Cloud9-capstone-2026/cloud9/blob/main/Team_Ground_Rule.md) |
| 최종수정일 | 2026.05.19 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-10"></a>
## Team 10 212223

| 항목 | 내용 |
|------|------|
| 프로젝트명 | 프롬프트 자동 최적화 기반 LLM API 비용 실시간 비교 웹 서비스 |
| 서비스명(브랜드) | |
| 트랙 | 산학 |
| 팀명 | 212223 |
| 팀구성 | 고윤진(2176018), 김나현(2276040), 이유진(2376218) |
| 팀지도교수 | 심재형 교수님 |
| 무엇을 만들고자 하는가 |  비개발자가 비효율적인 프롬프트를 입력하면, filler word·모호 표현·중복 코드를 실시간으로 감지하고, 오픈소스(LLMLingua, LangChain) 기반으로 프롬프트를 자동 최적화하여 전후 토큰 차이를 시각화하고, 7개 주요 LLM 모델의 예상 비용을 실시간 비교하는 웹 서비스 |
| 고객 (누구를 위해) | AI를 활용하여 코딩을 하고자 하는 비개발자 (바이브코딩 사용자, AI 기반 프로토타이핑을 하는 학생·기획자·스타트업 등 토큰 개념 없이 LLM을 사용하는 사용자) |
| Pain Point (해결할 문제) | ① 토큰 개념에 대한 이해 부족으로 인한 무의식적 비용 낭비 (바이브코딩 세션당 생성 코드의 30~40%가 폐기, 구조화 대비 3~4배 토큰 과소비) ② 개발 구조와 로직에 대한 이해 부족으로 인한 모호한 요구, 코드 통째 전송, 반복적 재프롬프팅 ③ 토큰과 모델별 가격 차이에 대한 인지 저조 |
| 사용 기술 | 오픈소스: tiktoken (토큰 정밀 측정), LangChain (프롬프트 템플릿 관리 및 체이닝), LLMLingua 또는 DSPy (프롬프트 압축/최적화, 성능 비교 후 택 1) |
| 개발환경 | 1. Client 디바이스: PC (Windows, Mac) 2. FE: Next.js, React, TailwindCSS, TanStack Query 3. BE: FastAPI (Python) 4. DB: Firebase Firestore 5. AI/NLP 오픈소스: tiktoken, LangChain, LLMLingua 또는 DSPy 6. 외부 API: OpenAI / Anthropic / Google AI SDK 7. 자체 개발 모듈: filler word 감지, 모호 표현 탐지, 토큰 과다 경고, 모델 추천 엔진 8. 배포: Vercel (프론트) + Railway 또는 Render (백엔드) 9. 특수 라이브러리: LiteLLM (백엔드 멀티모델 통합) |
| 사용하는 소프트웨어 URL | tiktoken: https://github.com/openai/tiktoken LangChain: https://github.com/langchain-ai/langchain LLMLingua: https://github.com/microsoft/LLMLingua DSPy: https://github.com/stanfordnlp/dspy LiteLLM: https://github.com/BerriAI/litellm Next.js: https://github.com/vercel/next.js FastAPI: https://github.com/tiangolo/fastapi Firebase: https://firebase.google.com TanStack Query: https://github.com/TanStack/query |
| 기대 효과 | ① 비개발자의 프롬프트 토큰 낭비를 시각화하여 인지시키고, 자동 최적화를 통해 평균 40% 이상의 토큰 절감 ② 모델별 비용 실시간 비교를 통해 동일 품질 대비 최저 비용 모델 선택 유도 ③ filler word 감지, 모호 표현 경고, 분할 제안 등 실시간 가이드를 통해 사용자의 프롬프트 작성 역량 자체를 향상 |
| GitHub Repo | [https://github.com/0727n1122-beep/graduationproject](https://github.com/0727n1122-beep/graduationproject) |
| Team Ground Rule | [Team Ground Rule](https://github.com/0727n1122-beep/graduationproject/blob/main/Team_Ground_Rule.md) |
| 최종수정일 | 04.15 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-11"></a>
## Team 11 알고리듬

| 항목 | 내용 |
|------|------|
| 프로젝트명 | SpeedSchedule: 인력 운영 최적화를 위한 AI 스케줄링 및 시간표 관리 웹 플랫폼 |
| 서비스명(브랜드) | 우리학교시간표 |
| 트랙 | 산학 |
| 팀명 | 알고리듬 |
| 팀구성 | PM / 조상은 / 컴퓨터공학과 / 2376273 <br> FE&Design / 정지유 / 국제사무학과 / 2416023 <br> BE&AI / 이시은 / 컴퓨터공학과 / 2466044 |
| 팀지도교수 | 오세은 교수님  |
| 무엇을 만들고자 하는가 | 인력 운영 최적화를 위한 AI 스케줄링 및 시간표 관리 웹 플랫폼.<br>교내의 복잡한 수업 시간표와 감독 배정 업무를 데이터 기반으로 자동화하며, 실시간 수정이 가능한 인터렉티브 캘린더와 결원 발생기 대리 근무자를 매칭해주는 기능까지 통합된 관리 솔루션. |
| 고객 (누구를 위해) | 학교 현장의 행정 관리자와 교사 |
| Pain Point (해결할 문제) | 기존 시스템은 AI 최적화가 없는 단순 알고리즘이라 교사 개개인의 선호도나 숙련도 반영이 불가능함. 이로 인해 관리자가 엑셀로 2차 수동 수정을 거치는 등 행정력이 낭비됨. <br> 또한 가나다순/ 고정 순번제 배정은 특정 인원에게 업무가 쏠리는 불균형을 초래하여 조직 내 공정성 시비와 만족도 저하를 일으킴. |
| 사용 기술 | AI : 딥러닝 기반 스케줄 최적화 알고리즘 (PyTorch / TensorFlow) <br> FE : React, Vite, Axios, Vercel, ESLint <br> BE : SpringBoot 3, MySQL, Hibernate(JPA), Docker, Gradle <br> DevOps : Docker, GitHub Action <br> Infra : AWS EC2 (Amazon Linux), AWS RDS
| 개발환경 | 1. Web -> PC 권장<br>2. javaScript<br>3. spring<br>4. MySQL 인데 PostgreSQL로 이전 고려중<br>5. Redis 캐싱<br>6. OpenAI
| 사용하는 소프트웨어 URL | 1. Web -> PC 권장<br>2. javaScript<br>3. spring<br>4. MySQL 인데 PostgreSQL로 이전 고려중<br>5. Redis 캐싱<br>6. OpenAI
| 기대 효과 | 스케줄링 업무 자동화를 통한 행정 비용 절감 및 운영 효율성 극대화. <br> 데이터 기반의 객관적 배정 시스템을 통한 운영의 투명성 확보. <br> 교사 업무 만족도 향상 및 조직 내 인력 운영 효율성 극대화.  |
| GitHub Repo | [https://github.com/speedSchedule/AlgoRhythm](https://github.com/speedSchedule/AlgoRhythm) |
| Team Ground Rule | [Team_Ground_Rule.md](https://github.com/speedSchedule/AlgoRhythm/blob/main/Team_Ground_Rule.md) |
| 최종수정일 | 2025/04/09 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-12"></a>
## Team 12 404

| 항목 | 내용 |
|------|------|
| 프로젝트명 | 여성 1인 여행자를 위해, AI 기반 안전 분석으로 정보 공백을 해결하고 안전 경로를 추천하는 지도 서비스 |
| 서비스명(브랜드) | 여기지! (여성 기행 지켜!) |
| 트랙 | 산학 |
| 팀명 | 404 |
| 팀구성 | 이아림, 노유나, 이채원  |
| 팀지도교수 | 오유란 |
| 무엇을 만들고자 하는가 | 여성 혼자 여행하는 사람들을 위한 안전 중심 여행 플랫폼을 개발하고자 한다. 여성 사용자들이 직접 작성한 안전 리뷰 데이터를 기반으로 여행지의 안전도를 지도에 표시하고, 이를 활용해 안전한 여행 경로를 추천한다. |
| 고객 (누구를 위해) | 20대 초반 여성교환 학생, 사회초년생 여성 직장인(20대 중후반) |
| Pain Point (해결할 문제) | 여성의 안전 정보 부족과 혼자 여행할 때의 불안감 |
| 사용 기술 | [AI] OpenAI API <br> [Frontend] React, Google Cloud Console, HTML / CSS / JavaScript <br> [Backend] FastAPI<br> [Database] MySQL |
| 개발환경 | 1. Client 디바이스는 Windows를 기반으로 한 PC로 한다.<br>2. FE는  React를 사용한다.<br>3. BE는 FastAPI를 기반으로 구현한다.<br>4. DB는 MySQL를 사용한다.<br>5. FE또는 BE에 사용하는 특별한 라이브러리는 Google Maps JavaScript API를 활용하여 지도 기반 기능을 구현한다.<br>6. API Call을 위해 OpenAI 서비스를 사용한다.
| 사용하는 소프트웨어 URL | 1. Client 디바이스는 Windows를 기반으로 한 PC로 한다.<br>2. FE는  React를 사용한다.<br>3. BE는 FastAPI를 기반으로 구현한다.<br>4. DB는 MySQL를 사용한다.<br>5. FE또는 BE에 사용하는 특별한 라이브러리는 Google Maps JavaScript API를 활용하여 지도 기반 기능을 구현한다.<br>6. API Call을 위해 OpenAI 서비스를 사용한다.
| 기대 효과 | 여성 1인 여행자가 안전하고 효율적으로 여행을 계획할 수 있고, 여성의 이동권과 안전권을 기술적으로 보장한다. |
| GitHub Repo | https://github.com/capstone-team404/Spring404 |
| Team Ground Rule | (https://github.com/capstone-team404/Spring404/blob/main/Team_Ground_Rule.md) |
| 최종수정일 | 26.05.06 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---
<a id="team-13"></a>
## Team 13 Semicolone;

| 항목 | 내용 |
|------|------|
| 프로젝트명 | AI 질문을 ‘기억되는 인사이트’로 바꿔주는 개인 지식 관리 플랫폼 |
| 서비스명(브랜드) | Flow(플로우) |
| 트랙 | 산학 |
| 팀명 | Semicolone; |
| 팀구성 | 신지원, 이채원, 윤현진 |
| 팀지도교수 | 이미정 |
| 무엇을 만들고자 하는가 | 본 프로젝트는 AI 기반 질문 기록 및 인사이트 내재화 모바일 플랫폼의 핵심 기능을 구현한다. 생성형 AI와의 대화 내용을 단순히 저장하는 것을 넘어, AI가 질문과 답변을 자동으로 요약하고 핵심 키워드를 추출하여 체계적인 지식 자산으로 전환하는 시스템을 구축한다. 본 단계(MVP)에서는 모바일 환경에서의 데이터 구조화와 핵심 요약, 그리고 월간 회고 기능 구현에 집중한다. 나아가 향후 플랫폼 접근성을 극대화할 '브라우저 익스텐션' 연동과, 사용자의 관심사 및 사고 패턴을 시각적으로 추적할 수 있는 AI 기반 '성향 분석 기능' 확장을 통해 점진적으로 완성형 개인 지식 관리 플랫폼을 구축하는 것을 목표로 한다.  |
| 고객 (누구를 위해) | 본 서비스의 주요 고객은 생성형 AI를 자주 활용하는 사용자들이다. 특히 학습이나 과제, 프로젝트, 창업 아이디어 탐색 등을 위해 AI에게 질문을 자주 하는 대학생을 주요 타겟으로 한다. AI를 통해 얻은 방대한 정보를 체계적으로 정리하고 내재화하고 싶은 사용자, 그리고 자신의 관심사와 학습 패턴을 돌아보며 성장을 추적하고 싶은 사용자에게 적합한 서비스이다. |
| Pain Point (해결할 문제) | AI와의 대화 이력은 길고 비정형적인 텍스트로 구성되어 있어, 시간이 흐른 뒤 필요한 핵심 정보를 다시 찾아내거나 기억하기 어렵다는 문제가 있다. 이로 인해 유익한 정보가 일회성으로 휘발되며, 개인의 지식으로 축적되지 못하는 비효율이 반복되고 있다.  |
| 사용 기술 | 🔹 프론트엔드: React Native<br>- 크로스플랫폼 모바일 앱 개발로 iOS/Android 동시 지원<br>- 컴포넌트 기반 구조를 통한 효율적 UI 개발 및 직관적인 인사이트 탐색 UX 구현<br><br>🔹 백엔드: FastAPI (Python)<br>- 비동기 처리 기반의 고성능 REST API 서버 구축<br>- 확장 가능한 라우터/스키마/모델 분리 구조 설계<br><br>🔹 데이터베이스: PostgreSQL<br>- 강력한 무결성을 기반으로 한 인사이트 간 논리적 연결 체계 관리<br>- 축적된 데이터의 안정적 보존 및 고도화된 지식 검색 기반 제공<br><br>🔹 AI 및 데이터 처리: Groq Cloud API (Llama 3.3)<br>- LPU 가속 엔진을 통한 실시간 인사이트 요약 및 분석<br>- 정교한 프롬프트 설계를 통한 JSON 기반 구조화 데이터 생성<br><br>🔹 배포: Oracle Cloud Free Tier + GitHub Actions CI/CD<br>- dev/main 브랜치 push 시 Oracle Cloud 서버 자동 배포 |
| 개발환경 | 🔹 OS: Windows 11<br>🔹 IDE: Visual Studio Code<br>🔹 프론트엔드: React Native (크로스플랫폼 모바일 UI/UX 설계)<br>🔹 백엔드: FastAPI / Python (비동기 REST API 서버)<br>🔹 데이터베이스: PostgreSQL (데이터 무결성 및 관계형 관리)<br>🔹 AI 엔진: Groq Cloud (Llama 3.3 실시간 추론)<br>🔹 로컬 개발: Docker Desktop + docker-compose<br>🔹 배포: Oracle Cloud Free Tier<br>🔹 버전 관리: Git, GitHub |
| 사용하는 소프트웨어 URL | 🔹 React Native: https://reactnative.dev/<br>🔹 FastAPI: https://fastapi.tiangolo.com/<br>🔹 PostgreSQL: https://www.postgresql.org/<br>🔹 Groq Cloud API: https://groq.com/<br>🔹 Llama 3.3: https://llama.meta.com/ |
| 기대 효과 | 본 서비스를 통해 사용자는 AI와의 대화에서 얻은 정보를 모바일 환경에서 언제든 체계적으로 관리할 수 있으며 저장된 인사이트는 카테고리와 키워드 기반으로 구조화되어 학습이나 프로젝트 과정에서 다시 활용될 가능성이 높아진다. 월간 회고 기능을 통해 한 달간의 질문 패턴을 돌아볼 수 있으며, AI 사용이 단순한 일회성 문답에서 끝나는 것이 아니라 개인의 지속적인 지식 축적과 성장을 돕는다. 결과적으로 현재 구현된 핵심 기능을 통해 지식 휘발 문제를 즉각적으로 해결할 수 있으며, 추후 브라우저 익스텐션과 성향 분석 기능이 추가됨에 따라 정보 수집의 편의성 향상 및 깊이 있는 자기 이해 효과까지 점진적으로 확대될 것으로 기대된다. |
| GitHub Repo | [https://github.com/Semicolone/start](https://github.com/Semicolone/start) |
| Team Ground Rule | [https://github.com/Semicolone/start/blob/main/Team_Ground_Rule.md](https://github.com/Semicolone/start/blob/main/Team_Ground_Rule.md) |
| 최종수정일 | 2026.06.03. |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-14"></a>
## Team 14 def

| 항목 | 내용 |
|------|------|
| 프로젝트명 | 코딩 에이전트를 위한 AST 기반 kv 재사용 추론 최적화 |
| 서비스명(브랜드) | |
| 트랙 | 연구 |
| 팀명 | def |
| 팀구성 | 서혜원, 신은서, 이재린 |
| 팀지도교수 | 심재형 교수님 |
| 무엇을 만들고자 하는가 | AI 코딩 에이전트가 멀티턴 세션에서 반복적으로 등장하는 코드 블록을 매번 처음부터 재계산하는 문제를 해결한다. 코드의 AST 구조를 활용해 함수·클래스·import 같은 블록 단위로 KV Cache를 재사용하고, 위치가 달라지더라도 RoPE re-positioning으로 보정하여 첫 응답 지연(TTFT)을 줄이는 추론 최적화 레이어를 구현한다.|
| 고객 (누구를 위해) | - 로컬 LLM으로 코딩 에이전트를 운용하는 개인 개발자 / 연구자 <br>- API 비용 대신 온디바이스 추론을 선택한 팀 (스타트업, 보안 민감 조직) <br>- NVIDIA GPU 기반 자체 인프라 운용 조직 |
| Pain Point (해결할 문제) | 코딩 에이전트의 멀티턴 세션에서 매 턴마다 타임스탬프·도구 호출 ID(tool_call_id) 등 동적 메타정보가 프롬프트 앞부분에 삽입된다. 이로 인해 "연속된 앞부분 토큰이 완전히 동일"해야 작동하는 vLLM prefix caching의 hit rate가 12%에 그쳐 매 턴 전체를 재계산(full prefill)하는 상황이 반복된다. 한편 코딩 컨텍스트에는 같은 함수 정의·import 구문이 세션 전반에 걸쳐 반복 등장하는 구조적 패턴이 존재하는데, 기존 prefix caching은 이를 전혀 활용하지 못한다. 결과적으로 멀티턴 세션에서 컨텍스트가 누적될수록 prefill 재계산 비용이 선형 증가하여 TTFT(첫 응답 지연)가 급격히 늘어난다. |
| 사용 기술 | - 에이전트 프레임워크 : OpenHands SDK <br>- Serving layer : vLLM <br>- 모델 : Qwen3-Coder-30B-A3B-FP8, Qwen2.5-Coder-0.5B-Instruct <br>- 타겟 하드웨어 : NVIDIA RTX 5090 × 2장 (VRAM 31.84GB × 2, Linux) <br>- AST 파싱 : Tree-sitter Python 바인딩 (증분 파싱) <br>- 지문 산출 : BLAKE3 해시 (α-rename 정규화 + S-expression 직렬화) <br>- KV Cache 제어 : vLLM block manager 커스터마이징 + RoPE Δ-rotation 모듈 <br>- 벤치마크 : SWE-bench Lite (50 멀티턴 trace, OpenHands 에이전트로 수집) <br>- 평가 지표 : TTFT(ms/턴), AST 서브트리 hit rate(%), Peak KV 메모리(MB)|
| 기대 효과 | - Prefill latency 감소: AST 서브트리 단위 KV Cache 재사용으로 반복 등장하는 코드 블록의 재계산 제거 <br>- 동적 메타정보 문제 해결: tool_call_id·타임스탬프 등으로 인한 prefix 불일치를 우회하여 멀티턴 세션 전반에서 cache hit 유지 <br>- 위치 독립적 재사용: RoPE re-positioning으로 위치가 달라진 서브트리도 KV를 올바르게 재사용 <br>- Long context 환경 대응: 히스토리가 누적되어 컨텍스트 길이가 증가해도 TTFT 선형 증가 억제|
| GitHub Repo | [https://github.com/capstone-2026-ewha/def](https://github.com/capstone-2026-ewha/def) |
| Team Ground Rule | [https://github.com/capstone-2026-ewha/def/blob/main/docs/Team_Ground_Rule.md](https://github.com/capstone-2026-ewha/def/blob/main/docs/Team_Ground_Rule.md) |
| 최종수정일 | 2026-06-01 |

---

<a id="team-15"></a>
## Team 15 햄부기

| 항목 | 내용 |
|------|------|
| 프로젝트명 | 2:4 Structured Sparsity for Faster ViT Inference on Edge Devices: TensorRT Fusion and Speed Bottlenecks |
| 서비스명(브랜드) | |
| 트랙 | 연구 |
| 팀명 | 햄부기 |
| 팀구성 | 신성현, 송영채, 장수연 |
| 팀지도교수 | 심재형 교수님 |
| 무엇을 만들고자 하는가 | 엣지 디바이스(NVIDIA Jetson AGX Orin) 위에서 Vision Transformer(ViT) 계열 모델에 2:4 Structured Sparsity를 적용하고, TensorRT Fusion 병목 현상을 커널 수준에서 분석 및 해결하여 추론 성능을 극대화하는 파이프라인 구축 |
| 고객 (누구를 위해) | Edge AI 기반 비전 서비스를 개발하는 학생 팀 및 제한된 엣지 환경에서 VFM을 구동해야 하는 연구자를 위해 |
| Pain Point (해결할 문제) | 기존 VLM의 비전 인코더는 방대한 파라미터로 인해 엣지 환경에서 추론 속도 병목이 발생한다. 이를 해결하고자 NVIDIA Ampere의 2:4 Structured Sparsity를 적용하려 해도, 실제 TensorRT 엔진 빌드 시 MatMul과 GeLU 레이어가 자동으로 퓨전되면서 Sparse Tensor Core가 제대로 활성화되지 않아 기대한 가속 성능(이론상 2배)에 도달하지 못하는 역설적인 문제가 발생한다. |
| 사용 기술 | **모델 분석 및 변환**<br>- Magnitude 기반 2:4 Pruning: 연속 4개 가중치 중 하위 2개를 0으로 마스킹하여 변환.<br>- QKV Split 최적화: CaiT 모델의 QKV projection을 독립 행렬로 분리하여 Sparsity 활용률 증대.<br><br>**추론 최적화 및 병목 해결**<br>- ONNX Graph Surgery: MatMul 출력 뒤 Identity 노드를 삽입해 TRT Fusion 강제 차단 (Unfused).<br>- Custom Triton Sparse Kernel: MVUE24 알고리즘 기반 커스텀 커널을 직접 구현하여 기댓값 보존.<br>- TensorRT 가속: CUTLASS 백엔드를 강제 사용하여 FP16 기반 엔진 빌드. |
| 개발환경 | 1. Client 디바이스 — PC (Windows) + Jetson AGX Orin (엣지 디바이스)<br>2. FE — 없음<br>3. BE — 없음<br>4. DB — 없음 (실험 결과는 TensorBoard로 시각화)<br>5. 특별한 라이브러리<br>- PyTorch (모델 학습 및 가지치기)<br>- torch.ao (2:4 Sparsity 적용)<br>- TensorRT (Jetson 추론 최적화)<br>- ONNX (모델 변환)<br>- TensorBoard (실험 결과 시각화)<br>6. API Call 서비스 — 없음 |
| 사용하는 소프트웨어 URL | - PyTorch(https://pytorch.org/)<br>- TensorRT(https://developer.nvidia.com/tensorrt)<br>- ONNX(https://onnx.ai/)<br>- NVIDIA Developer(https://developer.nvidia.com/) <br>- Triton(https://triton-lang.org/)|
| 기대 효과 | TensorRT의 자동 레이어 퓨전으로 인해 발생하는 Sparse Tensor Core 미활용 문제를 ONNX Surgery와 커스텀 커널로 직접 우회함으로써, 단순한 모델 경량화를 넘어 이론치에 가까운 실질적인 하드웨어 가속을 달성한다. DeiT, CaiT 등 다양한 비전 모델에 이 일관된 파이프라인을 적용하여, 무거운 VFM을 엣지 환경에서도 병목 없이 실시간으로 구동할 수 있는 핵심 기반을 마련한다. |
| GitHub Repo | [https://github.com/Ewha-Capstone-Project/Hambugy.git](https://github.com/Ewha-Capstone-Project/Hambugy.git) |
| Team Ground Rule | [https://github.com/Ewha-Capstone-Project/Hambugy/blob/main/Team_Ground_Rule.md](https://github.com/Ewha-Capstone-Project/Hambugy/blob/main/Team_Ground_Rule.md) |
| 최종수정일 | 26/06/03 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-16"></a>
## Team 16 퓨터

| 항목 | 내용 |
|------|------|
| 프로젝트명 | 대화 진행에 따라 성격이 변하는 AI 캐릭터와의 정서적 유대감 기반 영어 회화 학습 지속 서비스 |
| 서비스명(브랜드) | CharaShift |
| 트랙 | 산학 |
| 팀명 | 퓨터 |
| 팀구성 | 김민주, 백은혜, 이찬희, 최윤서 |
| 팀지도교수 | 심재형 |
| 무엇을 만들고자 하는가 | 사용자의 발화 스타일을 5축(격식도·에너지·친밀도·유머·탐구심)으로 분석하고, 그 결과를 바탕으로 AI 캐릭터의 성격이 대화마다 실시간으로 변화하는 영어 회화 학습 웹 서비스. 단순 맞춤형 응답이 아니라, 대화가 쌓일수록 캐릭터와의 정서적 유대감이 형성되어 학습을 자연스럽게 지속하게 만드는 것이 핵심 목표 |
| 고객 (누구를 위해) | 영어 회화를 꾸준히 지속하지 못하는 20~30대 중급(B1 이상) 학습자. 기존 앱의 획일적 응답에 흥미를 잃은 사용자 |
| Pain Point (해결할 문제) | 기존 영어 학습 앱은 응답이 고정되어 있어 사용자가 금방 흥미를 잃고 이탈함. AI가 사용자의 말투와 감정을 반영하지 못해 "나에게 맞춘 대화"가 아닌 "정해진 챗봇 응답"처럼 느껴지는 문제 |
| 사용 기술 | GPT-4o, Supabase (Auth · RLS · pgvector), Reddit PRAW, Canvas2D + Superformula, Next.js 14, FastAPI, GitHub Actions |
| 개발환경 | 1. PC (Windows, Mac) 및 Mobile 웹 브라우저<br>2. FE - Next.js 14, Tailwind CSS, Zustand, Canvas2D<br>3. BE - FastAPI (Python)<br>4. DB - Supabase (PostgreSQL · Auth · RLS · pgvector)<br>5. LLM - OpenAI GPT-4o / Embedding - text-embedding-3-small<br>6. 배포 - Vercel (FE), Railway (BE) |
| 사용하는 소프트웨어 URL | 1. Next.js 14: https://nextjs.org<br>2. FastAPI: https://fastapi.tiangolo.com<br>3. Supabase: https://supabase.com<br>4. OpenAI GPT-4o: https://openai.com<br>5. Vercel: https://vercel.com<br>6. Railway: https://railway.app |
| 기대 효과 | AI 캐릭터와의 정서적 유대감 형성으로 학습 지속률 향상 / 발화 스타일 분석 기반 개인화 대화로 몰입도 증가 / 최신 슬랭 RAG 파이프라인으로 실용 영어 학습 |
| GitHub Repo | [https://github.com/puter8/capstone](https://github.com/puter8/capstone) |
| Team Ground Rule | https://github.com/puter8/capstone/blob/main/docs/Team_Ground_Rule.md |
| 최종수정일 | 2026.04.27 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-17"></a>
## Team 17 SPY

| 항목 | 내용 |
|------|------|
| 프로젝트명 | Moni: AI 기반 소비 예측과 맞춤형 챌린지를 결합한 개인화 소비 코칭 서비스 |
| 서비스명(브랜드) | Moni(모니) |
| 트랙 | 산학 |
| 팀명 | SPY |
| 팀구성 | 신희조, 윤수연, 박은수 |
| 팀지도교수 | 오세은 |
| 무엇을 만들고자 하는가 | 본 프로젝트는 사용자의 과거 소비 패턴을 AI가 분석·예측하고, 바로 실천할 수 있는 개인화 챌린지를 제공하는 소비 습관 코칭 앱을 목표로 한다. 카테고리별 지출 예측을 바탕으로 사용자의 소비 목표와 당일 소비 현황을 반영한 데일리 챌린지를 자동 생성하며, 챌린지 달성 시 캐릭터가 성장하는 게임형 보상 구조를 통해 지속적인 행동 변화를 유도한다. |
| 고객 (누구를 위해) | 예산은 있지만 계획적으로 소비하기 어려운 사용자, 소비 습관 개선 필요성을 느끼거나 감정적·충동적 소비를 줄이고 싶은 사용자 |
| Pain Point (해결할 문제) | 많은 사용자는 예산을 설정해도 이를 실제 행동으로 이어가지 못하고, 자신의 소비 패턴을 직관적으로 파악하는 데 어려움을 겪는다. 기존 소비 관리 서비스는 기록과 통계 제공에 머무르는 경우가 많아 지속적인 행동 변화 유도가 부족하다. 소비 습관은 월간 통계가 아니라 오늘의 행동으로 결정되지만, 오늘 어떻게 행동해야 할지 알려주는 도구가 없다. |
| 사용 기술 |  FE: React Native (Expo), TypeScript / BE: FastAPI (Python), SQLModel, JWT 인증 / DB: PostgreSQL / AI: Python 기반 Prophet 시계열 예측 (데이터 부족 시 이동평균 폴백) / 챌린지 생성: 예산 압박도·소비 streak 기반 rule-based 엔진 / 배포: Railway<br>향후 확장 예정 — ARIMA·LSTM 예측 모델 비교 실험, OpenAI GPT API 기반 챌린지 문장 및 주간 리포트 생성 |
| 개발환경 | 1. 언어/런타임: Python 3.10+, TypeScript (Node.js)<br>2. AI/예측: Prophet 1.3, pandas, numpy (Jupyter/Colab 기반 실험)<br>3. Backend: FastAPI 0.136, SQLModel, Uvicorn (ASGI)<br>4. Frontend: React Native (Expo), Expo CLI<br>5. Database: PostgreSQL (psycopg2)<br>6. 배포/인프라: Railway (백엔드 HTTPS)<br>7. 협업: GitHub |
| 사용하는 소프트웨어 URL | FastAPI — https://fastapi.tiangolo.com<br>Prophet (Meta) — https://facebook.github.io/prophet<br>Expo (React Native) — https://expo.dev<br>PostgreSQL — https://www.postgresql.org<br>Railway (배포) — https://railway.app |
| 기대 효과 | 본 서비스는 소비가 발생하기 전에 개입하는 예측 기반 구조를 통해 사용자의 실제 소비 행동 변화를 유도하고, 예산 준수율 및 소비 습관 개선에 기여할 것으로 기대된다. 하루 단위의 챌린지와 보상 시스템으로 단기 실천을, 주간 리포트로 중기 점검을 함께 제공함으로써 사용자 참여도와 지속 사용성을 높인다. |
| GitHub Repo | [https://github.com/SPY-capstone-2026/SPY-capstoneREPO](https://github.com/SPY-capstone-2026/SPY-capstoneREPO) |
| Team Ground Rule | https://github.com/SPY-capstone-2026/SPY-capstoneREPO/blob/main/docs/Team_Ground_Rule.md |
| 최종수정일 | 2026.06.01 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-18"></a>
## Team 18 디바트(deep-art)

| 항목 | 내용 |
| --- | --- |
| 프로젝트명 | 철새 이동 경로 예측 모델과 설명 가능한 AI(XAI)를 사용하여 전시 관람객에게 AI의 추론 과정에 대한 시각적 경험을 제공하는 인터랙티브 미디어아트 설치 작품 |
| 트랙 | 연구 |
| 팀명 | 디바트(deep-art) |
| 팀구성 | 최현서, 이나겸, 김나경 |
| 팀지도교수 | 박현석 |
| 무엇을 만들고자 하는가 | 철새 GPS 데이터를 학습한 AI가 이동 경로를 확률적으로 예측하고, 그 추론 과정을 실시간으로 시각화하는 인터랙티브 미디어아트 설치 작품이다. 영상예술학과 대학원생(영상 연출·시각 디자인 담당)과의 협업 프로젝트로, 본 팀은 기술 구현 전반을 담당한다.<br><br>**[작품 형태]** <br>벽면에 영상을 비추는 설치 작품이다. 관람객은 스마트폰으로 QR을 통해 인터랙션용 웹 UI에 접속해 작품과 상호작용하고, 설치 화면에는 AI가 시뮬레이션한 철새 군집의 이동 장면이 실시간으로 펼쳐진다.<br> **- 시각화 연출**<br>화면에는 크게 두 가지 정보가 표현된다. 첫 번째는 **철새의 예측 경로**로, AI가 예측한 비행 궤적을 따라 철새 무리가 이동한다. 두 번째는 **환경 변수의 기여도**로, 순풍·역풍·대기 불안정도라는 각 환경 변수가 경로 선택에 끼친 영향을 XAI 기법으로 수치화하여 색과 밝기 변화로 표현한다.<br> **- 인터랙티브 요소**<br>관람객은 스마트폰으로 인터랙션용 웹 UI에 들어가, 자신의 바람을 담은 메세지를 철새에게 보낸다. 여러 개의 바람이 모이면, 철새에게 작용되는 환경 변수 중 순풍(날아가는 방향으로 도는 바람)이 강해지고, AI 모델은 앞으로 갈 길을 다시 계산한다. 실시간으로 무리가 새로운 경로를 따라 이동하며, XAI(Explainable AI, 설명 가능한 AI) 연출도 함께 달라진다. <br><br> **[시스템 구조]** <br>철새의 GPS 데이터 및 기후 데이터로 학습한 LSTM이 리더 철새의 경로 예측 → Captum Integrated Gradients로 환경 변수별 기여도 산출 → 위치·경로·XAI 데이터를 FastAPI·WebSocket으로 전송 → Unity에서 철새 군집 연출 및 VFX를 통해 실시간 렌더링 |
| 고객 (누구를 위해) | AI 기술을 사용하지만 그 결과를 맹목적으로 받아들이는 비전공자 전시 관람객 |
| Pain Point (해결할 문제) | AI의 활용이 확대되고 있는 현 사회의 문제 중 하나는, AI가 제시한 결과를 무비판적으로 신뢰하는 태도가 확산되고 있다는 점이다. 결과가 어떤 추론을 통해 도출되었는지에 대한 관심 없이 답의 유용함과 편리함만을 기준으로 받아들이는 경향이 두드러진다.<br><br>설명 가능한 AI(Explainable AI, XAI)는 AI의 판단 근거와 추론 과정을 사용자가 이해할 수 있도록 함으로써, AI에 대한 신뢰를 보다 근거 있게 형성하는 것을 목표로 한다. 이러한 관점에서 볼 때, AI가 제시한 결과를 단순히 수용하기보다 그 결과가 어떠한 과정을 통해 도출되었는지 함께 살펴보는 태도가 중요하다. 그러나 현재의 XAI는 주로 전공자를 위한 복잡한 수치나 그래프 형태로 제공되어 일반 대중이 접근하기 어렵다. 또한 AI의 복잡한 내부 구조는 추론 과정에 대한 이해를 더욱 어렵게 만든다.<br><br>본 작품은 미디어아트 설치를 통해 관람객이 AI의 추론 과정에 대한 관심을 불러 일으키는 것을 목표로 한다. 시각적 연출과 인터랙션으로써 AI의 추론 과정을 들여다보는 진입 장벽을 낮추고자 한다. |
| 사용 기술 | **LSTM** (Long Short-Term Memory): 시계열 GPS·기후 데이터를 학습하여 다음 이동 경로를 예측.<br>**Captum Integrated Gradients**: 각 환경 변수(순풍·역풍·대기 불안정도)가 모델 예측에 기여한 정도를 정량화하는 XAI 기법. <br>**Unity 철새 군집 연출**: 예측 방향을 따르는 리더·추종자 배치로 군집 이동을 표현.<br>**FastAPI·WebSocket**: 관람용 웹 페이지 제공, 서버·Unity 간 실시간 연동.<br>**Unity VFX Graph**: 수천 개의 파티클을 실시간으로 렌더링. |
| 개발 환경 | **OS**: Windows 11 / macOS<br>**Python**: 3.10+<br>**Unity**: 2022 LTS (VFX Graph 패키지)<br>**IDE**: VS Code (Python), Unity Editor (C#) |
| 사용 소프트웨어 URL | **AI / ML**<br>- PyTorch: https://pytorch.org/<br>- Captum: https://captum.ai/<br>- SciPy (Spline): https://scipy.org/<br>**백엔드·배포**<br>- FastAPI: https://fastapi.tiangolo.com/<br>- Railway: https://railway.com/<br>- GitHub Releases : https://docs.github.com/ko/repositories/releasing-projects-on-github/about-releases<br>**렌더링**<br>- Unity VFX Graph: https://docs.unity3d.com/Packages/com.unity.visualeffectgraph@latest |
| 기대 효과 | 첫째, 미디어아트 설치가 관람객의 AI 추론 과정에 대한 관심과 이해 필요성 인식에 미치는 효과를 실증한다. 전시 체험 전후 설문 등을 통해, AI 결과를 무비판적으로 수용하던 태도에서 추론 과정을 질문하는 태도로의 변화를 측정한다.<br>둘째, XAI를 일반 대중에게 다가가게 하는 새로운 방식을 제안한다. 수치·그래프 중심의 기존 설명을 넘어, 시각적 연출과 인터랙션으로 추론 과정을 들여다보는 진입 장벽을 낮추는 표현 방식을 탐구한다.<br>셋째, 본 프로젝트를 기술-예술 융합 사례로서 기록하고 분석한다. 컴퓨터 공학과 영상예술 전공 간 협업 구조 안에서 기술적 구현과 예술적 연출이 어떻게 상호작용하며 설계·기획되었는지를 방법론적으로 정리한다. |
| GitHub Repo  | https://github.com/ewha-deep-art/bird-xai |
| Team Ground Rule | https://github.com/ewha-deep-art/bird-xai/blob/main/docs/Team_Ground_Rule.md |
| 최종수정일 | 2026.06.08 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

<a id="team-19"></a>
## Team 19 Logue

| 항목 | 내용 |
|------|------|
| 프로젝트명 | 자연어 기반 데이터 분석 질의를 통해 조직의 데이터 접근성과 의사결정 속도를 향상시키는 AI 기반 데이터 분석 웹 인터페이스, Logue |
| 서비스명(브랜드) | Logue |
| 트랙 | 산학 |
| 팀명 | Logue |
| 팀구성 | 손하늘, 김겨레, 김예원, 민지인 |
| 팀지도교수 | 하진용 |
| 무엇을 만들고자 하는가 | 자연어 질문만으로 데이터베이스에서 필요한 정보를 조회할 수 있는 데이터 분석 인터페이스 |
| 고객 (누구를 위해) | 데이터 기반 의사결정을 해야 하지만 SQL이나 데이터 조회가 어려운 기획자·마케터 |
| Pain Point (해결할 문제) | 비즈니스 데이터를 확인할 때 개발자에게 쿼리를 요청해야 하는 의존성과 분석 지연 문제를 해결 |
| 사용 기술 | LLM 기반 Text-to-SQL, 데이터베이스 스키마 이해, 자연어 질의 처리 기술을 사용 |
| 개발환경 | Device : PC(Window)<br>FE<br>- Next.js<br>- Typescript<br>- Vite<br>- yarn<br>- Axios<br>- Tailwindcss v4.2<br>- StoryBook<br>- Zustand<br>- Tanstack Query<br>- React Hook form + Zod<br>- shadcn/ui (ui  컴포넌트)<br>- ECharts<br>- Monaco Editor(필요시)<br>- Vercel or Jenkins<br><br>BE<br>- Java 21, Spring Boot 3<br>- Spring AOP<br>- PostgreSQL<br>- AWS RDS<br>- AWS S3<br>- Redis<br>- Flyway<br>- Github Actions<br>- Docker<br>- Kubernetes<br>- AWS ec2, Route53, ALB<br>- AWS CloudWatch<br>- Sentry<br>- Slf4j, Logback<br>- Spring Security<br>- OAuth2.0<br>- JWT<br>- Swagger<br>- k6, p6spy<br><br>AI<br>- Python<br>- FastAPI<br>- Pydantic v2<br>- pandas<br>- sentence-transformers<br>- OpenAI API<br>- Uvicorn<br>- pytest<br>- Render<br>- GitHub Actions
| 사용하는 소프트웨어 URL | Device : PC(Window)<br>FE<br>- Next.js<br>- Typescript<br>- Vite<br>- yarn<br>- Axios<br>- Tailwindcss v4.2<br>- StoryBook<br>- Zustand<br>- Tanstack Query<br>- React Hook form + Zod<br>- shadcn/ui (ui  컴포넌트)<br>- ECharts<br>- Monaco Editor(필요시)<br>- Vercel or Jenkins<br><br>BE<br>- Java 21, Spring Boot 3<br>- Spring AOP<br>- PostgreSQL<br>- AWS RDS<br>- AWS S3<br>- Redis<br>- Flyway<br>- Github Actions<br>- Docker<br>- Kubernetes<br>- AWS ec2, Route53, ALB<br>- AWS CloudWatch<br>- Sentry<br>- Slf4j, Logback<br>- Spring Security<br>- OAuth2.0<br>- JWT<br>- Swagger<br>- k6, p6spy<br><br>AI<br>- Python<br>- FastAPI<br>- Pydantic v2<br>- pandas<br>- sentence-transformers<br>- OpenAI API<br>- Uvicorn<br>- pytest<br>- Render<br>- GitHub Actions
| 기대 효과 | 비개발자도 즉시 데이터를 탐색하고 빠르게 의사결정을 내릴 수 있게 됨. |
| GitHub Repo | [https://github.com/26-ewha-capstone-logue](https://github.com/26-ewha-capstone-logue/logue) |
| Team Ground Rule | [Team_Ground_Rule](https://github.com/26-ewha-capstone-logue/docs/blob/main/Team_Ground_Rule.md) |
| 최종수정일 | 2026.03.16 |

[↑ 목록으로](#2026-spring-전체-프로젝트-리스트)

---

