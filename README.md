# LanYunGeZhu.github.io
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>下拉菜单</title>
<style>
*{
margin: 0;
padding: 0;
list-style: none;
}
.nav{
width: 430px;
height: 40px;
background: skyblue;
margin: 100px auto;
text-align: center;
line-height: 40px;

}
a{
color: #fff;
text-decoration: none;

}
.nav li{
width: 100px;
height: 40px;
background: skyblue;

}
.nav>li{
float: left;
margin-right: 10px;
/*相对位置*/
position: relative;
}
.nav>li:last-child{
margin-right: 0;
}
.nav li ul{
/*绝对位置*/
position: absolute;
left: 0;
top: 40px;
display: none;
}
</style>
</head>
<body>

<ul class="nav">
<!---->
<li>
<a href="javascript:;">首页</a>
</li>
<!---->
<li id="li1">
<a href="javascript:;">UI设计</a>
<ul id="ul1">
<li><a href="javascript:;">界面设计-1</a></li>
<li><a href="javascript:;">界面设计-2</a></li>
<li><a href="javascript:;">界面设计-3</a></li>
</ul>
</li>
<!---->
<li id="li2">
<a href="javascript:;">WEB前端</a>
<ul id="ul2">
<li><a href="javascript:;">HTML5-1</a></li>
<li><a href="javascript:;">HTML5-2</a></li>
<li><a href="javascript:;">HTML5-3</a></li>
</ul>
</li>
<!---->
<li id="li3">
<a href="javascript:;">公开课</a>
<ul id="ul3">
<li><a href="javascript:;">网页设计-1</a></li>
<li><a href="javascript:;">网页设计-2</a></li>
<li><a href="javascript:;">网页设计-3</a></li>
</ul>
</li>

</ul>


<script>
//            //
//            var oLi1 = document.getElementById('li1');
//            var oUl1 = document.getElementById('ul1');
//            
//            oLi1.onmouseover = function(){
//                oUl1.style.display = 'block';
//            }
//            oLi1.onmouseout = function(){
//                oUl1.style.display = 'none';
//            }
//            //
//            var oLi2 = document.getElementById('li2');
//            var oUl2 = document.getElementById('ul2');
//            
//            oLi2.onmouseover = function(){
//                oUl2.style.display = 'block';
//            }
//            oLi2.onmouseout = function(){
//                oUl2.style.display = 'none';
//            }
//            //
//            var oLi3 = document.getElementById('li3');
//            var oUl3 = document.getElementById('ul3');
//            
//            oLi3.onmouseover = function(){
//                oUl3.style.display = 'block';
//            }
//            oLi3.onmouseout = function(){
//                oUl3.style.display = 'none';
//            }

//优化上面三段重复性代码
function nav(liID,ulID){
var oLi = document.getElementById(liID);
var oUl = document.getElementById(ulID);

oLi.onmouseover = function(){
oUl.style.display = 'block';
}
oLi.onmouseout = function(){
oUl.style.display = 'none';
}
}
nav('li1','ul1');
nav('li2','ul2');
nav('li3','ul3');


</script>


</body>
</html>


