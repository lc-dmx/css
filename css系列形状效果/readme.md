主要效果如下：
![](https://github.com/lc-dmx/css/blob/master/css%E7%B3%BB%E5%88%97%E5%BD%A2%E7%8A%B6%E6%95%88%E6%9E%9C/comment_bubble.jpg)
```
.comment_bubble {
        width: 140px;
        height: 100px;
        background: #088cb7;
        position: relative;
        border-radius: 12px;
}
  
.comment_bubble:before {
        content: "";
        width: 0;
        height: 0;
        right: 100%;
        top: 38px;
        position: absolute;
        border-top: 13px solid transparent;
        border-right: 26px solid #088cb7;
        border-bottom: 13px solid transparent;
}
```
![](https://github.com/lc-dmx/css/blob/master/css%E7%B3%BB%E5%88%97%E5%BD%A2%E7%8A%B6%E6%95%88%E6%9E%9C/geometry.jpg)
```
.oval{
	width: 200px;
	height: 100px;
	margin: 50px;
	float: left;
	position: relative;
	background: #e9337c;
	border-radius: 100px / 50px;
}

.triangle1 {
    	width: 0;
    	height: 0;
	margin: 50px;
	float: left;
	position: relative;
   	border-bottom: 100px solid #fcf921;
    	border-left: 50px solid transparent;
    	border-right: 50px solid transparent;
} 

.triangle2 {
    	width: 0;
    	height: 0;
	margin: 50px;
	float: left;
	position: relative;
   	border-top: 100px solid #20a3bf;
    	border-left: 50px solid transparent;
    	border-right: 50px solid transparent;
} 

.triangle3 {
    	width: 0;
    	height: 0;
	margin: 50px;
	float: left;
	position: relative;
 	border-top: 50px solid transparent;
    	border-right: 100px solid #6bbf20;
    	border-bottom: 50px solid transparent;
} 

.diamond {
	width: 100px;
	height: 100px;
	background: #1eff00;
	position: relative;
	left: 150px;
	top: 250px;

	-webkit-transform: rotate(-45deg);
	-moz-transform: rotate(-45deg);
	-ms-transform: rotate(-45deg);
	-o-transform: rotate(-45deg);
    	transform: rotate(-45deg);

	-webkit-transform-origin: 0 100%;
	-moz-transform-origin: 0 100%;
	-ms-transform-origin: 0 100%;
	-o-transform-origin: 0 100%;
    	transform-origin: 0 100%;
}

.trapezium {
    	height: 0;
        	width: 100px;
	left: 300px;
	top: 150px;
    	position: relative;
    	border-bottom: 100px solid #ec3504;
    	border-left: 50px solid transparent;
    	border-right: 50px solid transparent;
} 

.parallelogram {
    	width: 150px;
    	height: 100px;
    	left: 550px;
	top: 50px;
    	position: relative;
    	background: #8734f7;
	-webkit-transform: skew(30deg);
	-moz-transform: skew(30deg);
	-o-transform: skew(30deg);
    	transform: skew(30deg);
}  

.egg{
	width: 140px;
	height: 200px;
	left: 80px;
	top: 100px;
    	position: relative;
	background: #ffc000;
	display: block;
	border-radius: 50% 50% 50% 50% / 60% 60% 40% 40%;
}
```
![](https://github.com/lc-dmx/css/blob/master/css%E7%B3%BB%E5%88%97%E5%BD%A2%E7%8A%B6%E6%95%88%E6%9E%9C/heart.gif)
```
.heart{
	position: relative;
	width: 100px;
	height: 100px;
	background-color: red;
	margin:100px;

	animation: heartAnimate 1.5s ease infinite;
             -webkit-animation: heartAnimate 1.5s ease infinite;    
             -moz-animation: heartAnimate 1.5s ease infinite;
             -o-animation: heartAnimate 1.5s ease infinite;
             -ms-animation: heartAnimate 1.5s ease infinite;

}

.heart:before , .heart:after{
	position: absolute;
	display: block;
	content: "";
	width: 100px;
	height: 100px;
	border-radius: 100%;
	background-color: red;
}

.heart:before{
	left: -50%;
	top: 0;
}

.heart:after{
	right: 0;
	top: -50%;
}

@keyframes heartAnimate{
	0%,100%{
		transform: scale(1) rotate(45deg);
	}
	10%,30%{
		transform: scale(0.9) rotate(45deg);
	}
	20%,40%,60%,80%{
		transform: scale(1.1) rotate(45deg);
	}
	50%,70%{
		transform: scale(1.1) rotate(45deg);
	}
}
```
![](https://github.com/lc-dmx/css/blob/master/css%E7%B3%BB%E5%88%97%E5%BD%A2%E7%8A%B6%E6%95%88%E6%9E%9C/hexagon.jpg)
```
.hexagon {
        width: 100px;
        height: 55px;
        background: #fc5e5e;
        position: relative;
}
  
.hexagon:before {
        content: "";
        width: 0;
        height: 0;
        position: absolute;
        top: -25px;
        left: 0;
        border-left: 50px solid transparent;
        border-right: 50px solid transparent;
        border-bottom: 25px solid #fc5e5e;
}
.hexagon:after {
        content: "";
        width: 0;
        height: 0;
        position: absolute;
        bottom: -25px;
        left: 0;
        border-left: 50px solid transparent;
        border-right: 50px solid transparent;
        border-top: 25px solid #fc5e5e;
}      
```
![](https://github.com/lc-dmx/css/blob/master/css%E7%B3%BB%E5%88%97%E5%BD%A2%E7%8A%B6%E6%95%88%E6%9E%9C/infinity.jpg)
```
.infinity {
	width: 220px;
	height: 100px;
	position: relative;
}

.infinity:before {
	content: "";
	width: 60px;
	height: 60px;
	position: absolute;
	top: 0;
	left: 0;
	border: 20px solid #06c999;
	-moz-border-radius: 50px 50px 0;
	border-radius: 50px 50px 0 50px;
	-webkit-transform: rotate(-45deg);
	-moz-transform: rotate(-45deg);
	-ms-transform: rotate(-45deg);
	-o-transform: rotate(-45deg);
	transform: rotate(-45deg);
}

.infinity:after {
	content: "";
	width: 60px;
	height: 60px;
	position: absolute;
	top: 0;
	left: 120px;
	border: 20px solid #06c999;
	-moz-border-radius: 50px 50px 50px 0;
	border-radius: 50px 50px 50px 0;
	-webkit-transform: rotate(45deg);
	-moz-transform: rotate(45deg);
	-ms-transform: rotate(45deg);
	-o-transform: rotate(45deg);
	transform: rotate(45deg);
}
```
![](https://github.com/lc-dmx/css/blob/master/css%E7%B3%BB%E5%88%97%E5%BD%A2%E7%8A%B6%E6%95%88%E6%9E%9C/search.jpg)
```
.search{
	position: relative;
}

.search:before{
	content:"";
	position: absolute;
	width: 90px;
	height: 90px;
	border: 1px solid #666;
	border-radius: 100%;
	box-shadow: 1px 1px 30px rgba(0,0,0,0.3) inset;
}

.search:after{
	content:"";
	position: absolute;
	width: 80px;
	height: 15px;
	background: #666;
	border-radius: 5px 0 0 5px;

 	transform: rotate(210deg);
 	-webkit-transform: rotate(210deg);
   	-moz-transform: rotate(210deg);
   	-ms-transform: rotate(210deg);
  	-o-transform: rotate(210deg);
}

.search:before {
    top: 0;
    left: 0;
}
.search:after {
    left: 78px;
    top:83px;
}
```
![](https://github.com/lc-dmx/css/blob/master/css%E7%B3%BB%E5%88%97%E5%BD%A2%E7%8A%B6%E6%95%88%E6%9E%9C/sixStar.jpg)
```
.sixStar {
	width: 0;
	height: 0;
	display: block;
	position: absolute;
	border-left: 50px solid transparent;
	border-right: 50px solid transparent;
	border-bottom: 100px solid #de34f7;
	margin: 10px auto;
}
.sixStar:after {
	content: "";
	width: 0;
	height: 0;
	position: absolute;
	border-left: 50px solid transparent;
	border-right: 50px solid transparent;
	border-top: 100px solid #de34f7;
	margin: 30px 0 0 -50px;
} 
```
![](https://github.com/lc-dmx/css/blob/master/css%E7%B3%BB%E5%88%97%E5%BD%A2%E7%8A%B6%E6%95%88%E6%9E%9C/star.jpg)
```
.star{
	width: 0;
	height: 0;
	margin: 50px;
	color: #fc2e5a;
	position: relative;
	display: block;
	border-right: 100px solid transparent;
	border-bottom: 70px solid #fc2e5a;
    	border-left: 100px solid transparent;
	transform: rotate(35deg);
	-webkit-transform: rotate(35deg);
	-moz-transform: rotate(35deg);
	-ms-transform: rotate(35deg);
	-o-transform: rotate(35deg);
}
.star:before {
	content: '';
	width: 0;
	height: 0;
	position: absolute;
	display: block;
	top: 3px;
	left: -105px;
	color: #fc2e5a;
	border-right: 100px solid transparent;
	border-bottom: 70px solid #fc2e5a;
	border-left: 100px solid transparent;
	transform: rotate(-70deg);
	-webkit-transform: rotate(-70deg);
	-moz-transform: rotate(-70deg);
	-ms-transform: rotate(-70deg);
	-o-transform: rotate(-70deg);
}   



.star:after{
	content: '';
	height: 0;
	width: 0;
	position: absolute;
	display: block;
	top: -45px;
	left: -62px;
	border-bottom: 80px solid #fc2e5a;
	border-left: 30px solid transparent;
	border-right: 30px solid transparent;
	transform: rotate(-35deg);
	-webkit-transform: rotate(-35deg);
	-moz-transform: rotate(-35deg);
	-ms-transform: rotate(-35deg);
	-o-transform: rotate(-35deg);
}
```
