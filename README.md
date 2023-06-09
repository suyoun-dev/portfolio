# Suyoun's porftolio

---

# 👩🏻‍💻 **About Me**

💡 **언어학 기반 데이터 분석가 -** **언어학을 기반으로 기계가 학습하기 어려운 복잡한 언어의 문장 구조를 분석하여 특징을 도출해 언어 모델 성능 개선이 목표입니다.**

## ☎️ Contact.

📧 **E-mail : mingk968@gmail.com**

📲 **Phone : 010-7761-8474**

**📡 Github : [https://github.com/suyoun-dev](https://github.com/suyoun-dev)**

## 🏫 Education

**성신여자대학교**

2015.03 ~ 2020.02 (졸업)

주전공 - 영어영문학과

부전공 - IT학부 정보시스템학과

GPA: 3.91/4.5

## 

**한국외국어대학교 일반대학원**

2020.03 ~ 2022.02 (수료)

전공 - 영어학과 전산언어학

GPA: 4.18/4.5

# 💻Skills
<p align="center" display="inline-block">
    <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=Python&logoColor=white">
    <img src="https://img.shields.io/badge/Pytorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white">
 <br>
  <img src="https://img.shields.io/badge/JAVA-007396?style=for-the-badge&logo=java&logoColor=white"> 
  <img src="https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=Spring&logoColor=white">
  <img src="https://img.shields.io/badge/Javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
  <img src="https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=oracle&logoColor=black">
  <img src="https://img.shields.io/badge/Css-1572B6?style=for-the-badge&logo=css3&logoColor=white"><br>
  <img src="https://img.shields.io/badge/Html-E34F26?style=for-the-badge&logo=html5&logoColor=white">
  <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=Amazon AWS&logoColor=white">
  <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=Linux&logoColor=white">
  <img src="https://img.shields.io/badge/SpringBoot-6DB33F?style=for-the-badge&logo=SpringBoot&logoColor=white">
 <br>
    <img src="https://img.shields.io/badge/Github-181717?style=for-the-badge&logo=github&logoColor=white"> 
</p>

# 🗂️Projects

### 트위터 크롤링 데이터 기반 비교문화 분석

**[Public’s appraisal of a wrongdoer from a cultural perspective : 
BERTopic, Semantic network analysis of Twitter in the United States and South Korea]**

**2022.09.03~2023. **
- **사용 언어** : Python
- **데이터 수집 및 전처리**
- **사용 모델**
    → Bertopic, Netminer


### 트위터 크롤링 데이터 기반 감정분석

**[2022 대선 감정분석 - 주요 키워드를 중심으로](https://www.notion.so/2022-15b17d7c38c2412ab0c008b04f17912d)** 

**2022.03.20~2022.05.24**

- **사용 언어** : Python
- **작업툴** : Visual Studio Code, Google Colabatory
- **인원** : 5명
- **데이터 전처리 및 시각화**
    
    → Mecab, Matplotlib, Seaborn, Pandas, Numpy
    
- **딥러닝**
    
    → HuggingFace, Pytorch
    
- **감정분석 모델 및 파인튜닝 **
    
    → KcBERT, [**Korean UnSmile Dataset**](https://github.com/smilegate-ai/korean_unsmile_dataset#korean-unsmile-dataset)
    
<details>
<summary>프로젝트 요약</summary>

**[개요]**

- 140자 내로 다양한 의견을 자유롭게 표현하는 소셜 네트워크 서비스인 트위터에 대선 관련 주요 키워드(예: 윤석열, 이재명, 소신투표 등)을 검색하여 나오는 데이터를 크롤링하여 각 키워드에 대한 여론 조사 및 감정 분포도를 조사하고자 진행.
 
**[역할]**

- 키워드 **윤석열, ㅇㅅㅇ, ㅇㅈㅁ, 소신투표**에 대한 크롤링, 전처리, 감정분석 후 시각화
- 스마일게이트 AI에서 공개한 한국어 혐오 데이터셋을 이용한 혐오감정분류 모델 사용 제안 및 적용
- 맡은 키워드에 대한 인사이트 도출 및 정리

**[과정]**

- 대선 후보 등록 시기부터 대선 당일 전까지(2월 8일~3월8일) 약 한달 간의 데이터를 크롤링하여 진행. 데이터가 너무 많은 키워드(예: 윤석열, 이재명)은 하루당 1000개씩 랜덤으로 추출하여 감정분석을 진행.
    
    **1) 데이터 전처리 :** 트위터 특성 상 멘션(@아이디), 리트윗(rt, RT, 알티 등)을 정규표현식을 사용하여 전처리함. 해당 기간 동안의 트렌드를 분석하기 위해 해시태그(#키워드)는 유지.
    
    **2) 감정 분석 :** HuggingFace에서 영화 리뷰 데이터로 사전학습된 감정분석 모델 kcbert를 불러와 파인튜닝을 한 후 감정분석을 진행. 부정 레이블이 상당히 많아 이에 대해 더 분석하고자 스마일게이트의 혐오 감정 데이터셋 Unsmiledataset을 사용하여 혐오 감정 분석을 진행. 다중감정분류(기쁨, 슬픔, 분노, 즐거움 등)도 진행을 했으나 다소 정확성이 떨어져 생략하기로 결정.
    
    **3) 데이터 분석 및 시각화 :** 전체 기간, 주차별, 일별로 가장 빈도수가 높은 단어들의 분포도와 워드클라우드를 만들어 사건 및 키워드 분석 진행.
    

**[인사이트]**

- 프로젝트 초기 목적은 소셜네트워크 상에서 대선 후보 및 공약에 대한 유저들의 다양한 의견을 분석하고 어떤 흐름인지 분석하고자 했다. 하지만 분석 결과, 공약에 대한 의견보다는 혐오를 기반으로 본인이 지지하지 않는 후보들에 대한 비방 목적의 트윗이 주를 이뤘다. 또한 정확한 이름이 아닌 초성으로 후보를 지칭하는 경우 대부분은 모욕적인 발언을 담고 있었다.
- 정답이 없는 주제에 대해서는 누가 맞고 틀리다라는 것 또한 없다. 하지만 이번 대선에 관련해서는 서로 본인의 의견이 맞다고만 주장하고 본인과 다른 의견은 옳지 않다고 무시하는 경향이 많이 보였다. 단순히 무시가 아닌 혐오 단어를 사용하며 부정적인 감정을 표출하고 있다.

**[한계점 및 개선사항]**

- 모든 트위터 데이터가 부정적인 감정을 갖고 있지 않으나, 아직까지는 문장에 부정적인 단어가 많은지, 긍정적인 단어가 많은지로 해당 데이터에 대한 감정이 결정되는 것으로 보임. 
-  그러나 한 트윗에 A에 대한 긍정적인 의견이 있는 것과 동시에 B에 대한 부정적인 의견이 같이 있을 수 있음.
-  이 때 나오는 감정 분석의 결과는 어떤 대상에 대한 감정인지 분류하기 어려움.
-  일반적인 상품 리뷰에서는 Aspect-based 감정분석이 많이 쓰이고 있으며, 이는 배터리, 음질 등 핸드폰의 특징을 기준으로 다양한 양상에서 좋고 나쁨을 가를 수 있음.
-  지금은 불규칙적인 문법과 새로 나오는 각종 신조어 등을 사용하는 소셜네트워크에서는 문장 안의 각 요소에 대한 감정분석이 어려울 수 있으나 추후 이런 세세한 부분까지 분석이 가능할 수 있도록 언어 모델을 개선하는 것이 목표임.
</details>

---

### **2020년 인공지능 학습용 데이터 구축(2차) 사업 - 한국지능정보사회진흥원**

**2020.09.26~2021.02.28**

### **[한국외국어대학교 영어학과 연구과제 연구 보조원 - 일반 외래어 스크립트 작성]**
- **사용언어** : Python
- **작업툴** : Visual Studio Code, Excel
- 인원: 11명
- 내용:
    - 국립 국어원에 등록된 외래어를 크롤링하여 외래어 리스트 생성
    - 각 단어마다 중분류(유래어), 소분류(전문 분야), 한글(원어)로 분류
    - 아래의 규칙에 맞게 스크립트 작성
        - 스크립트 1개당 발화 길이 -> 약 3초 내외 (15~20 문자)
        - 1개 단어당 3개 스크립트 작성
        - 구어체 / 평서문 또는 의문문 / 두 개 이상 외래어 조합 가능 / 외래어와 의미가 통하는 자연스러운 문장
        - 단어는 최대한 문장 중간에 있을 수 있도록 작성(발화할 때 단어 앞뒤의 어두, 어미에 따라 발음이 달라질 수 있기 때문)
    - 스크립트 작성 후 1차 검수

---
### **영화 통합 정보 사이트 - TMI 프로젝트**
`2019.05~2019.10`
 TMI 프로젝트를 진행. 주요 기능으로 위치기반 지역별 통합시간표, 영화 정보 열람 및 검색, 영화 정보 공유 커뮤니티 제공을 구축함. 로그인, 회원가입, 아이디, 비밀번호 찾기, 메인 페이지, 영화목록, 영화 상세 페이지, 마이페이지, 레이아웃 디자인 및 기능 구현 등 전체적인 프론트 엔드 구현과 회원 관리 데이터베이스를 구축하여 화면과 연동

# 💼Careers
`2022.08~` 한국외국어대학교 데이터센터 수집 및 분석 연구원<br>
`2020.09.01~2022.02.28` 한국외국어대학교 언어공학연구소 조교<br>
[연구소 행정 업무]
- 연구소 운영비, 연구소활성화지원금, 인건비 정산 및 관리
- 회의 진행 및 회의록 작성
- 연구소 장비(프로그램, 장비 등) 대여, 정비, 관리
- 연구소 소유 데이터 관리(NAS, LDC 등)
- 녹음실 관리 및 필요 시 음성 데이터 녹음 보조
- 연구소 홈페이지 관리<br>

[AI융합전공(Language&AI트랙)학과 행정 업무]
- 학과 운영비 정산 및 관리
- 학생 질의 응답
- 수강신청(교과목 개설, 강의시간표 배정, 강의실 배정 등) 업무
- 학과 학사 일정 조정 및 관리(학점인정, 졸업시험, 졸업사정, 현장실습 인턴십 등)
- 그 외 학과 업무<br>

`2020.03.02~2020.08.31` 한국외국어대학교 대학원 교학처 행정 조교<br>
[대학원 교학처 업무 전반 보조]
- 전화 응대
- 외국어시험, 종합시험 보조(감독, 시험 준비 등)
- 강의실 대여 및 배정
- 우편 전달 및 발송
- 입시 일정 보조(서류 관리, 일정 안내 등) <br>

`2020.03.20~2020.12.21`
`2017.09.04~2018.05.29` 한국저작권위원회 등록임치팀 / 사무보조 아르바이트<br>
[등록임치팀 사무보조]<br>
- 우편 업무
    - 전날 등록 완료된 건 데이터 정리(등록증, 사본교부, 재교부, 보완, 반려, 취하, 말소 등)
    - 출력 후 우편 봉투 작업 후 우편 발송
- 복제물 작업 및 검수
    - 신청서류, 복제물 분류 및 바코드 작업 후 복제물 보관실에 보관
    - 정기적으로 복제물 검수(복제물 상태 및 정확한 위치에 보관 여부) 후 본사로 발송
- 복제물 복제
    - 필요시 받은 복제물을 CD로 복제하여 보관
- 기타 사무보조 업무

# 🪂Activities
|활동명|Type|활동기간|활동내용|
|------------|--|---|----------|
|JAVA기반 빅데이터 IT콘텐츠 정보시스템 취업과정|교육|`2019.05.04~2019.10.10`|JAVA, 데이터베이스, 화면구현, JSP, Servlet, R studio, Python 위주의 교육과정을 통해 IT/SW분야 직무 이해 및 프로그래밍 언어 활용법을 학습. - 배운 것을 바탕으로 영화 통합 정보 사이트 TMI 프로젝트를 진행. 주요 기능으로 위치기반 지역별 통합시간표, 영화 정보 열람 및 검색, 영화 정보 공유 커뮤니티 제공을 구축함. 로그인, 회원가입, 아이디, 비밀번호 찾기, 메인 페이지, 영화목록, 영화 상세 페이지, 마이페이지, 레이아웃 디자인 및 기능 구현 등 전체적인 프론트 엔드 구현과 회원 관리 데이터베이스를 구축하여 화면과 연동.|


# 📜Certificates

[제목 없음](%E1%84%8B%E1%85%A9%E1%84%89%E1%85%AE%E1%84%8B%E1%85%A7%E1%86%AB(OH%20SUYOUN)%20(1)%203834118249114d24a7c3d4a8db60a9bc/%E1%84%8C%E1%85%A6%E1%84%86%E1%85%A9%E1%86%A8%20%E1%84%8B%E1%85%A5%E1%86%B9%E1%84%82%E1%85%B3%E1%86%AB%20%E1%84%83%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%90%E1%85%A5%E1%84%87%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%89%E1%85%B3%2053d486d0ead84049b65169f0dc9f5348.md)

# 🏆Awards

[제목 없음](%E1%84%8B%E1%85%A9%E1%84%89%E1%85%AE%E1%84%8B%E1%85%A7%E1%86%AB(OH%20SUYOUN)%20(1)%203834118249114d24a7c3d4a8db60a9bc/%E1%84%8C%E1%85%A6%E1%84%86%E1%85%A9%E1%86%A8%20%E1%84%8B%E1%85%A5%E1%86%B9%E1%84%82%E1%85%B3%E1%86%AB%20%E1%84%83%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%90%E1%85%A5%E1%84%87%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%89%E1%85%B3%20a826306d17b94ff2a997f689b99d9fed.md)
