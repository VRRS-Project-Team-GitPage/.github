# 채식 어디

### 📖 프로젝트 정보
> **프로젝트 명**
> 
> 
> *채식 유형에 따른 공산품의 섭취 여부 판독 및 데이터 기반 제품 추천 서비스(채식 어디)*
> 
- 개발 기간: 2024년 03월 ~ 2024년 11월 (총 9개월)
- 신한대학교 SW 졸업 프로젝트

---

### 💬 프로젝트 아이디어 및 배경
최근 건강과 채식에 대한 관심이 증가하면서 국내 채식 인구는 꾸준히 증가하는 추세입니다.
하지만 채식주의자들은 여전히 식생활에서 어려움을 겪고 있습니다.
이는 
- 채식 제품에 관한 정보 및 서비스 부족
  - 한국 채식 서비스 시장의 저조함
- 대체 식품의 높은 가격
- 다양한 채식주의자 유형에 비해 비건 중심의 한정적인 서비스

가 주요 원인입니다.
이를 해결하기 위해 채식주의자들이 다양한 제품 정보를 쉽게 찾을 수 있는 서비스를 제공하고자 합니다.

비건뿐 아니라 채식주의자 전체를 아우르는 정보를 통해 편리한 식생활을 지원하는 플랫폼을 구축합니다.

---

### 시스템 구성도
![image](https://github.com/user-attachments/assets/68c854fe-e8e2-4386-b334-58acac83e966)

---

### 시스템 개발 기술
**1) React Native**

버전: 0.76

기술 개요 및 특징:

크로스 플랫폼 모바일 앱 개발을 지원하는 프레임워크로 JavaScript와 React를 기반으로 ios와 android 모두 실행되는 앱을 개발할 수 있다. 
React는 큰 커뮤니티와 다양한 라이브러리가 있어 많은 기능을 구현하기 쉬운 것이 특징이다.
최대한 다양한 채식주의자가 사용함을 목표로 하기에 ios와 android에서 모두 활용 가능하고, 개발 기간 단축과 비용 절감을 할 수 있어 선택하였다.

활용: 
- 기존 기술 개선: Figma에서 디자인한 UX/UI을 React Native로 재구성하였고 모바일에서 최적화된 디자인을 구현했다.
- 기술 적용 후 서비스 구현: ios와 android, 크로스 플랫폼에서 사용 가능한 모바일 앱으로 개발하였다. 채식주의자는 어디에서나 채식 판독 및 추천 서비스를 이용할 수 있다.

**2) Clover OCR**

기술 개요 및 특징: 

이미지에서 텍스트를 추출하여 디지털 텍스트로 변환시키는 OCR 기술을 다양한 운영체제에서 지원하는 엔진이다. 
다양한 언어가 섞여 있는 원재료명을 파악하기에 다국어 지원하는 OCR 엔진이 필요했고 쉬운 시스템 통합을 위해 API를 활용할 수 있는 Clover OCR을 사용했다.

활용: 
- 기술 단순 적용: 시스템 내에서 직접 촬영하거나 이미지 파일을 업로드하여 받은 이미지 데이터를 디지털 텍스트로 변환하도록 구현했다. 
- 기술 적용 후 서비스 구현: 변환된 텍스트는 API를 통해 시스템에 연동되어, 사용자가 업로드한 이미지 내의 OCR 변환은 최대 3초 이내, 해당 사용자 채식 유형에 적합 여부를 최대 1초 이내에 판단하여 섭취 여부를 제공하는 서비스를 제공한다. 

**3) 부분 일치 유사도 (Partial Match Similarity)**
- 개요: 부분적으로 일치하는 항목 간의 유사도를 계산하는 기법
- 활용: 사용자 리뷰와 키워드/식품 유형을 기반으로 한 CBF 알고리즘 구현에 활용

**4) 자카드 유사도 (Jaccard Similarity)**
- 개요: 두 집합 간의 교집합과 합집합을 기반으로 유사도를 측정하는 기법
- 활용: 판독 데이터를 바탕으로 한 유사품 추천 알고리즘 구현

**4) Spring Boot**

버전: 3.3.3

- 개요: 스프링 기반 애플리케이션의 빠른 생성과 배포를 위한 프레임워크
- 활용: 서버 개발

**5) Figma**
- 개요: 실시간 협업을 지원하는 UI 디자인 툴
- 활용: 서비스의 전반적인 UI 디자인

### 시스템 개발 인력
**front**

이서림:
- 보유 기술: JavaScript, HTML, CSS 주력 / Python, Java 사용 가능
- 활용: UX&UI 총괄 및 디자인 통일 
	ReactNative를 통한 프론트 개발: 홈, 사전, 판독, 추천 파트

송한이:
- 보유 기술: Python, Java, HTML 주력
- 활용: UX&UI 디자인: 로그인, 메인, 추천화면 
	ReactNative를 통한 프론트 개발: 로그인, 사용자 화면

**back**

맹현지:
- 보유 기술: Python, Java, SQL 주력
- 활용: 알고리즘 및 기능 구현 / 원재료 데이터 전처리 / 데이터 관리
  
최지영:
- 보유 기술: Python, Java, SQL 주력
- 활용: 기능 구현 / 제품 데이터 전처리 / 데이터 관리

---

### 📖 프로젝트 정보 영상
> **소개 영상**
> 
> ▶️ [채식 어디 소개 영상](https://youtu.be/eAx9oLKwpAM)

> **시연 영상**
> 
> ▶️ [채식 어디 시연 영상](https://youtu.be/PUEc9VYo3kM)

---

# 📖 프로젝트 소개