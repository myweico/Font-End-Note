- 语义化标签的作用
    - 可读性、可维护性
    - 有助于seo

- 条件注释,可以避免多余的加载
```html
<!--[if lte ie 8]>
    <script src="htmlshiv.min.js"></script>
<![endif]-->
```
- 即使图片可以显示特殊的内容，但是搜索爬虫不会识别，可以填写一些标签，例如h1来描述图片的主要内容，然后将其隐藏即可

- 图片显示的方式
    - 直接使用图片标签元素，会全部显示出来
    - div+img，需要使用定位规定图片显示的位置
    - div的background，可以重复，可以快速使用定位，但是无法超过容器

- 当图片尺寸超过容器的时候默认会全部显示出来，溢出了也没关系
- 使用steller插件实现滚差效果   




## 注意的点
- 使用父元素float后，子元素也会继承float属性，显示的顺序会有所改变
- img若过大，不会自动进行缩放显示，而是会按照原来的尺寸裁切显示一部分，若想显示全部内容可以设置宽或高为100%,另一半会自动进行缩放，这是图片的一个特殊的属性
- 可以添加有些隐藏的标签以便于seo
- background-size, cover尺寸不变扩展到容器都铺满图片时停止，contain尺寸不变图片一边碰到容器停止