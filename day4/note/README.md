# 背景边框链接和更复杂的选择器
## w3school
### css背景
  背景色：background-color:gray;背景图片:  
  background-image:url(图片地址); 背景重复:background-repeat:repeat-y;可以向x,y方向来重复背景图片。

  值|描述
  ---|---
  repeat|默认。背景图像将在垂直和水平方向重复
  repeat-x|背景图像将在水平方向重复


  ![Alt text](images/b_css.png)
  #### 背景图片的位置:background-position:
  你需要把background-attachment属性设置为"fixed"，才能保证该属性在Firefox和Opera 正常工作，当内容滚动时，指定元素背景的行为，例如，它是滚动的内容，还是固定的?
  ![Alt text](images/css_b.png)  
  坐标位置:图像的左上角是原点(0,0)。把背景想象成一个图形，先从左到右，y坐标从上到下  

  该属性可以接受不同类型的值:  
  像px这样的绝对值:background-position:200px 25px;  
  像rems这样的相对值:background-position:20rem 2.5rem;  
  百分比:background-position:90%  25%;  
  关键字:background-postion:right center;  


# MDN什么是背景
##什么是背景？
background-clip:可以改变背景所占用的区域（设置元素的背景（背景图片或者是颜色）是否要延伸到边框下面）
background-clip:border-box;背景延伸到边框外沿（但在边框之下)  
background-clip:padding-box;边框下面没有背景，即背景延伸到内边距外沿  
background-clip:content-box;背景裁剪到内容区外沿  
background-clip:tex;背景被裁剪为文字的前景色（只有chrome支持）  
##背景图像:渐变  
###线性渐变:  
线性渐变是通过linear-gradient()函数传入的，它是一个background-image属性的值。函数至少需要用逗号来分隔的3个参数:背景中渐变的方向，开始颜色和结尾颜色。  
例如:background-image:linear-gradient(to bottom,orange,yellow);  
这个渐变将从上到下，从顶部的橙色开始，然后平稳的过渡到底部的黄色。可以使用关键字制定方向（to bottom,to right,to bottom right等）,或角度值（0deg相当于to top,90deg相当于  to right,直到360deg，它相当于to top）  
你也可以在颜色定义的渐变中指定其他的点——这些被称为颜色站点(color stops)，浏览器会计算出每一组颜色站点之间的颜色渐变。比如：  
background-image:liner-gradient(to bottom,yellow,orange 40%,yellow);  
注意:你还可以使用repeating-linear-gradient()函数来设置一个重复的线性渐变。它的工作方式完全相同，只不过你设置的模式会不断重复，直到背景的边框。例如:  
background-image:reqeating-linear-gradient(to fight,yellow,orange 25%,yellow 50%);  
这将会产生一个渐变，从黄色到橙色，在沿着渐变的每50个像素再回来  
##背景附着  
background-attachment:属性是指定当内容滚动时他们是如何滚动的。有以下三种情况:  
scroll:会把背景修改为页面视图，背景不会滚动，只是文本内容滚动  
fixed:可以在页面的位置上固定背景，所以当页面滚动时，他不会滚动。  
local:  
##背景简写  
background:yellow linear-gradient(to bottom,orange,yellow) no-repeat left center scoll;  
##多个背景  
可以用逗号来分隔不同的背景定义  

background:rul(image.png) no-repeat 99% center,url(background-tile.png),linear-gradient(to bottom,yellow,#dddd00 50%,orange);  
也可以像普通的写法那样来写:  
background-image:url(),rul();  
background-repeat:no-repeat,repeat;  
##背景尺寸  
background-size:16px 16px;  
 
 
