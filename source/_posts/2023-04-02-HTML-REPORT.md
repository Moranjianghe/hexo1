title: Pacific Trails Resort 网页实验报告
lang: zh-CN
date: 2023-04-02 18:48:02
tags: [HTML, CSS, lab-report]
---
## 实验目的

本次网页实验的目的是创建一个旅游度假胜地的网站，展示该度假胜地的照片和相关信息，提供在线预定服务。

## 实验过程

1. 创建 HTML 文件并添加所需元素，如头部、主体和页脚。
2. 为 HTML 添加样式，如背景色、字体、边距和大小。
3. 使用 CSS 创建一个导航栏和按钮，提供页面导航和在线预定服务。
4. 添加图像，创建一个带有照片展示的区域，展示该度假胜地的美景。
5. 复制 index.html 进并行简单的修改，获得 activities.html、reservations.html、yurts.html

## 实验结果

本次实验创建了几个简单的旅游度假胜地网页，分别包括以下几个部分：

* 头部：包括网页标题和导航栏，提供导航和在线预定服务。
* 主体：包括欢迎语、关于我们、预定按钮、内容介绍等。
* 页脚：包括版权信息和网站制作者（我）的信息。

### styles.css

```css
body {
	font-family: Arial, sans-serif;
	margin: 0;
	padding: 0;
}

header {
	background-color: #0077be;
	color: #fff;
	padding: 10px 20px;
}

nav ul {
	list-style: none;
	margin: 0;
	padding: 0;
}

nav li {
	display: inline-block;
	margin-right: 20px;
}

nav li:last-child {
	margin-right: 0;
}

nav a {
	color: #fff;
	text-decoration: none;
}

main {
	max-width: 1200px;
	margin: 0 auto;
	padding: 20px 20px 0;
}

section {
	margin-bottom: 40px;
}

h2 {
	font-size: 36px;
	margin-bottom: 20px;
}

p {
	font-size: 18px;
	line-height: 1.5;
	margin-bottom: 20px;
}

.cta {
	background-color: #0077be;
	color: #fff;
	display: inline-block;
}

img {
	max-width: 100%;
	height: auto;
}

footer {
	margin-top: auto;
	text-align: center;
	padding: 20px;
	background-color: #f1f1f1;
}
```

这是一个网站的样式表，用于定义网站各个部分的样式和布局。以下是每个部分的解释：

* `body`: 设置页面主体部分的样式，包括字体、页边距和内边距。
* `header`: 设置网站头部区域的样式，包括背景颜色、文本颜色和内边距。
* `nav ul`: 设置导航栏列表的样式，包括去除列表样式、页边距和内边距。
* `nav li`: 设置导航栏列表项的样式，包括将列表项呈现为内联块、右边距和左右对齐。
* `nav li:last-child`: 设置导航栏的最后一个列表项的样式，将其右边距设置为0，避免在导航栏的最右侧出现多余的空白。
* `nav a`: 设置导航栏链接的样式，包括文本颜色和去除下划线。
* `main`: 设置网站主要内容区域的样式，包括最大宽度、水平居中和内边距。
* `section`: 设置每个内容区块的样式，包括底部外边距。
* `h2`: 设置二级标题的样式，包括字体大小和底部外边距。
* `p`: 设置段落文本的样式，包括字体大小、行高和底部外边距。
* `.cta`: 设置一个带有背景颜色和文本颜色的按钮。
* `img`: 设置图像的样式，将其最大宽度设置为100%，并根据宽高比自适应高度。
* `footer`: 设置网站页脚区域的样式，包括顶部外边距、文本居中和背景颜色。

以上是样式表中的主要样式设置，它们的作用是定义网站的各个部分的样式和布局，以使网站呈现出整体统一、美观、易读和易用的外观。

### index.html

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>Pacific Trails Resort</title>
	<link rel="stylesheet" href="styles.css">
</head>
<body>
	<header>
		<h1>Pacific Trails Resort</h1>
		<small>Web page made by Moran Xia</small>
		<nav>
			<ul>
				<li><a href="index.html">主页</a></li>
				<li><a href="yurts.html">圆顶帐篷</a></li>
				<li><a href="activities.html">活动</a></li>
				<li><a href="reservations.html">预定</a></li>
			</ul>
		</nav>
	</header>
	<main>
		<section id="hero">
			<h2>欢迎来到 Pacific Trails Resort</h2>
			<p>逃离城市的喧嚣，来到被大自然包围的宁静之地。在户外体验奢华的生活。</p>
			<a href="reservations.html" class="cta">现在预定</a>
		</section>
		<section id="about">
			<h2>关于我们</h2>
			<p>Pacific Trails Resort 是位于加利福尼亚北部美丽海岸线上的一家高级度假胜地。我们提供舒适的圆顶帐篷和高档餐饮住宿设施。我们的度假村非常适合喜欢户外活动和安静环境的情侣或夫妇。</p>
			<a href="yurts.html" class="cta">了解更多</a>
		</section>
		<section id="gallery">
			<h2>照片展示</h2>
			<div class="gallery-container">
				<img src="images\sea-1598758.jpg" alt="Pacific Trails Resort">
				<img src="images\vacation-2218746.jpg" alt="Pacific Trails Resort">
				<img src="images\pacific-2190967.jpg" alt="Pacific Trails Resort">
				<img src="images\california-1596181.jpg" alt="Pacific Trails Resort">
			</div>
		</section>
	</main>
	<footer>
		<p>&copy; 2023 Moran Xia Resort.</p>
	</footer>
</body>
</html>
```
![](reportimg/index.png)
这是一个 HTML 网页，作为网站主页，用于介绍。下面是该 HTML 网页的主要部分：

* head：HTML head 部分包含了一些元数据和样式表的引用。在这个网页中，head 中定义了该网页的编码方式、视口大小，网页标题和一个名为 styles.css 的样式表的引用。
  
* header：HTML header 部分通常包含了一些重要的内容，例如网页的标题和导航栏等。在这个网页中，header 中包含了网页的标题、作者信息和一个简单的导航菜单。
  
* main：HTML main 部分通常包含了网页的主要内容。在这个网页中，main 中包含了网站的三个主要部分，分别是欢迎页面、关于页面和照片展示页面。
  
* section：HTML section 元素是一种通用的容器元素，通常用于将网页内容分成不同的部分。在这个网页中，section 元素被用于分离不同的页面部分，例如欢迎页面、关于页面和照片展示页面。
  
* h2 和 p：HTML h2 和 p 元素分别用于定义标题和段落。在这个网页中，h2 和 p 元素被用于定义各个部分的标题和内容。
  
* a：HTML a 元素用于定义超链接，可以让用户通过点击链接跳转到其他网页。在这个网页中，a 元素被用于定义导航菜单中的链接和 CTA 按钮。
  
* img：HTML img 元素用于在网页中嵌入图片。在这个网页中，img 元素被用于嵌入照片展示页面中的图片。
  
* footer：HTML footer 元素通常包含了网站的一些脚注信息。在这个网页中，footer 中包含了版权信息。

### activities.html

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>Pacific Trails Resort - 活动</title>
	<link rel="stylesheet" href="styles.css">
</head>
<body>
	<header>
		<h1>Pacific Trails Resort</h1>
		<small>Web page made by Moran Xia</small>
		<nav>
			<ul>
				<li><a href="index.html">主页</a></li>
				<li><a href="yurts.html">圆顶帐篷</a></li>
				<li><a href="activities.html">活动</a></li>
				<li><a href="reservations.html">预定</a></li>
			</ul>
		</nav>
	</header>
	<main>
		<section id="hero">
			<h2>体验户外活动的乐趣</h2>
			<p>在 Pacific Trails Resort，我们提供各种户外活动，让您与大自然亲密接触，感受自然之美，让您的假期更加难忘。</p>
			<a href="reservations.html" class="cta">预定活动</a>
		</section>
		<section id="activities">
			<h2>我们的活动</h2>
			<ul>
				<li>
					<h3>远足</h3>
					<img src="images\mountaineering-455338.jpg" alt="远足">
					<p>加利福尼亚北部美丽的海岸线和茂密的森林提供了各种难度的远足径，适合各种能力的人。</p>
				</li>
				<li>
					<h3>钓鱼</h3>
					<img src="images\angler-3071970.jpg" alt="钓鱼">
					<p>在我们的私人湖中放松心情，享受钓鱼的乐趣。我们的湖里有各种鱼类，如鲑鱼、鳟鱼和鲈鱼。</p>
				</li>
				<li>
					<h3>皮划艇</h3>
					<img src="images\girl-1561989.jpg" alt="皮划艇">
					<p>在太平洋海岸的平静水域上划皮划艇，欣赏海岸线上的美景。</p>
				</li>
				<li>
					<h3>自行车</h3>
					<img src="images\man-5610626.jpg" alt="自行车">
					<p>通过自行车体验森林中的山地道路，让您在大自然中感受自由与兴奋。</p>
				</li>
			</ul>
			<a href="reservations.html" class="cta">预定活动</a>
		</section>
	</main>
	<footer>
		<p>&copy; 2023 Moran Xia Resort.</p>
	</footer>
</body>
</html>
```

![](reportimg/activities.png)

各部分功能结构与 index.html 基本相同。
用于介绍各项活动。

### reservations.html

```html
<!DOCTYPE html>
<html lang="zh-CN">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pacific Trails Resort</title>
    <link rel="stylesheet" href="styles.css">
</head>

<body>
    <header>
        <h1>Pacific Trails Resort</h1>
		<small>Web page made by Moran Xia</small>
        <nav>
            <ul>
                <li><a href="index.html">主页</a></li>
                <li><a href="yurts.html">圆顶帐篷</a></li>
                <li><a href="activities.html">活动</a></li>
                <li><a href="reservations.html">预定</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section id="hero">
            <h2>欢迎来到 Pacific Trails Resort</h2>
            <p>逃离城市的喧嚣，来到被大自然包围的宁静之地。在户外体验奢华的生活。</p> <a href="mailto:info@pacifictrails.com" class="cta">邮件预定</a>：info@pacifictrails.com
        </section>
        <section id="about">
            <h2>关于我们</h2>
            <p>Pacific Trails Resort 是位于加利福尼亚北部美丽海岸线上的一家高级度假胜地。我们提供舒适的圆顶帐篷和高档餐饮住宿设施。我们的度假村非常适合喜欢户外活动和安静环境的情侣或夫妇。</p> <a
                href="yurts.html" class="cta">了解更多</a>
        </section>
    </main>
    <footer>
        <p>&copy; 2023 Moran Xia Resort.</p>
    </footer>
</body>

</html>
```
![](reportimg\reservations.png)

各部分功能结构与 index.html 基本相同。  
使用了 mailto 链接，用于客户快速打开邮箱。

### yurts.html

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>Pacific Trails Resort - 圆顶帐篷</title>
	<link rel="stylesheet" href="styles.css">
</head>
<body>
	<header>
		<h1>Pacific Trails Resort</h1>
		<small>Web page made by Moran Xia</small>
		<nav>
			<ul>
				<li><a href="index.html">主页</a></li>
				<li><a href="yurts.html">圆顶帐篷</a></li>
				<li><a href="activities.html">活动</a></li>
				<li><a href="reservations.html">预定</a></li>
			</ul>
		</nav>
	</header>
	<main>
		<section id="hero">
			<h2>圆顶帐篷</h2>
			<p>我们的圆顶帐篷是由最好的材料制成，非常舒适，适合情侣或夫妇入住。每个帐篷都设有独立的浴室和淋浴设施。</p>
			<a href="reservations.html" class="cta">现在预定</a>
		</section>
		<section id="yurts">
			<h2>我们的圆顶帐篷</h2>
			<div class="yurt-container">
				<div class="yurt">
					<img src="images\treehouse-livingroom.jpg" alt="圆顶帐篷1">
					<h3>豪华圆顶帐篷</h3>
					<p>我们的豪华圆顶帐篷提供豪华的床铺、柔软的毛毯和舒适的家具。它们还配备了一个小厨房，让您可以在度假时自行烹饪。</p>
				</div>
				<div class="yurt">
					<img src="images\yurt-interior.jpg" alt="圆顶帐篷2">
					<h3>标准圆顶帐篷</h3>
					<p>我们的标准圆顶帐篷提供基本的床铺和设施，是预算友好型的选择。它们还提供一个室外烧烤区，供您在户外享用烧烤晚餐。</p>
				</div>
			</div>
		</section>
	</main>
	<footer>
		<p>&copy; 2023 Moran Xia Resort.</p>
	</footer>
</body>
</html>
```
![](reportimg\yurts.png)

各部分功能结构与 index.html 基本相同。  
介绍了圆顶帐篷。

## 实验总结

本次实验通过使用 HTML 和 CSS 创建了一个简单的旅游度假胜地网站，包括页面导航、在线预定服务和照片展示等部分。在实验过程中，学习了如何使用 HTML 和 CSS 创建基本的网页结构和样式，了解了如何使用不同的标记和属性，以及如何使用 CSS 创建不同的样式。通过实验，加深了对 HTML 和 CSS 的理解和掌握，提高了对网页开发的认识和技能。  
