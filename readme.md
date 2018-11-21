# background

background 简写属性在一个声明中设置所有的背景属性。

可以设置如下属性：

background-color
background-position
background-size
background-repeat
background-origin
background-clip
background-attachment
background-image

# background-color

```css
body
  {
  background-color:yellow;
  }
h1
  {
  background-color:#00ff00;
  }
p
  {
  background-color:rgb(255,0,255);
  }
```

# background-position

设置背景图像的起始位置

| 可能取到的值  | 描述  |
| :------------ |:---------------:|
| (top left) (top center) (top right) (center left) (center center) (center right) (bottom left) (bottom center) (bottom right)      | 如果只规定了一个关键词，则第二个关键词默认为center |
| x% y%      | 第一个值是水平位置，第二个值是垂直位置；左上角是 0% 0%。右下角是 100% 100%；如果您仅规定了一个值，另一个值将是 50%。       |
| xpos ypos | 第一个值是水平位置，第二个值是垂直位置；左上角是 0 0。单位是像素 (0px 0px) 或任何其他的 CSS 单位；如果您仅规定了一个值，另一个值将是50%；您可以混合使用 % 和 position 值。       |

# background-size

```css
background-size：100% 100%;
```

按容器比例撑满，图片变形；

```css
background-size：100% auto;
```

第一个值为x轴方向的缩放比例或者px,第二个值为y轴方向的缩放比例或者px，如果只写一个值，则第二个值默认为auto(根据图片原来的比例，以及现有的宽度，来确定高度)


```css
background-size：cover;
```
把背景图片放大到适合元素容器的尺寸，图片比例不变，但是要注意，超出容器的部分可能会裁掉。

# background-repeat

| 可能取到的值  | 描述  |
| :------------ |:---------------:|
| repeat  | 默认。背景图像将在垂直方向和水平方向重复。 |
| repeat-x  | 背景图像将在水平方向重复。   |
| repeat-y | 背景图像将在垂直方向重复。|
| no-repeat	 | 背景图像将仅显示一次。|

# background-image

```css
background-image: url("../img/bg.jpg")
```

# 参考文献

http://www.w3school.com.cn/cssref/pr_background.asp