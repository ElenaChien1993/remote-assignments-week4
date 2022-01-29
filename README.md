### DEMO page

[Remote Assignments - Week 4](https://elenachien1993.github.io/remote-assignments-week4/)

## 作業項目

- 完成 2 題 JS function
- 將 Week 1 project 轉換成 React project

## Assignment 3: Re-Implement Layout by React
### 學習筆記

### 1. 在 React 中使用 media query

 [https://github.com/yocontra/react-responsive](https://github.com/yocontra/react-responsive) 

我參考使用了 react-responsive 函式庫

```jsx
import MediaQuery from 'react-responsive'

const Header = (props) => {
  return (
    <div className="main-header">
      <h4 className="name">Animal Shelter</h4>
      <MenuBars 
        toggleMenuOpen={ props.toggleMenuOpen }
        isMenuOpen={ props.isMenuOpen }
      />
      <MenuOverlay 
        isMenuOpen={ props.isMenuOpen }
      />
      <MediaQuery minWidth={800}>
        <Nav />
      </MediaQuery>
    </div>
  )
}
```

### 2. 在 React 中放圖片

[【React.js入門 - 29】 使用圖片、使用css檔、新手容易遇到的問題 - iT 邦幫忙::一起幫忙解決難題，拯救 IT 人的一天](https://ithelp.ithome.com.tw/articles/10226711)

原本以為 HTML 直接複製貼上即可，才發現圖片會消失，必須使用 `import` 或是 `require`

如果要使用 jpg、png 這種圖片，方式有兩種:

1. import後再使用
    
    ```jsx
    import Rice from "./rice.jpg";
    ```
    
    ```jsx
    <img src={Rice} alt="Rice"/>
    ```
    
2. 直接在 src 使用 require
    
    ```jsx
    <img src={require("./rice.jpg")} alt="Rice"/>
    ```
    

### 3. 將 React 專案放上 github page

[[Day 29 - 即時天氣] 寫網頁就是要炫耀啊，不然要幹麻？發布上 Github Pages 吧！ - iT 邦幫忙::一起幫忙解決難題，拯救 IT 人的一天](https://ithelp.ithome.com.tw/articles/10228423)
