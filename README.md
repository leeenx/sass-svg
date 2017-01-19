# sass-svg 介绍

这里包含两个文件：`sass-svg-encodeuri.scss` 与 `sass-svg-base64.scss`。是实现 svg 转 Data-URI 的两个库。

## sass-svg-encodeuri

将 svg 转换成 URL 编码的 sass 函数。

语法如下： 

```scss
sass-svg-encodeuri($svg-string);
```

实例：
```
$svg: '<svg viewBox="0 0 750 400" width="750" height="400">
			<path d="M0,0 L750,0 L750,400 L388,400 L375,387, L362,400 L0,400Z" fill="#0f0"></path>
		</svg>';
background: url(sass-svg-encodeuri($svg)) 0 0 no-repeat;
background-size: 100% 100%;
```


## sass-svg-base64

将 svg 转换成 base编码的 sass 函数。

语法如下： 

```scss
sass-svg-base64($svg-string);
```

实例：
```
$svg: '<svg viewBox="0 0 750 400" width="750" height="400">
			<path d="M0,0 L750,0 L750,400 L388,400 L375,387, L362,400 L0,400Z" fill="#0f0"></path>
		</svg>';
background: url(sass-svg-base64($svg)) 0 0 no-repeat;
background-size: 100% 100%;
```