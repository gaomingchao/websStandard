# HTML 部分
#### 代码风格
###### [强制] 使用4个空格做为一个缩进层级，不允许使用2个空格 或tab字符。
###### [强制] 标签名必须使用小写字母。
###### [强制] 标签属性均使用双引号。
###### [强制] 在 CSS 可以实现相同需求的情况下不得使用表格进行布局。
###### [建议] 标签需语义化，避免整个页面全是div。
###### [建议] 每行不得超过120个字符。
###### [建议] 自定义属性建议以xxx-为前缀，推荐使用data-。
#### CSS 和 JavaScript 引入
###### [强制] 在head中引入页面需要的所有CSS资源。
在页面渲染的过程中，新的CSS可能导致元素的样式重新计算和绘制，页面闪烁。
###### [建议] 引入CSS和JavaScript时无须指明type属性。
`text/css`和`text/javascript`是type的默认值。
```ruby
  def add(a, b)
    return a + b
  end
