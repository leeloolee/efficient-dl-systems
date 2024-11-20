# 효율적인 딥러닝 시스템
이 저장소는 [HSE 대학교](https://www.hse.ru/en/)의 [컴퓨터 과학 학부](https://cs.hse.ru/en/)와 [Yandex 데이터 분석 학교](https://academy.yandex.com/dataschool/)에서 진행되는 **효율적인 딥러닝 시스템(Efficient Deep Learning Systems)** 강좌의 자료를 포함하고 있습니다.

__이 브랜치는 진행 중인 2024년도 강좌에 해당합니다. 이전 연도의 전체 자료를 보려면 ["Past versions"](https://github.com/mryab/efficient-dl-systems/tree/2023) 섹션을 참조하세요.__

---

## 강의 계획
- [__1주차:__](./week01_intro) __소개__
  - **강의**: 강좌 개요 및 운영 세부 사항. GPU 아키텍처 및 CUDA API의 핵심 개념.
  - **세미나**: PyTorch에서 CUDA 연산. 벤치마킹 소개.
- [__2주차:__](./week02_management_and_testing) __실험 관리, 모델 및 데이터 버전 관리, Python에서 딥러닝 코드 테스트__
  - **강의**: 실험 관리 기초 및 파이프라인 버전 관리. Python 애플리케이션 구성. 정규 및 속성 기반 테스트 소개.
  - **세미나**: DVC와 Weights & Biases 프로젝트 예제 살펴보기. pytest를 활용한 테스트 소개.
- [__3주차:__](./week03_fast_pipelines) __훈련 최적화 및 딥러닝 코드 프로파일링__
  - **강의**: 혼합 정밀 훈련(Mixed-Precision Training). 데이터 저장 및 로딩 최적화. 딥러닝 워크로드 프로파일링 도구.
  - **세미나**: PyTorch에서 자동 혼합 정밀도 구현. 시퀀스 데이터 동적 패딩 및 JPEG 디코딩 벤치마크. py-spy, PyTorch Profiler, PyTorch TensorBoard Profiler, nvprof, Nsight Systems를 활용한 프로파일링 기초.
- [__4주차:__](./week04_distributed) __분산 머신러닝 기초__
  - **강의**: 분산 훈련 소개. 프로세스 기반 통신. 매개변수 서버(Parameter Server) 아키텍처.
  - **세미나**: 멀티프로세싱 기초. 병렬 GloVe 훈련.
- [__5주차:__](./week05_data_parallel) __데이터 병렬 훈련 및 All-Reduce__
  - **강의**: 신경망의 데이터 병렬 훈련. All-Reduce 및 그 효율적인 구현.
  - **세미나**: PyTorch Distributed 소개. 데이터 병렬 훈련 기본 연산.
- [__6주차:__](./week06_large_models) __대규모 모델 훈련__
  - **강의**: 모델 병렬 처리, 그래디언트 체크포인팅, 오프로딩(offloading), 셰이딩(sharding).
  - **세미나**: 그래디언트 체크포인팅 및 텐서 병렬 처리 실습.
- [__7주차:__](./week07_application_deployment) __Python 웹 애플리케이션 배포__
  - **강의/세미나**: 프로덕션 수준의 웹 서비스 구축 및 배포. 애플리케이션 및 웹 서버, Docker, Prometheus, HTTP 및 gRPC를 통한 API.
- [__8주차:__](./week08_inference_software) __LLM 추론 최적화 및 소프트웨어__
  - **강의**: 추론 속도 지표. KV 캐싱, 배치 추론, 연속 배칭. FlashAttention과 그 수정 버전, PagedAttention. 주요 LLM 서빙 프레임워크 개요.
  - **세미나**: Triton 언어 기초. PyTorch 및 Triton에서의 레이어 병합(fusion). KV 캐싱 및 FlashAttention 구현 실습.
- [__9주차:__](./week09_compression) __효율적인 모델 추론__
  - **강의**: 딥러닝을 위한 하드웨어 활용 지표. 지식 증류(Knowledge Distillation), 양자화(Quantization), LLM.int8(), SmoothQuant, GPTQ. 효율적인 모델 아키텍처. 추측 디코딩(Speculative Decoding).
  - **세미나**: 메모리 대역폭 활용 측정 실습. 데이터 비의존 양자화(Data-free Quantization), GPTQ, SmoothQuant을 PyTorch에서 구현.
- __10주차:__ __게스트 강연__

---

## 평가 방식
여러 과제가 진행되며, 다음과 같은 주제를 다룹니다:
- 훈련 파이프라인 및 코드 프로파일링
- 분산 및 메모리 효율적인 훈련
- 프로덕션 모델 배포 및 최적화

최종 점수는 각 과제 점수의 가중 합으로 계산됩니다. 세부 사항은 각 기관의 강좌 페이지를 참조하세요.

---

## 강사진
- [Max Ryabinin](https://github.com/mryab)
- [Just Heuristic](https://github.com/justheuristic)
- [Alexander Markovich](https://github.com/markovka17)
- [Anton Chigin](https://github.com/achigin)
- [Ruslan Khaidurov](https://github.com/newokaerinasai)

---

## 이전 버전
- [2023](https://github.com/mryab/efficient-dl-systems/tree/2023)
- [2022](https://github.com/mryab/efficient-dl-systems/tree/2022)
- [2021](https://github.com/yandexdataschool/dlatscale_draft)
