效果如下：
![](https://github.com/lc-dmx/css/blob/master/CSS3%E5%AE%9E%E7%8E%B0%E2%80%9C%E5%9B%BE%E7%89%87%E9%98%B4%E5%BD%B1%E2%80%9D%E6%95%88%E6%9E%9C/4.jpg)
主要代码如下:
实现曲线阴影
```
.effect{
	position: relative;
	box-shadow:0 1px 4px rgba(0,0,0,0.3),0 0 40px rgba(0,0,0,0.1) inset;
	-webkit-box-shadow:0 1px 4px rgba(0,0,0,0.3),0 0 40px rgba(0,0,0,0.1) inset;
	-moz-box-shadow:0 1px 4px rgba(0,0,0,0.3),0 0 40px rgba(0,0,0,0.1) inset;
	-o-box-shadow:0 1px 4px rgba(0,0,0,0.3),0 0 40px rgba(0,0,0,0.1) inset;
}
.effect:before,.effect:after{
	content:'';
	background:red;
	position: absolute;
	z-index: -1;
	top:50%;
	bottom:0;
	left:25px;
	right:25px;
	box-shadow:0 0 20px rgba(0,0,0,0.8);
	-webkit-box-shadow:0 0 20px rgba(0,0,0,0.8);
	-moz-box-shadow:0 0 20px rgba(0,0,0,0.8);
	-o-box-shadow:0 0 20px rgba(0,0,0,0.8);
	border-radius: 100px/10px;
}
```
实现翘边阴影
```
.box li{
	width:300px;
	height:auto;
	float:left;
	position: relative;
	background: #fff;
	margin:20px 10px;
	border:2px solid #efefef;
	box-shadow: 0 1px 4px rgba(0,0,0,0.27),0 0 60px rgba(0,0,0,0.1) inset;
	-webkit-box-shadow: 0 1px 4px rgba(0,0,0,0.27),0 0 60px rgba(0,0,0,0.1) inset;
	-moz-box-shadow: 0 1px 4px rgba(0,0,0,0.27),0 0 60px rgba(0,0,0,0.1) inset;
	-o-box-shadow: 0 1px 4px rgba(0,0,0,0.27),0 0 60px rgba(0,0,0,0.1) inset;
}
.box li img{
	width:290px;
	height:auto;
	margin:5px;
	display:block;
}
.box li:before{
	content:'';
	position: absolute;
	z-index: -1;
	width:90%;
	height: 80%;
	left:20px;
	bottom:8px;
	background:transparent;
	box-shadow:0 8px 20px rgba(0,0,0,0.6);
	-webkit-box-shadow:0 8px 20px rgba(0,0,0,0.6);
	-moz-box-shadow:0 8px 20px rgba(0,0,0,0.6);
	-o-box-shadow:0 8px 20px rgba(0,0,0,0.6);
	-webkit-transform: skew(-12deg) rotate(-4deg);
	-moz-transform: skew(-12deg) rotate(-4deg);
	-o-transform: skew(-12deg) rotate(-4deg);
	-ms-transform: skew(-12deg) rotate(-4deg);
}
.box li:after{
	content:'';
	position: absolute;
	z-index: -1;
	width:90%;
	height: 80%;
	right:20px;
	bottom:8px;
	background:transparent;
	box-shadow:0 8px 20px rgba(0,0,0,0.6);
	-webkit-box-shadow:0 8px 20px rgba(0,0,0,0.6);
	-moz-box-shadow:0 8px 20px rgba(0,0,0,0.6);
	-o-box-shadow:0 8px 20px rgba(0,0,0,0.6);
	-webkit-transform: skew(12deg) rotate(4deg);
	-moz-transform: skew(12deg) rotate(4deg);
	-o-transform: skew(12deg) rotate(4deg);
	-ms-transform: skew(12deg) rotate(4deg);
}
```
