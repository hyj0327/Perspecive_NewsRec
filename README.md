# Perspecive_NewsRec


## 프로젝트 개요

### 문제 인식 : 확증 편향
  - 사람은 자신의 의견과 일치하는 정보는 더 믿고 더 찾아보려 한다. (자신의 신념을 확인하려는 경향이 있다.)
    - 그러나 자신이 이미 알던 것과 다른 내용은 무시하거나 찾으려 하지 않는다.
    - 확증 편향이 심화되며 사회 계층 양극화를 비롯한 각종 사회 문제가 야기되기까지 한다.
  - 확증 편향을 완벽히 없앨 수는 없지만, "완화" 할 수는 있다.
    - 확증 편향으로 인한 의도적 합리화에 빠지게 되더라도 동일한 반대 관점에 지속적으로 노출되면 결국 '티핑 포인트'에 이르러 신념이 바뀔 수 있다. ([David Redlawsk et al, "The Affective Tipping Point: Do Motivated Reasoners Ever 'Get It'?"](https://edisciplinas.usp.br/pluginfile.php/4912780/mod_resource/content/1/BACKFIRE_TIPPING_POINT_redlawsk2010.pdf))

### 프로젝트 목표
- 이슈성 정보를 다루는 뉴스에서 기존 관점 다른 관점을 제공해 주어 확증 편향을 완화
- 비판적인 사고력과 자기 객관화 능력 및 정보 분별력 등의 능력 신장에 도움을 주는 프로그램 구축을 목표로 함.

### 왜 "뉴스"인가?

- "글" 로 정보를 전달하는 매체.
  - 실시간, 최신의 쟁점성 정보들이 제공된다.
- 기사 전문을 읽어 맥락을 파악하는 것과 기사 요약본, 제목만 읽고 맥락을 파악하는 점은 다르다

### 파이프라인

![image](https://github.com/deepshadow25/Perspecive_NewsRec/assets/115054681/7d61dc8c-aec6-43bd-9326-52866501da37)


## 데이터 설명

- 네이버 뉴스 크롤링 수집 코드
  - 매일 22시마다 기사 자동 수집
- 사용하는 요소 : 기사제목, 기사링크, 기사본문
  - 수집한 기사 본문 바탕으로 요약문장 뽑아내기.
  - 언론사 정보도 수집하지만, 전처리에만 이용하고 삭제함.

[상세 데이터 설명](https://github.com/deepshadow25/Perspecive_NewsRec/blob/main/Dataset/dataset.md)


## 모델 설명

### 임베딩 및 문서 요약 모델

- KPFBERT 임베딩


### 뉴스 추천 모델

클러스터링을 통해 뉴스

