- 使用class来改变动画样式
- 动画要使用位移而不是定位
- 动画默认会变为原来的样式，若没有设置最后的关键帧，则将一开始的样式作为最后的关键帧、
- 若一开始的关键帧与最后的关键帧与原来的样式有冲突的话，会有一个突变的瞬间
- 建议动画使用位移不要使用定位（暂时不知道为什么）
- css3当中监听动画的结束 过渡 transitionend  动画 animationend
- 背景图的百分比不是按照容器的宽度来计算的，其是容器宽度减去背景的宽度再乘以百分比来计算的
- keyframes中的动画总是相对于最开始的样式
- transform中的动画中使用translate时，最开始最好写上translate(0,0)，否则会看不到效果
- fadeIn()和display:none配合才有效果，与opacity:0配合无效
- jq中的动画通过类名、css属性以及动画方法实现，后面两种都是通过改变style属性进行
- removeSAttr比attr("name","")更干净
- border-image的切割顺序位上右下左，round会缩小凑够整数平铺，repeated平铺会从中间进行平铺，大小不变