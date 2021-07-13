![](https://images.velog.io/images/songbetter/post/f683338e-de4e-4f7b-976f-d6a8579000e3/image.png)
# [직방](https://www.zigbang.com/)을 모티브 한 2차 프로젝트: 먹방
> 이 프로젝트는 직방 사이트를 참조하여 학습목적으로 만들었습니다. 실무수준의 프로젝트이지만 학습용으로 만들었기 때문에 이 코드를 활용하여 이득을 취하거나 무단 배포할 경우 법적으로 문제될 수 있습니다.

## Overview
>레이아웃은 직방 웹페이지를 참고했으며, 지역별 매물이 아닌 맛집 정보를 제공하는 사이트로 기획, 제작했습니다. -> [먹방 프로젝트 기획내용 바로보기](https://velog.io/@songbetter/%EC%A7%81%EB%B0%A9-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8-%ED%8C%80-%EB%B0%9C%ED%91%9C)

* **GitHub Repository** Front: [2nd-mukbang-frontend](https://github.com/wecode-bootcamp-korea/18-2nd-mukbang-frontend), Back: [2nd-mukbang-backend](https://github.com/wecode-bootcamp-korea/18-2nd-mukbang-backend)
* **작업기간** 2021/3/29 ~ 2021/4/9
* **기술스택** HTML/CSS, JavaScript(ES6+), React, React Hooks, React Router, Styled Components
* **팀원구성** 프론트엔드 3명 (배성훈, ⭐송나은⭐, 정승옥), 백엔드 2명 (김택향, 이호열)

### 주요 구현 기능
* 카카오맵 API를 활용한 지도, 로드뷰, 클러스터러, 마커 구현 ⭐
* 카카오로그인 API를 활용한 계정 연동, 문자인증 기능 구현
* 검색 필터기능 구현
* 리뷰, 상점 등록기능 구현 ⭐
* 이미지 슬라이더 및 별점기능 구현 ⭐
## 결과
### Map
카카오맵 API 클러스터러, 마커. 지도 레벨에 따라 보여지는 가게의 수가 달라진다.
![image](https://user-images.githubusercontent.com/75013112/125447404-c0332b3f-b6cd-41c8-8264-6c587d5ca97f.png)
### Login & Signup
카카오계정연동 및 자체 회원가입. 문자인증. 컴포넌트 재사용
![](https://images.velog.io/images/songbetter/post/b703c10f-fe36-4234-ac8d-228b231ae425/image.png)
### Home (검색)
![](https://images.velog.io/images/songbetter/post/a35b02d1-ad99-4d80-9e38-9e38f46336be/image.png)
### StoreList
지역 별 가게리스트. 무한스크롤. 특정 가게 호버 시 지도에 마커 표시
### StoreDetail ⭐
* 이미지 슬라이더, 찜하기, 메뉴판/리스트 보기, 메뉴 더보기
![](https://images.velog.io/images/songbetter/post/b012a738-1133-4240-aacf-64fdab872eee/image.png)
* 토글, 별점, 리뷰![](https://images.velog.io/images/songbetter/post/c0e57b33-574e-40d2-85d3-5f2f3023066a/image.png)
* 카카오맵 API 현재 위치 지도, 로드뷰![image](https://user-images.githubusercontent.com/75013112/125447573-29d582fa-d6d2-4da9-aafb-965b043706ad.png)

### Favorite ⭐
StoreDetail 페이지에서 찜한 가게를 모아볼 수 있는 페이지

![](https://images.velog.io/images/songbetter/post/1673a0ad-7eeb-4207-8e1d-aa47d0bb199e/image.png)
### Register
사장님이 가게 정보를 등록할 수 있는 페이지

![](https://images.velog.io/images/songbetter/post/95c71bc3-bf07-4d8f-8761-8113709502b9/image.png)

