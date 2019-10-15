复杂页面的实现
====
<ol>
<li>铺满屏幕：height: calc(100vh);<br/></li>
<li>div里含左右2个div，左栏高度随右栏高度自适应，bug：左栏底部内容隐藏</li>
  float: left;<br/>
  margin-bottom: -9999px;<br/>
  padding-bottom: 9999px;<br/>
<li>实现子元素在父元素垂直居中</li>
  position: absolute;<br/>
  top: 50%;<br/>
  transform: translateY(-50%);<br/>
<li>修改a链接样式</li>
  .button:link, .button:visited {<br/>
    text-decoration: none;<br/>
    color: #b7c0cd;<br/>
  }<br/>
  .button:hover, .button:active {<br/>
    position: relative;<br/>
    color: #fff;<br/>
  }<br/>
<li>flex对齐方式</li>
  垂直居中：align-items: center;<br/>
  顶部对齐：align-items: flex-start;<br/>
<li>滚动条</li>
  .scroll {<br/>
      /*滚动条*/<br/>
      overflow-x: hidden;<br/>
      overflow-y: auto;<br/>
      /*隐藏滚动条，其width：16px*/<br/>
      margin-right: -16px;<br/>
      width: calc(100% + 16px);<br/>
      height: 100%;/*81px*/<br/>
  }<br/>
<li>鼠标接触显示另一图片</li>
  .photo {position: relative;}<br/>
  .p_hover {display: none;}<br/>
  .photo:hover .p_hover { /*photo为p_hover的父元素*/<br/>
    position: absolute; /*绝对定位*/<br/>
    left: 0;<br/>
    top: 0;<br/>
    display: block;<br/>
    width: 100%;<br/>
    height: 100%;<br/>
    background-color: rgba(0,0,0,0.65);/*蒙黑色阴影*/<br/>
  }<br/>
<li>图片水平垂直居中</li>
  .parent {text-align: center;}<br/>
  .parent .img {<br/>
    position: absolute;<br/>
    top: 0;<br/>
    bottom: 0;<br/>
    left: 0;<br/>
    right: 0;<br/>
    margin: auto;<br/>
  }<br/>
