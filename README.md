# Suyoun's porftolio
# 오수연(OH SUYOUN) (1)

---

<aside>
👩🏻‍💻 **About Me**

</aside>

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

[제목 없음](%E1%84%8B%E1%85%A9%E1%84%89%E1%85%AE%E1%84%8B%E1%85%A7%E1%86%AB(OH%20SUYOUN)%20(1)%203834118249114d24a7c3d4a8db60a9bc/%E1%84%8C%E1%85%A6%E1%84%86%E1%85%A9%E1%86%A8%20%E1%84%8B%E1%85%A5%E1%86%B9%E1%84%82%E1%85%B3%E1%86%AB%20%E1%84%83%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%90%E1%85%A5%E1%84%87%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%89%E1%85%B3%202e0a735f02104e0c89cbb4fe3e5142cb.md)

# 🗂️Projects

### 트위터 크롤링 데이터 기반 감정분석

**[2022 대선 감정분석 - 주요 키워드를 중심으로](https://www.notion.so/2022-15b17d7c38c2412ab0c008b04f17912d)** 

**2022.03.20~2022.05.24**

- **사용 언어** : Python
- **데이터 전처리 및 시각화**
    
    → Mecab, Matplotlib, Seaborn, Pandas, Numpy
    
- **머신러닝**
    
    → HuggingFace, Pytorch
    
- **감정분석 모델**
    
    → KcBERT, [**Korean UnSmile Dataset**](https://github.com/smilegate-ai/korean_unsmile_dataset#korean-unsmile-dataset)
    

### [2022 대선 감정분석 - 주요 키워드를 중심으로]

**[개요]**

- 130자 내로 다양한 의견을 자유롭게 표현하는 소셜 네트워크 서비스인 트위터에 대선 관련 주요 키워드(예: 윤석열, 이재명, 소신투표 등)을 검색하여 나오는 데이터를 크롤링하여 각 키워드에 대한 여론 조사 및 감정 분포도를 조사하고자 진행.

**[역할]**

- 키워드 **윤석열, ㅇㅅㅇ, ㅇㅈㅁ, 소신투표**에 대한 크롤링, 전처리, 감정분석 후 시각화
- 스마일게이트 AI에서 공개한 한국어 혐오 데이터셋을 이용한 혐오감정분류 모델 사용 제안 및 적용
- 맡은 키워드에 대한 인사이트 도출 및 정리

**[과정]**

- 대선 후보 등록 시기부터 대선 당일 전까지(2월 8일~3월8일) 약 한달 간의 데이터를 크롤링하여 진행. 데이터가 너무 많은 키워드(예: 윤석열, 이재명)은 하루당 1000개씩 랜덤으로 추출하여 감정분석을 진행하기로 함.
    
    **1) 데이터 전처리 :** 트위터 특성 상 멘션(@아이디), 리트윗(rt, RT, 알티 등)을 정규표현식을 사용하여 전처리함. 해당 기간 동안의 트렌드를 분석하기 위해 해시태그(#키워드)는 유지.
    
    **2) 감정 분석 :** HuggingFace에서 영화 리뷰 데이터로 사전학습된 감정분석 모델 kcbert를 불러와 파인튜닝을 한 후 감정분석을 진행. 부정 레이블이 상당히 많아 이에 대해 더 분석하고자 스마일게이트의 혐오 감정 데이터셋 Unsmiledataset을 사용하여 혐오 감정 분석을 진행. 다중감정분류(기쁨, 슬픔, 분노, 즐거움 등)도 진행을 했으나 다소 정확성이 떨어져 생략하기로 결정.
    
    **3) 데이터 분석 및 시각화 :** 전체 기간, 주차별, 일별로 가장 빈도수가 높은 단어들의 분포도와 워드클라우드를 만들어 사건 및 키워드 분석 진행.
    

**[인사이트]**

- 프로젝트 초기 목적은 소셜네트워크 상에서 대선 후보 및 공약에 대한 유저들의 다양한 의견을 분석하고 어떤 흐름인지 분석하고자 했다. 하지만 분석 결과, 공약에 대한 의견보다는 혐오를 기반으로 본인이 지지하지 않는 후보들에 대한 비방 목적의 트윗이 주를 이뤘다. 또한 정확한 이름이 아닌 초성으로 후보를 지칭하는 경우 대부분은 모욕적인 발언을 담고 있었다.
- 정답이 없는 주제에 대해서는 누가 맞고 틀리다라는 것 또한 없다. 하지만 이번 대선에 관련해서는 서로 본인의 의견이 맞다고만 주장하고 본인과 다른 의견은 옳지 않다고 무시하는 경향이 많이 보였다. 단순히 무시가 아닌 혐오 단어를 사용하며 부정적인 감정을 표출하고 있다.

**[한계점 및 개선사항]**

- 모든 트위터 데이터가 부정적인 감정을 갖고 있지는 않을 것이다. 다만 아직까지는 문장에 부정적인 단어가 많은지, 긍정적인 단어가 많은지로 데이터에 대한 감정이 분류가 되는 것 같다. 왜냐하면 한 트윗에 A에 대한 긍정적인 의견도 있지만 이와 함께 B에 대한 부정적인 의견이 같이 있을 수도 있으며, 이 때 나오는 감정 분석의 결과는 어떤 대상에 대한 감정인지 분류하기 어렵다.
- 리뷰에서는 Aspect-based 감정분석이 많이 쓰이고 있으며, 이는 배터리, 음질 등 핸드폰의 특징을 기준으로 다양한 양상에서 좋고 나쁨을 가를 수 있다. 지금은 불규칙적인 문법과 새로 나오는 각종 신조어 등을 사용하는 소셜네트워크에서는 문장 안의 각 요소에 대한 감정분석이 어려울 수 있으나 추후 이런 세세한 부분까지 분석이 가능할 수 있도록 언어 모델을 개선시키고 싶다.

---

### **2020년 인공지능 학습용 데이터 구축(2차) 사업 - 한국지능정보사회진흥원**

**2020.09.26~2021.02.28**

### **[한국외국어대학교 영어학과 연구과제 연구 보조원 - 일반 외래어 스크립트 작성]**

- 국립 국어원에 등록된 외래어를 크롤링하여 외래어 리스트 생성
- 각 단어마다 중분류(유래어), 소분류(전문 분야), 한글(원어)로 분류
- 아래의 규칙에 맞게 스크립트 작성
    - 스크립트 1개당 발화 길이 -> 약 3초 내외 (15~20 문자)
    - 1개 단어당 3개 스크립트 작성
    - 구어체 / 평서문 또는 의문문 / 두 개 이상 외래어 조합 가능 / 외래어와 의미가 통하는 자연스러운 문장
    - 단어는 최대한 문장 중간에 있을 수 있도록 작성(발화할 때 단어 앞뒤의 어두, 어미에 따라 발음이 달라질 수 있기 때문)
- 스크립트 작성 후 1차 검수

---

# 💼Careers

[제목 없음](%E1%84%8B%E1%85%A9%E1%84%89%E1%85%AE%E1%84%8B%E1%85%A7%E1%86%AB(OH%20SUYOUN)%20(1)%203834118249114d24a7c3d4a8db60a9bc/%E1%84%8C%E1%85%A6%E1%84%86%E1%85%A9%E1%86%A8%20%E1%84%8B%E1%85%A5%E1%86%B9%E1%84%82%E1%85%B3%E1%86%AB%20%E1%84%83%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%90%E1%85%A5%E1%84%87%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%89%E1%85%B3%20e668999c0afe4a38bd82a19d4937a658.md)

# 🪂Activities

[제목 없음](%E1%84%8B%E1%85%A9%E1%84%89%E1%85%AE%E1%84%8B%E1%85%A7%E1%86%AB(OH%20SUYOUN)%20(1)%203834118249114d24a7c3d4a8db60a9bc/%E1%84%8C%E1%85%A6%E1%84%86%E1%85%A9%E1%86%A8%20%E1%84%8B%E1%85%A5%E1%86%B9%E1%84%82%E1%85%B3%E1%86%AB%20%E1%84%83%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%90%E1%85%A5%E1%84%87%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%89%E1%85%B3%20d5b61e61c38440f78ba090465009fa9f.md)

# 📜Certificates

[제목 없음](%E1%84%8B%E1%85%A9%E1%84%89%E1%85%AE%E1%84%8B%E1%85%A7%E1%86%AB(OH%20SUYOUN)%20(1)%203834118249114d24a7c3d4a8db60a9bc/%E1%84%8C%E1%85%A6%E1%84%86%E1%85%A9%E1%86%A8%20%E1%84%8B%E1%85%A5%E1%86%B9%E1%84%82%E1%85%B3%E1%86%AB%20%E1%84%83%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%90%E1%85%A5%E1%84%87%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%89%E1%85%B3%2053d486d0ead84049b65169f0dc9f5348.md)

# 🏆Awards

[제목 없음](%E1%84%8B%E1%85%A9%E1%84%89%E1%85%AE%E1%84%8B%E1%85%A7%E1%86%AB(OH%20SUYOUN)%20(1)%203834118249114d24a7c3d4a8db60a9bc/%E1%84%8C%E1%85%A6%E1%84%86%E1%85%A9%E1%86%A8%20%E1%84%8B%E1%85%A5%E1%86%B9%E1%84%82%E1%85%B3%E1%86%AB%20%E1%84%83%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%90%E1%85%A5%E1%84%87%E1%85%A6%E1%84%8B%E1%85%B5%E1%84%89%E1%85%B3%20a826306d17b94ff2a997f689b99d9fed.md)
