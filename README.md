![](https://images.velog.io/images/songbetter/post/f683338e-de4e-4f7b-976f-d6a8579000e3/image.png)
# [직방](https://www.zigbang.com/)을 모티브 한 2차 프로젝트: 먹방

## Preview
>### 내가 직방을 선택했었나?
라는 생각을 계속 하게했던 프로젝트.. 처음 프로젝트 멤버로 발표가 되고 나서 웹페이지를 들어갔을 때 지도를 보고 지레 겁먹었었다. 직방을 모티브로 했던 이전 기수들의 후기를 찾아보면서 엄청 힘들었다는 이야기와 가이드를 이해하는데만 일주일이 걸렸다는 이야기를 보았고, 이번에 기능 구현은 욕심내지 말자고 다짐했다. 

## Overview
>레이아웃은 직방 웹페이지를 참고했으며, 지역별 매물이 아닌 맛집 정보를 제공하는 사이트로 기획, 제작하였다. -> [먹방 프로젝트 기획내용 바로보기](https://velog.io/@songbetter/%EC%A7%81%EB%B0%A9-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8-%ED%8C%80-%EB%B0%9C%ED%91%9C)

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
* 카카오맵 API 현재 위치 지도, 로드뷰

### Favorite ⭐
StoreDetail 페이지에서 찜한 가게를 모아볼 수 있는 페이지

![](https://images.velog.io/images/songbetter/post/1673a0ad-7eeb-4207-8e1d-aa47d0bb199e/image.png)
### Register
사장님이 가게 정보를 등록할 수 있는 페이지
![](https://images.velog.io/images/songbetter/post/95c71bc3-bf07-4d8f-8761-8113709502b9/image.png)


## Review
>### 2차 프로젝트를 대하는 나의 목표
* Hooks, Styled-components, Rebase 지도 API 사용하는 방법 제대로 알기!
* mergy>mergy>mergy 해서 기능+레이아웃을 합쳤을 때 conflict 빠르게 해결하기
* 추가 기능구현에 욕심내는 것보단 구현한 기능을 버그없이 완성하기!
* 컴포넌트 재사용, 함수재사용, 변수활용으로 불필요한 반복 줄이기!

열정 넘치는 팀원들에 비해 나는 많은 기능을 구현하는 것보다 기본에 충실하려고 노력했다.
그래도 내가 맡은 StoreDetail 영역이 여러 기능을 구현해 볼 수 있는 영역이어서 할 수 있는 기능은 다 해본 것 같다.

> 가게정보, 메뉴, 토글, 방문자 사진, 리뷰는 모두 컴포넌트를 재사용하는 방법을 이용했고, 컴포넌트를 재사용하면서 함께 움직이는 것들에 대한 제어가 필요했다.

Hooks를 배우는 과정이었기 때문에 멘토님들께 힌트를 얻고나서도 이해하는 데 많은 시간이 걸렸다. state를 배열로 관리한다는 생각은 아예 하지도 못했었다.
버그로 남겨놓고 내가 맡은 기능 구현을 이어 나가면서 어떻게 해결해야 할 지 고민이 많았는데, 별점기능을 구현하면서 state를 배열로 관리한다+index를 이용한다를 알게되었다.
2주동안 useEffect와 useState를 계속 사용하면서 자연스럽게 체득하게 되었고 결국 버그를 해결할 수 있었다. 지금보면 너무 간단한 토글기능(👇사진)
![](https://images.velog.io/images/songbetter/post/488d458e-779c-4f0e-a83b-974ee7a9ceb8/image.png)

> 이미지슬라이더와 별점은 라이브러리를 사용하지 않고 구현했다.
처음엔 어떻게 접근해야 할 지 몰라서 구글링을 열심히 했다. 다른 개발자의 코드를 갖다 쓰는 게 라이브러리를 쓰는거랑 뭐가 다른건가 싶은 생각이 들었고, 순간 뭐하고 있는거지 라는 생각이 들었다.
따라치는 것이 아니라 강의나 참고자료를 본 다음 이해한 것을 바탕으로 나만의 방식으로 코드를 작성하려고 노력했다. 별점 기능을 구현할 때에도 대부분 하나의 아이콘에 CSS로 Color를 변화하는 식으로 구현했지만, 나는 아이콘을 하나하나 바꿔주는 방법을 택했다. 이해를 바탕으로 작성한 코드였기 때문에 다른 기능을 구현할 때 엄~청 도움이 됐다.
![](https://images.velog.io/images/songbetter/post/2931e89d-0cce-4d87-af88-404dd017bbab/image.png)

> 이번 프로젝트에서 개인적인 목표는 달성했다. 
새로운 기술을 배우고, 구글링을 하면서 그냥 복사+붙여넣기 하지 않으려고 노력했고, 버그 없이 완성된 결과물을 낼 수 있었다. 
리뷰 반영도 최우선적으로 고려한 덕분에 멘토님들의 리뷰를 돌아가면서 받으며 기본을 단단히 다질 수 있었다.
지도를 다루는 프로젝트에서 커스텀하는 부분을 많이 해보지 못한 건 아쉽지만, 기본을 다지는 것만으로도 벅찬 2주였다.

> 팀의 목표를 달성하기 위해서 문제를 함께 해결해나갔다.
먹방 프로젝트를 시작할 때 내가 맡은 부분은 찜한가게, 스토어디테일 부분이었다.
하지만 1차 Sprint가 시작되고 내가 갑자기 리뷰 부분을 추가로 맡게 되었고, 성훈님이 찜한가게를 맡아 주시기로 했다.
작업을 하던 중 내가 맡은 부분이 생각보다 빠르게 진행되어 새로운 기능 구현이 가능한 상태였지만, 일단 찜한가게를 뒤로 미루고 성훈님의 문제를 함께 해결해나갔다.
팀 프로젝트였기 때문에 혼자 기능구현 하는 것보다 서로 코드리뷰를 해주면서 함께 완성해 나가는 게 더 중요하다고 생각했다.
성훈님의 코드를 고쳐나가면서 기능 구현 뿐만 아니라 중복되는 코드를 줄일 수 있었고, 내가 구현해보지 않은 기능에 대해서 배울 수 있어서 서로 윈윈할 수 있었다.
