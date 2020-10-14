# CBNU web-programming playground

## 🙌 1주차 실습

- [hello world](./lecture1/index.html)

<br>

## 🙌 2주차 실습

### DEMO: [CLICK HERE 👀](./lecture2/index.html)

- [Anchor 태그 실습](./lecture2/anchor.html)
- [Image 태그 실습](./lecture2/image.html)
- [List 태그 실습](./lecture2/list.html)
- [Table 태그 실습](./lecture2/table.html)
- [Audio 태그 실습](./lecture2/audio.html)
- [Video 태그 실습](./lecture2/video.html)
- [Youtube 동영상 삽입](./lecture2/youtube.html)
- [Form 양식 태그 실습](./lecture2/form.html)

## 🙌 4주차 실습
#### [Demo Link](./lecture4/index.html)

## 요구사항

 **'My Home Page' 레이아웃 구현하기**

<img width="550" alt="스크린샷 2020-10-14 오후 10 30 13" src="https://user-images.githubusercontent.com/36187948/95995718-d5bb2280-0e6c-11eb-9e56-c2ee0a135029.png">

<br>

## 구조 설계

- 각 section의 구조 정하기

  - header section
  <img width="500" alt="스크린샷 2020-10-14 오후 10 34 48" src="https://user-images.githubusercontent.com/36187948/95996327-81fd0900-0e6d-11eb-8f41-25724e147c0e.png">
    
    - navigation menu 구현 (list tag 사용)
      ```html
  	  <ul class="nav">
    	  <li class="nav-menu">메뉴1</li>
        <li class="nav-menu">메뉴2</li>
        <li class="nav-menu">메뉴3</li>
      </ul>
  	  ```
      
      ```css
      {
        display: flex;  
        align-items: center;
      }
      ```
    
      flex값을 적용시켜 메뉴들을 나란히 나열한다.
      
      hover와 active 상태일 때, 컬러를 적용하여 유저에게 UI피드백을 제공한다.
      
      > hover
  
       <img width="177" alt="스크린샷 2020-10-14 오후 10 41 36" src="https://user-images.githubusercontent.com/36187948/95997140-7100c780-0e6e-11eb-8585-1df80da38f65.png">
      
        > active
      
        <img width="173" alt="스크린샷 2020-10-14 오후 10 45 25" src="https://user-images.githubusercontent.com/36187948/95997649-f5534a80-0e6e-11eb-9fd7-93f2f5d23871.png">

    <br>
  
- content section

  <img width="400" alt="스크린샷 2020-10-14 오후 10 34 53" src="https://user-images.githubusercontent.com/36187948/95996334-83c6cc80-0e6d-11eb-955b-534d40de4b5f.png">

  - content-image section

     <img width="400" alt="스크린샷 2020-10-14 오후 10 38 07" src="https://user-images.githubusercontent.com/36187948/95996709-f59f1600-0e6d-11eb-8060-e83b1e6a5672.png">
     - image container영역에` position: relative`값을 적용
     - img태그에 width 100%를 적용
     - "My Home Page"와 하단의 "Lorem ipsum dolor" 텍스트에 absolute값을 적용하여, 각각의 위치를 잡아줌
  - article-section

     <img width="400" alt="스크린샷 2020-10-14 오후 10 38 11" src="https://user-images.githubusercontent.com/36187948/95996715-f6d04300-0e6d-11eb-9542-35b599155551.png">
     - Section1 과 Aside를 top-section, Section2를 bottom-section으로 구분
     - Section1과 Aside container에 `flex`를 적용
     - Section1 에 `flex: 2 1 0`, Aside에 `flex: 1 1 0`을 적용하여 2:1 비율 유지 
     - Section2와 이미지는 flex로 나열

  <br>

- footer section

  <img width="500" alt="스크린샷 2020-10-14 오후 10 34 58" src="https://user-images.githubusercontent.com/36187948/95996336-84f7f980-0e6d-11eb-90c3-1a9e43ea6b45.png">

  ```css
  {
    display: flex;
    align-items: center;
    justify-content: center;
  }
  ```

  > flex 속성을 이용하여, 좌우 상하 가운데 정렬

