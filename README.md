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

