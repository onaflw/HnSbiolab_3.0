# 🩺 신장질환 관리를 위한 디지털 헬스케어 플랫폼

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/146da311-7423-4416-8235-6fd54e057cee" />

<br/>

## 프로젝트 소개

👉 **신장질환의 조기 발견**과 지속적인 관리를 위해 **진단 키트와 검사 데이터를 통합 분석·관리**하는 디지털 헬스케어 서비스입니다.

- 초기 증상이 거의 없는 신장 질환의 특성을 고려하여, 조기 발견과 지속적인 건강 관리를 목표로 개발되었습니다.
- 신장병 조기진단 키트와 연동하여 검사 결과를 분석하고 데이터를 저장합니다.
- 건강검진 기록 및 혈액검사 데이터를 통합 관리할 수 있도록 설계되었습니다.
- 질환 진행을 예방하고 환자의 삶의 질을 향상시키는 것을 목표로 합니다.

<br/>

**Development History**

<p align="left">
  <sub>
  이 레포는 리팩토링 및 구조 재정리된 최종 버전입니다.<br/>
  초기 개발 레포지토리는 아래에서 확인할 수 있습니다.<br/>
  👉 <a href="https://github.com/beefed-up-geek/HnSbio_ver2">Original Repository</a>
  </sub>
</p>

<br/>

## 팀원 구성

<div align="center">

  <table> 
    <tr> 
      <td align="center"><img src="https://avatars.githubusercontent.com/u/62469125?v=4" width="100px"></td> 
      <td align="center"><img src="https://avatars.githubusercontent.com/u/163401793?v=4" width="100px"></td> 
      <td align="center"><img src="https://avatars.githubusercontent.com/u/110738697?v=4" width="100px"></td> 
      <td align="center"><img src="https://avatars.githubusercontent.com/u/92612072?v=4" width="100px"></td> 
      <td align="center"><img src="https://avatars.githubusercontent.com/u/149086418?v=4" width="100px"></td> 
    </tr>
    <tr> 
      <td align="center"><a href="https://github.com/beefed-up-geek">곽태윤</a> <br>Tech Lead<br/>BE</td>
      <td align="center"><a href="https://github.com/clrdl">김지수</a> <br>FE</td>
      <td align="center"><a href="https://github.com/drdr3040">오지훈</a> <br>FE</td>
      <td align="center"><a href="https://github.com/onaflw">최한송</a> <br>Team Lead<br/>BE</td> 
      <td align="center"><a href="https://github.com/yellowacidblack">황재현</a> <br>FE</td> 
    </tr> 
  </table>

</div>

<br/>

## 기술 스택

- **Frontend**: React Native, Kakao API, Google APIs, Apple Developer
- **Backend**: Node.js, Express.js, MongoDB, Meilisearch
- **Infrastructrue**: AWS EC2, Amazon S3
- **External APIs**: ScalaWox API, Codef API, HIRA Open Data, MFDS Open Data
- **DevOps**: Git, GitHub, GitHub Actions

<br/>

## 아키텍처 다이어그램

![구성도.png](readme_assets/arch.png)

<br/>

## 🏆 프로젝트 성과

- 건강보험심사평가원 보건의료빅데이터활용 창업경진대회 | **우수상**
- 식품의약품안전처 식의약 데이터 활용 경진대회 | **장려상**

<br/>

## 설치/실행 방법

```
npm install
npm start
```

### iOS 실행

```
npx react-native run-ios
```

### Android 실행

```
npx react-native run-android
```

---

<br/>

## 🔎 주요 기능

### 1. 키트 검사

키트 검사 방법을 설명하고, 키트 검사를 실시합니다. 사용자가 키트의 이미지를 Scala Wox의 API에 전송하면, 키트 검사의 결과를 반환받아서 DB에 저장합니다.

<p align="center">
  <img src="readme_assets/KakaoTalk_Photo_2024-12-31-14-13-15_015.jpeg" width="30%" />
  &nbsp;&nbsp;&nbsp;
  <img src="readme_assets/KakaoTalk_Photo_2024-12-31-14-13-15_016.jpeg" width="30%" />
</p>

<br/>

### 2. 건강검진 내역 불러오기

[Codef API의 건강검진 API](https://developer.codef.io/products/public/each/pp/nhis-health-check)를 통해 보건복지부에서 사용자의 건강검진 기록과 결과 PDF를 불러옵니다. 불러온 결과를 분석하고, 신장병과 긴밀히 연관된 기저질환·성인병 분석도 진행할 예정입니다.

<p align="center">
  <img src="readme_assets/KakaoTalk_Photo_2024-12-31-14-13-15_023.jpeg" width="30%" />
  &nbsp;&nbsp;&nbsp;
  <img src="readme_assets/KakaoTalk_Photo_2024-12-31-14-13-15_018.jpeg" width="30%" />
</p>

<br/>

### 3. 혈액검사 기록 & 콩팥 건강 분석

신장병 고위험군 혹은 환자는 정기적으로 혈액검사를 실시합니다. 앱에서 혈액검사 결과를 기록하고, 분석 결과를 제공합니다.

<p align="center">
  <img src="readme_assets/KakaoTalk_Photo_2024-12-31-14-13-15_023.jpeg" width="30%" />
  &nbsp;&nbsp;&nbsp;
  <img src="readme_assets/KakaoTalk_Photo_2024-12-31-14-13-15_022.jpeg" width="30%" />
  &nbsp;&nbsp;&nbsp;
  <img src="readme_assets/KakaoTalk_Photo_2024-12-31-14-13-14_009.jpeg" width="30%" />
</p>

<br/>

### 4. 투석병원 & 의약품 검색

[혈액투석 적정성 평가 등급](https://www.hira.or.kr/ra/hosp/getHealthMap.do?pgmid=HIRAA030002010000&WT.gnb=%EB%B3%91%EC%9B%90+%C2%B7+%EC%95%BD%EA%B5%AD%EC%B0%BE%EA%B8%B0#a)을 참고하여  주변 투석 병원을 검색할 수 있습니다. 거리, 등급, 병원 종류 등의 필터가 제공되며, 자주 찾는 병원은 즐겨찾기로 지정할 수 있습니다.

<p align="center">
  <img src="readme_assets/KakaoTalk_Photo_2024-12-31-14-13-15_024.jpeg" width="30%" />
  &nbsp;&nbsp;&nbsp;
  <img src="readme_assets/KakaoTalk_Photo_2024-12-31-14-13-15_025.jpeg" width="30%" />
</p>

**[식품의약품안전처 의약품 데이터](https://www.data.go.kr/data/15075057/openapi.do)를 바탕**으로 의약품을 검색할 수 있습니다. [대한약사협회 신장병 위해 성분 정보](https://www.health.kr/Menu.PharmReview/_uploadfiles/Safety%20Report_%EC%8B%A0%EC%9E%A5%EC%97%90%20%EC%98%81%ED%96%A5%EC%9D%84%20%EB%AF%B8%EC%B9%98%EB%8A%94%20%EC%95%BD%EB%AC%BC%20%EC%95%88%EC%A0%84%EC%84%B1%20%EC%A0%95%EB%B3%B4.pdf)도 참고하여, 어떤 의약품이 신장에 해로운지 안내합니다.

<p align="center">
  <img src="readme_assets/KakaoTalk_Photo_2024-12-31-14-13-16_027.jpeg" width="30%" /> 
  &nbsp;&nbsp;&nbsp;
  <img src="readme_assets/KakaoTalk_Photo_2024-12-31-14-13-16_028.jpeg" width="30%" />
</p>

<br/>

### 5. 데일리 체크

콩팥 상태를 매일 체크할 수 있는 6가지 항목을 제공하며, 3개 이상 위험 신호가 감지되면 키트 검사를 유도합니다.

<div align="center">
  <img src="readme_assets/KakaoTalk_Photo_2024-12-31-14-13-14_006.jpeg" width="30%" />
  &nbsp;&nbsp;&nbsp;
  <img src="readme_assets/KakaoTalk_Photo_2024-12-31-14-13-14_010.jpeg" width="30%" />
</div>
