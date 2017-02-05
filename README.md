## 效果图
![image](http://ok7n02kz6.bkt.clouddn.com/loq2-mW0ahXlLzYt4Xoi60aJgcyd.gif)

## CSS部分
1. flexbox
使用`flex`可以使各元素占有一定的比例。主要步骤:
2. 将父元素`.panels`设置为`display:flex`
3. 将每个子元素的`flex:1`,设置其`flex-direction:column`
4. 控制`.panle` 的子元素 <p> 中的文字垂直、水平居中
设置为 `display:flex`
设置`flex`值
设置其子元素的布局方式：垂直水平居中（沿主轴、侧轴居中）
5. 设定点击图片后文字移动的样式`transform: translateY(-100%)`
6. 设定点击图片展开后的图片的 flex 值

## js部分
1. 获取所有类名为`panel`的元素
2. 为其添加`click`事件监听，编写触发事件调用的函数（给触发的 DOM 元素添加/去掉样式，实现拉伸/压缩的效果）
3. 为其添加`transitionend`事件监听，编写调用的函数（添加/去掉样式，实现文字的飞入/飞出效果）
PS:`transitionend`事件在CSS完成过渡后触发。