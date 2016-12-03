# svgToBase64 介绍

最近想在 sass 中使用内联的svg。 sass 默认不自带这个功能，所以自己写了一个。使用方式很简单，如下：

```sass

.test {
	background: url(svgToBase64('<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" preserveAspectRatio="xMidYMid" viewBox="0 0 750 400"><path d="M0,0 L750,0 L750,400 L388,400 L375,387, L362,400 L0,400Z" fill="#0f0"></path></svg>'));
	background-size: 100px 100px;
}

```