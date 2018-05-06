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
# MDN什么是背景
##什么是背景？
background-clip:可以改变背景所占用的区域（设置元素的背景（背景图片或者是颜色）是否要延伸到边框下面）
background-clip:border-box;背景延伸到边框外沿（但在边框之下)  
background-clip:padding-box;边框下面没有背景，即背景延伸到内边距外沿  
background-clip:content-box;背景裁剪到内容区外沿  
background-clip:tex;背景被裁剪为文字的前景色（只有chrome支持）