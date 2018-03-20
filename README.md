# Pt-my-first-web2.0
第一个网页 单纯的css实现的静态页面 主要是稍稍体会一下实战的感觉 以后慢慢的加上一些js效果 争取做成更加丰满的网页。</br>
梳理一下主要碰到的问题：</br>
1、整个背景图的大小为1920  给定了最小宽度 1200 即浏览器宽度增大到1200后 底部不出现滚动条</br>
当某一元素的实际宽度超过1200后 窗口大小在1200以上时整个网页不会同步缩放 右侧会出现白色的空白区域</br>
解决： 给超出元素的父级添加 overflow：hidden  比较暴力的方法：给整个Html添加超出隐藏</br>

2、布局技巧： 1) 父相子绝 （据说定位还是少用的好）</br>
2) 类似ul li 结构 li浮动，防止宽度不够li掉块的做法： ul设置的宽一些（200%）,然后让ul父级超出隐藏 能防止几px的误差导致的掉块。</br>
3)小图标一般用span</br>
4) 配图的文字（绝对定位于图片上方）整体上下移动效果（hover）  文字盒子给定一个初始高度  transition：translate（0，-100%)将其抬高一个身位
此时为正常状态（隐藏一大部分）  hover后还原（全部显示在屏幕），大概是这个意思。。

