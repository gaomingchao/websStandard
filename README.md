# HTML 部分
> 代码风格
##### [强制] 使用4个空格做为一个缩进层级，不允许使用2个空格 或tab字符。
##### [强制] 标签名必须使用小写字母。
##### [强制] 标签属性均使用双引号。
##### [强制] 在 CSS 可以实现相同需求的情况下不得使用表格进行布局。
##### [建议] 标签需语义化，避免整个页面全是div。
##### [建议] 每行不得超过120个字符。
##### [建议] 自定义属性建议以xxx-为前缀，推荐使用data-。
> CSS 和 JavaScript 引入
##### [强制] 在head中引入页面需要的所有CSS资源。
###### 在页面渲染的过程中，新的CSS可能导致元素的样式重新计算和绘制，页面闪烁。
##### [建议] 引入CSS和JavaScript时无须指明type属性。
###### `text/css`和`text/javascript`是type的默认值。
```<script src="//cdn.bootcss.com/jqueryui/1.12.1/jquery-ui.css"></script>```
> 图片
##### [建议] 避免为img添加不必要的title属性。
###### 多余的title影响看图体验，并且增加了页面尺寸。
##### [建议] 为重要图片添加alt属性。
###### 可以提高图片加载失败时的用户体验。
##### [建议] 添加width和height属性，以避免页面抖动。

# CSS 部分
##### [强制]使用link的方式调用外部样式。
##### [强制]使用4个空格做为一个缩进层级，不允许使用2个空格 或tab字符。
##### [强制]选择器与{之间必须包含空格。
``` 
.selector {
} 
```
##### [强制]属性名与之后的:之间不允许包含空格，:与属性值之间必须包含空格。如：`margin: 0;`
##### [强制]无继承关系时，使用缩写 如：`margin:10px 20px;`。
##### [强制]如果属性值为0，则不要为0加单位。
##### [建议]如果是0开始的小数，前面的0可以省略不写 如：`opacity:.5;`。
##### [建议]不要在url()里对引用资源加引号 如：`background-image: url(sprites.png);`。
##### [建议]多组选择器之间需换行。
```
h1,
h2,
h3 {
}
```
##### [建议]在不考虑低版本浏览器兼容的情况下，避免无意义的空标签出现，用::after和::before代替；
##### [建议]尽量避免使用class和标签名组合使用；
###### 不要这样 `div.nav`;
##### CSS书写顺序；
1. 位置属性(position, top, right, z-index, display, float等)
2. 盒模型(width, height, padding, margin,border)
3. 文字系列(font, line-height, letter-spacing, color- text-align等)
4. 背景(background等)
5. 其他(animation, transition等)

# class类名命名规则
##### 简单模块：在子孙模块数量可预测的情况下，继承祖先模块命名的前缀，用“-”分割（不要用下划线“_”）；
```
<div class="slider">
    <ul class="slider-list">
        <li class="slider-item"></li>
    </ul>
</div>
```
##### 复杂模块：当子孙模块过多且无法预估的时候，采用“祖先+父”作为命名前缀；
```
<div class="slider">
     <ul class="slider-list">
         <li class="slider-item">
             <div class="slider-item-left">
                  <span class="slider-left-tips"></span>
             </div> 
         </li>
     </ul>
</div>
```
##### 全站公共模块以 mod- 开头；
##### 页面公共模块以 xx-mod- 开头 （xx页面名字）；
##### 命名用英文，较长的使用缩写;

