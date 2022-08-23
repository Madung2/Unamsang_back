# 📌 You know what I'm sayin'

<img src='https://velog.velcdn.com/images/tasha_han_1234/post/69414403-7a14-42e1-acb9-490194034a8e/image.png'>

- 텍스트 to 이미지 AI 서비스
- 사이트 링크: 

## 1. 제작 기간 & 참여 인원
- 2022.06.28 ~ 2022.07.05
- 팀 프로젝트(4명)

## 2. 사용 기술

<div style="display:flex">
    <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=Python&logoColor=white">
    <img src="https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=Django&logoColor=white">
      <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=JavaScript&logoColor=white">
    <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=HTML5&logoColor=white">
      <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=CSS3&logoColor=white">
      <img src="https://img.shields.io/badge/MySQL-4169E1?style=for-the-badge&logo=MySQL&logoColor=white">
        <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=PyTorch&logoColor=white">
  </div>

## 3. 아키텍쳐 및 ERD 설계

<img src='https://velog.velcdn.com/images/tasha_han_1234/post/3a9841c6-21b2-4880-81ef-78ffd98b5cf8/image.png'>

## 4. 핵심 기능
<details close>
  <summary>📌 로그인/회원가입</summary>
  유효성 검사, 아이디 중복 검사, JWT Token사용, 카카오 소셜 로그인
</details>


## 5. 핵심 트러블 슈팅

#### 검색창에 active 상태가 true면서, 게시 만료일이 지나지 않은 게시물 sorting 하는 방법 

* 검색창에서 쿼리를 날릴때, 3가지 조건, 검색어가 제목이나 작정자에 해당하면서도, active 상태가 true, 게시물 만료일이 지나지 않은 것을 검색할 필요가 있었습니다.

* 하지만 처음의 전 각각 따로 sorting 하는 방법밖에 떠오르지 않았고, 불필요한 쿼리를 줄이고 싶다고 생각하게 되었습니다.<br> 

* 이 시점쯤에 stackoverflow와 장고 도큐먼트를 좀 더 편하게 사용할 수 있게 되었는데,<br>
검색어로 'django filter', 'django queries'등을 검색한 결과 Q()를 사용해 3가지 조건을 연결을 할 수 있는 식을 세우게 되었습니다. 


![code1](https://user-images.githubusercontent.com/104334219/186073479-6e66c1c2-4770-4afb-b4df-692c4164fe7f.png)


## 6. 기타 트러블 슈팅

<details close>
  <summary>📌 Assertion Error</summary>
  assertion의 뜻은 '역설'이라는 말인데 개발자가 생각을 못한 문제가 에러가 생겼을때 뜨는 에러입니다.
  'AssertionError: Expected a Response, HttpResponse or HttpStreamingResponse to be returned from the view, but received a <class 'NoneType'>'이란 에러문구가 떴는데,
  Response를 원한다고 해서 백에서의 문제일거라 생각하고 하나하나 체크를 해봤는데 큰 문제가 없었습니다.
  다시 print를 찍어가며 차근차근 에러가 난 곳을 되짚어 가보니 back이 아닌 front 단에서 유저명이 겹치는 문제가 있었습니다.
</details>
    
<details close>
  <summary>📌 AI 적용시 시간 소요 문제 </summary>
    처음에는 'Dall-E'모델을 사용해서 text-to-image를 구현하려고 했습니다만, 모델이 많이 무거워서 우리같은 초보자들이 구현하기에는 어렵겠다 싶었고 

</details>



## 7. 성장 & 회고
* 요즘 가장 핫한 ai 분야 중 하나인 'text to image'를 사용해 볼 수 있었던게 정말 즐거운 경험이 된것 같습니다. 
* 본격적으로 DRF를 사용한 첫 프로젝트 였는데 시리얼라이저를 쓰면서 좀더 클린한 코드를 쓰고 싶다는 욕심도 갖게 되었습니다. 이후 '파이썬 클린 코드'란 책을 읽으면서 조금씩 제 코드에 대입해 보고 있습니다. 

* 이 프로젝트를 하기 전까지 자바스크립트를 전혀 할 줄 몰랐습니다. 주변사람에 묻고 구글링을 하면서 하나의 프로젝트를 완성하고 나니 편안하게 기본적인 사이트 구성에 필요한 [자바스크립트](https://velog.io/@tasha_han_1234/exqg7cbz)를 쓸 수 있게 되었는데, 이 점도 스스로 뿌듯함을 느낄 수 있었던 부분 입니다.

