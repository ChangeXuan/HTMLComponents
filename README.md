# HTMLComponents
## 这里收集一些HTML和CSS的布局组件，方便开发


- 导航栏组件
```html
<link href="http://cdn.static.runoob.com/libs/bootstrap/3.3.7/css/bootstrap.min.css" rel="stylesheet">

<nav class="navbar navbar-default navbar-fixed-top topnav" role="navigation">
        <div class="container">
            <div class="navbar-header">
                <a class="navbar-brand" href="https://github.com/ChangeXuan" target="_blank">ChangeXuan</a>
            </div>

            <div class="navbar-collapse">
                <ul class="nav navbar-nav navbar-right">
                    <li>
                        <a href="#about">About</a>
                    </li>
                    <li>
                        <a href="#skills">Skills</a>
                    </li>
                    <li>
                        <a href="#portfolio">Portfolio</a>
                    </li>
                   <li>
                        <a href="#contact">Contact</a>
                    </li>
                </ul>
            </div>
        </div>
</nav>
```
```css
.topnav {
    font-size: 16px;
    border-bottom: 1px outset rgba(0, 0, 0, 1);
    background: rgba(0, 0, 0, 1);
    box-shadow: 0px 1px rgba(0, 0, 0, 1);
}

.navbar-brand {
  	background: rgba(0, 0, 0, 1);
	color: #fff;
}

.topnav ul.navbar-nav li a {
	background: rgba(0, 0, 0, 1);
	color: #fff;
}

.topnav ul.navbar-nav li a:hover,
.topnav ul.navbar-nav li a:focus
 {
background: rgba(255, 255, 255, 0.5);
color: #fff;
}

.topnav .navbar-brand:hover,
.topnav .navbar-brand:focus {
  background: rgba(255, 255, 255, 0.5);
  color: #fff;
}
```

- 展示组件
```
由于不好描述，所以我以文件的形式放在相应的文件夹中
html->./html/ShowPortfolio.html
css->./css/ShowPortfolio.html
js->./js/easyResponsiveTabs.js
需要使用jquery.min.js
把easyResponsiveTabs.js放在./js下
```

- 页尾署名组件
```html
<div class="pageFooter">
  <p> &copy; Hello World | Design by <a href="https://github.com/ChangeXuan">ChangeXuan</a></p>
</div>
```
```css
.pageFooter{
	padding:30px 0px;
}
.pageFooter p{
	text-align:center;
	color:#000;
	font-size:14px;
}
.pageFooter p a{
	color: #F58703;
}
.pageFooter p a:hover{
	text-decoration:underline;
}
```

- 关于我组件
```html
<div class="about">
  <div class="container">
    <h3>About Me</h3>
    <label class="line"></label>
    <img src="https://image.com" alt="this is img" />
    <p>xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx</p>
    <p>xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx</p>
  </div>
</div>
```
```css
.about {
	padding:55px 0px;
	text-align:center;
}
.about h3 {
	color:#000;
	font-size:36px;
}
.line {
    display: block;
    background-color: #56b2e6;
    width: 65px;
    height: 3px;
    margin: 12px auto;
}
.about img {
    width: 10%;
    border-radius: 50%;
	margin-top:35px;
}
.about p{
	text-align:center;
	font-size:14px;
	color:#000;
	line-height:27px;
	width:60%;
	margin:0 auto;
	margin-top:20px;
}
```

- 描述小卡片组件
```html
<div class="article">
  <a href="https://en.wikipedia.org/wiki/Hello Kitty" target="_blank">
    <h2>Hello Kitty</h2>
    <div>
      <img src="https://image.jpg">
      <p>Hello this is mini car</p>
    </div>
  </a>
</div>
```
```css
.article {
  padding: 20px;
  font-family: 'Lora', serif;
  background: #fff;
  padding: 20px 50px;
  margin-bottom: 20px;
}

.article:hover {
  background-color: #E5EDDC;
}

.article img {
  float: left;
  margin: 0 5px 5px 0;
}
```

- 点击镂空效果按钮
```html
<head>
<link href="http://cdn.static.runoob.com/libs/bootstrap/3.3.7/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
	<div class="text-center">
		<button class="testButton" type="button">LOGIN</button>
	</div>
</body>
```
```css
.testButton {
    font-size: 1em;
    color: #fff;
    background: #FFC107;
    border: 3px solid #FFC107;
    outline: none;
    cursor: pointer;
    padding: .6em 1em;
    -webkit-appearance: none;
    width: 50%;
    -webkit-border-radius: 8px;
    -moz-border-radius: 8px;
    -ms-border-radius: 8px;
    -o-border-radius: 8px;
    border-radius: 8px;
}
.testButton:hover {
    background: transparent;
    color: #FFC107;
    border-color:#FFC107 ;
    transition: 0.5s all ;
    -webkit-transition: 0.5s all;
    -moz-transition: 0.5s all;
    -o-transition: 0.5s all;
    -ms-transition: 0.5s all;
}

.testButton { 
    margin-top:  2.1em;
    margin-bottom: 2.1em;
    padding: .5em 1em; 
    border-width: 1px; 
    font-size: 0.9em; 
}
```

- 登录输入框组件
```html
<head>
<link href="http://cdn.static.runoob.com/libs/bootstrap/3.3.7/css/bootstrap.min.css" rel="stylesheet">
</head>
<body style="background:#000;">
	<h3 class="text-center" style="color:#fff;">hello</h3>
	<form action="#" method="post">
		<div class="input-row">
	 		<input type="text" class="userinput" name="User Name" placeholder="User Name" required=""/> 
	 		<input type="password" class="pwdinput" name="Password" placeholder="Password" required=""/>
		</div>
	</form>
</body>
```
```css
.input-row {
    margin-left: auto;
    margin-right: auto;
    width:50%;
    margin-top: 5em;
    padding: 1em 1.5em;
    border: 1px solid #c7c7c7;
    -webkit-border-radius: 15px; 
    -moz-border-radius: 15px;  
    -o-border-radius: 15px;
    -ms-border-radius: 15px;
    border-radius: 15px;
}

.userinput,.pwdinput {
    outline: none;
    font-size: 1em;
    color: #fff;
    padding: 0.6em 1em .8em 2em;
    margin: 0;
    width: 83.6%;
    border: none;
    -webkit-appearance: none;
    display: block;
    background: transparent;
    -webkit-border-radius: 3px;
    -moz-border-radius: 3px;
    -o-border-radius: 3px;
    -ms-border-radius: 3px;
    border-radius: 3px;
    font-family: 'Athiti', sans-serif;
}
.userinput {
    background: url(../images/1.png)no-repeat 2px 10px;
    display: block;
    border-bottom: 1px solid #c7c7c7;
}
.pwdinput{
    background: url(../images/2.png)no-repeat 2px 10px;
    display: block;
    margin-top:0.3em;
}

.userinput::-webkit-input-placeholder{ 
    font-size: 1em; 
    font-family: 'Athiti', sans-serif;
}
::-webkit-input-placeholder {
   color: #fff; 
   font-family: 'Athiti', sans-serif; 
} 
:-moz-placeholder { /* Firefox 18- */
   color: #fff;
   font-family: 'Athiti', sans-serif;
} 
::-moz-placeholder {  /* Firefox 19+ */
    color: #fff; 
    font-family: 'Athiti', sans-serif;
} 
:-ms-input-placeholder {  
   color: #fff; 
   font-family: 'Athiti', sans-serif;
}
```

- 跳转链接文字
