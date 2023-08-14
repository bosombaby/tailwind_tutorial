# 一、前言
[Tailwind CSS - Rapidly build modern websites without ever leaving your HTML.](https://tailwindcss.com/)

Tailwind是一款CSS框架，它的主要特点是提供了一系列的CSS类，可以快速地构建出各种样式。Tailwind的发展历史可以追溯到2017年，由Adam Wathan、Steve Schoger和Jonathan Reinink共同创建。Tailwind的设计理念是提供一系列的原子类，每个类都只包含一个具体的样式，通过组合这些类来构建出复杂的样式。这种设计理念可以让开发者更加灵活地控制样式，同时也可以减少样式冗余，提高代码的可维护性。
Tailwind的主要特点包括：

- 提供了一系列的原子类，可以快速地构建出各种样式。
- 可以通过配置文件来自定义样式，包括颜色、字体、边框等。
- 支持响应式设计，可以根据不同的屏幕尺寸来应用不同的样式。
- 支持插件机制，可以扩展框架的功能。
- 提供了一些实用的工具类，如布局类、间距类、文本类等，可以帮助开发者更快地构建页面。

总的来说，Tailwind是一款非常实用的CSS框架，可以帮助开发者更快地构建页面，同时也可以提高代码的可维护性。
# 二、基础教程 上
## 2.1 颜色
**white, black, red, green, blue, orange, yellow, purple, lime, emerald, teal, cyan, indigo, violet, fuchsia, pink, rose, sky, gray, slate, zinc, neutral, stone, amber**
```html
<!-- Default colors -->
    <!-- white, black, red, green, blue, orange, yellow, purple, lime, emerald, teal, cyan, indigo, violet, fuchsia, pink, rose, sky, gray, slate, zinc, neutral, stone, amber,  -->

    <!-- Text Colors -->
    <p class="text-black">Tailwind is awesome</p>
    <p class="text-red-50">Tailwind is awesome</p>
    <p class="text-red-100">Tailwind is awesome</p>
    <p class="text-red-200">Tailwind is awesome</p>
    <p class="text-red-300">Tailwind is awesome</p>
    <p class="text-red-400">Tailwind is awesome</p>
    <p class="text-red-500">Tailwind is awesome</p>
    <p class="text-red-600">Tailwind is awesome</p>
    <p class="text-red-700">Tailwind is awesome</p>
    <p class="text-red-800">Tailwind is awesome</p>
    <p class="text-red-900">Tailwind is awesome</p>

    <!-- Background Colors -->
    <div class="bg-slate-600">
      <p class="text-white">Tailwind is awesome</p>
    </div>
    <div class="bg-zinc-400">
      <p class="text-white">Tailwind is awesome</p>
    </div>
    <div class="bg-emerald-600">
      <p class="text-white">Tailwind is awesome</p>
    </div>

    <!-- Text Underline -->
    <p class="underline text-red-700 decoration-red-700">Tailwind is awesome</p>
    <p class="underline text-blue-700 decoration-blue-700">
      Tailwind is awesome
    </p>

    <!-- Border Colors -->
    <input class="border-2 border-rose-500" />
    <input class="border-2 border-blue-300" />
    <input class="border-2 border-purple-900" />
    <input class="border-2 border-yellow-500" />

    <!-- Divide Colors -->
    <div class="divide-y divide-blue-200">
      <div>Item 1</div>
      <div>Item 2</div>
      <div>Item 4</div>
      <div>Item 5</div>
      <div>Item 6</div>
    </div>

    <!-- Outline Colors -->
    <button class="outline outline-blue-500">Subscribe</button>
    <button class="outline outline-purple-300">Subscribe</button>
    <button class="outline outline-gray-500">Subscribe</button>

    <!-- Box Shadow Colors (Opacity defaults to 100, but you cans set it)-->
    <button class="bg-cyan-500 shadow-lg shadow-cyan-500">Subscribe</button>
    <button class="bg-blue-500 shadow-lg shadow-blue-500/50">Subscribe</button>
    <button class="bg-indigo-500 shadow-lg shadow-indigo-500/50">
      Subscribe
    </button>

    <!-- Accent Colors -->
    <input type="checkbox" class="accent-purple-500" checked /> Option 1
    <input type="checkbox" class="accent-pink-500" checked /> Option 2
    <input type="checkbox" class="accent-red-300" checked /> Option 3

    <!-- Arbitrary Colors -->
    <div class="bg-[#427fab] h-10">Hello</div>
    <div class="text-[#427fab] h-10">Hello</div>
    <div class="border border-[#427fab] h-10">Hello</div>
```
## 2.2 边距
### 2.2.1 container
```css
container	None	width: 100%;
sm (640px)	    max-width: 640px;
md (768px)	    max-width: 768px;
lg (1024px)	    max-width: 1024px;
xl (1280px)	    max-width: 1280px;
2xl (1536px)	  max-width: 1536px; 
```
### 2.2.2 margin
```html
    <div class="bg-slate-100 m-2">Hello Tailwind</div>
    <div class="bg-slate-100 mx-10">Hello Tailwind</div>
    <div class="bg-slate-100 my-10">Hello Tailwind</div>
    <div class="bg-slate-100 ml-4">Hello Tailwind</div>
    <div class="bg-slate-100 mt-4">Hello Tailwind</div>
    <div class="bg-slate-100 mr-4">Hello Tailwind</div>
    <div class="bg-slate-100 mb-4">Hello Tailwind</div>
    <div class="bg-slate-100 mt-[20px]">Hello Tailwind</div>
```

- 数值  m-1 margin: 0.25rem; /* 4px */ 默认值，可以修改 1rem = 16px
### 2.2.3 padding
```html
  <div class="bg-slate-100 p-2">Hello Tailwind</div>
  <div class="bg-slate-100 px-10">Hello Tailwind</div>
  <div class="bg-slate-100 py-10">Hello Tailwind</div>
  <div class="bg-slate-100 pl-4">Hello Tailwind</div>
  <div class="bg-slate-100 pt-4">Hello Tailwind</div>
  <div class="bg-slate-100 pr-4">Hello Tailwind</div>
  <div class="bg-slate-100 pb-4">Hello Tailwind</div>
  <div class="bg-slate-100 pt-[20px]">Hello Tailwind</div>
```
### 2.2.4 space
```html
    <!-- Space Between X -->
    <div class="flex mt-10 space-x-24">
      <div>item 1</div>
      <div>item 2</div>
      <div>item 3</div>
      <div>item 4</div>
      <div>item 5</div>
      <div>item 6</div>
      <div>item 7</div>
    </div>
    <!-- Space Between Y -->
    <div class="flex flex-col mt-10 space-y-4">
      <div>item 1</div>
      <div>item 2</div>
      <div>item 3</div>
      <div>item 4</div>
      <div>item 5</div>
      <div>item 6</div>
      <div>item 7</div>
    </div>
```

![1.png](https://cdn.nlark.com/yuque/0/2023/png/27367619/1690505217478-d0c86e71-f1a1-48a1-b473-d1b5d162bfe9.png#averageHue=%23fdfdfd&clientId=u1ec9c3c7-aef5-4&from=ui&id=uab75c5b2&originHeight=387&originWidth=1186&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=10278&status=done&style=none&taskId=ue5566f65-5289-4a79-b454-478f3333dd6&title=)
## 2.3 排版
**Font Family**
[https://fonts.google.com/](https://fonts.google.com/)
```html
	<script>
    tailwind.config = {
      theme: {
        fontFamily: {
          sans: ['ui-sans-serif', 'system-ui'],
          serif: ['ui-serif', 'Georgia'],
          mono: ["ui-monospace", "SFMono-Regular"],
          custom: ['Roboto']
        }
      }
    }
  </script>
```

- Font Family 可以使用内置的字体或者自定义的字体
- Font Size 设置文字的大小
- Font Weight 设置文字的粗细
- Letter Spacing 设置文字的间距
- Text Alignment 设置文字左、居中、右
- Text Decoration 用于设置文本的装饰效果，例如下划线、删除线、上划线等
- Decoration Style 设置样式
- Decoration Offset 用于设置文本装饰线与文本本身之间的距离
- Text Transform 用于设置文本的大小写转换方式
## 2.4  尺寸

- 设置元素的宽高 w-8 h-8
-  w-screen 设置视口 w-full设置100%
- 可设置最大最小尺寸
## 2.5 定位
![5.png](https://cdn.nlark.com/yuque/0/2023/png/27367619/1690544894860-fa76640d-6efa-47af-86d2-ed30dbfb3024.png#averageHue=%23fef9f2&clientId=u2cd32e95-eaab-4&from=ui&id=ub0a5893e&originHeight=711&originWidth=1125&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=10344&status=done&style=none&taskId=u6bfd705c-6ff3-4902-9d45-3d6a91cc6dc&title=)

- 子绝父相
- inset-y-0 意思是 top 0 bottom 0
- 浮动元素 left right（用的少）
- display: block;：将元素显示为块级元素，即元素会在页面中独占一行，并且可以设置宽度、高度、内边距和外边距等属性。常用于页面布局中的容器元素，例如 div、p、h1 等。
- display: inline-block;：将元素显示为行内块级元素，即元素会在一行中显示，并且可以设置宽度、高度、内边距和外边距等属性。常用于页面布局中的容器元素，例如 button、input 等。
- display: inline;：将元素显示为行内元素，即元素会在一行中显示，并且不可以设置宽度、高度、内边距和外边距等属性。常用于页面中的文本元素，例如 a、span、em 等。
## 2.6 阴影

![6.png](https://cdn.nlark.com/yuque/0/2023/png/27367619/1690545058764-16af2241-69d1-41b6-af04-d63e090fbdf6.png#averageHue=%23f9f8f8&clientId=u2cd32e95-eaab-4&from=ui&id=u0b20cd68&originHeight=671&originWidth=1350&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=72102&status=done&style=none&taskId=uc976f522-0ace-49b3-b0db-b3f781dcee4&title=)
**颜色渐变**
```html
<!-- Gradients -->
  <div class="h-24 bg-gradient-to-r from-cyan-500 to-blue-500"></div>
  <div class="h-24 bg-gradient-to-r from-indigo-500 via-purple-500 to-pink-500"></div>
```

```html
  <div class="w-96 mt-6 ml-4 p-3 shadow-xl shadow-blue-500/50">
    Lorem, ipsum dolor sit amet consectetur adipisicing elit. Mollitia minus
    deleniti iusto delectus alias natus quam dolor explicabo quas eius!
  </div>
```

- 在Tailwind CSS中，可以使用 shadow 类名来设置元素的阴影效果
- shadow 类名可以与以下的修饰符一起使用，以便更好地控制阴影的大小和颜色
## 2.7 边框

![7.png](https://cdn.nlark.com/yuque/0/2023/png/27367619/1690545212664-a3f1bdf8-89b8-4d59-b230-906357a9aa29.png#averageHue=%23f8f7f7&clientId=u2cd32e95-eaab-4&from=ui&id=u9f1124d0&originHeight=538&originWidth=923&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=28799&status=done&style=none&taskId=u51cff4fb-2ad3-4f33-a1c7-09210b58ba4&title=)

- 边框可以设置大小、颜色、方位、边角、边框偏移量
## 2.8 滤镜（filter）

![8.png](https://cdn.nlark.com/yuque/0/2023/png/27367619/1690545362809-a74e5cb8-583a-441d-bc47-f25a3c5d5de0.png#averageHue=%23f6f6f6&clientId=u2cd32e95-eaab-4&from=ui&id=ube3337c7&originHeight=700&originWidth=1382&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=149698&status=done&style=none&taskId=u40b3bd0b-93e8-4e47-beb2-2a846c69283&title=)

CSS中，可以使用 filter 属性来为元素添加滤镜效果。常用的滤镜属性包括：

- blur()：用于为元素添加高斯模糊效果，其中括号中的值表示模糊半径，取值范围为0到正无穷大。
- brightness()：用于为元素添加亮度效果，其中括号中的值表示亮度值，取值范围为0到正无穷大。
- contrast()：用于为元素添加对比度效果，其中括号中的值表示对比度值，取值范围为0到正无穷大。
- grayscale()：用于为元素添加灰度效果，其中括号中的值表示灰度值，取值范围为0到1。
- hue-rotate()：用于为元素添加色相旋转效果，其中括号中的值表示旋转角度，取值范围为0到360度。
- invert()：用于为元素添加反转颜色效果，其中括号中的值表示反转颜色的程度，取值范围为0到1。
- opacity()：用于为元素添加透明度效果，其中括号中的值表示透明度值，取值范围为0到1。
- saturate()：用于为元素添加饱和度效果，其中括号中的值表示饱和度值，取值范围为0到正无穷大。
- sepia()：用于为元素添加褐色效果，其中括号中的值表示褐色值，取值范围为0到1。

需要注意的是，滤镜属性可以组合使用，以便实现更加复杂的效果。
# 三、基础教程 下
## 3.1 伪类元素

![9.png](https://cdn.nlark.com/yuque/0/2023/png/27367619/1690545539648-3d28c4b8-fc3f-404e-9ccb-85974a6b1d2a.png#averageHue=%23e0f1f1&clientId=u2cd32e95-eaab-4&from=ui&id=u9b6020dc&originHeight=735&originWidth=1712&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=47376&status=done&style=none&taskId=u13297076-7460-47f6-ac03-cc42b589402&title=)

- 在Tailwind CSS中，可以使用伪类元素来为元素添加特殊的样式。常用的伪类元素包括 :hover、:focus、:active 等
- 父子元素可以通过group属性自动向下触发
- appearance-none重置默认元素样式
- resize是CSS中的一个属性，用于控制元素是否可以被用户调整大小
- Smooth Scroll 平滑过渡属性
## 3.2 媒体查询
```html
    sm	640px	  @media (min-width: 640px) { ... }
    md	768px	  @media (min-width: 768px) { ... }
    lg	1024px	@media (min-width: 1024px) { ... }
    xl	1280px	@media (min-width: 1280px) { ... }
    2xl	1536px	@media (min-width: 1536px) { ... }
```

- 在CSS中，可以使用媒体查询（Media Queries）来根据设备的特性（如屏幕宽度、高度、分辨率等）来为不同的设备设置不同的样式
- tailwind 使用更加方便的md:类名方式进行适配
## 3.3 Columns

![10.png](https://cdn.nlark.com/yuque/0/2023/png/27367619/1690545753793-390db89b-5e6f-4df8-8ffd-926cadea9c97.png#averageHue=%23566155&clientId=u2cd32e95-eaab-4&from=ui&id=ub31cc13f&originHeight=653&originWidth=1838&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=800357&status=done&style=none&taskId=uc3bfa23f-992c-4a35-80a9-f1e84280b09&title=)

columns 是一个用于创建网格布局的类名。columns 类名可以与数字（1到12）组合使用，以便更好地控制网格的列数。
## 3.4 flex布局
![11.png](https://cdn.nlark.com/yuque/0/2023/png/27367619/1690545854297-a7b701ae-937f-4514-8a15-f6dd0dc1d2f1.png#averageHue=%23dfe4eb&clientId=u2cd32e95-eaab-4&from=ui&id=uca4a9fc8&originHeight=821&originWidth=1669&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=22779&status=done&style=none&taskId=u0b01f132-2d63-42ca-b6bc-c9a28d1068e&title=)

- 和css 使用的布局差不多，可以设置列、行。使用order可以二次设置元素的方向

[Flex 布局语法教程 | 菜鸟教程](https://www.runoob.com/w3cnote/flex-grammar.html)

- flex-none：将元素的flex属性设置为 none，表示该元素不会随着容器的大小而改变大小，即不会发生伸缩。
- flex-initial：将元素的flex属性设置为 0 1 auto，表示该元素可以缩小但不能放大，同时会考虑元素的初始大小。
- flex-auto：将元素的flex属性设置为 1 1 auto，表示该元素可以根据容器的大小自动伸缩，同时会考虑元素的初始大小。
- flex-1：将元素的flex属性设置为 1 1 0%，表示该元素可以根据容器的大小自动伸缩，同时会忽略元素的初始大小。
## 3.5 grid布局
![12.png](https://cdn.nlark.com/yuque/0/2023/png/27367619/1690545992659-bd511332-1b52-4fb1-96ad-5b1361a6b6ab.png#averageHue=%23d7e6fa&clientId=u2cd32e95-eaab-4&from=ui&id=u072069c3&originHeight=808&originWidth=1916&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=13990&status=done&style=none&taskId=ue2f9bb1d-e8ea-4338-b86e-bbb1af3be77&title=)

```html
<div class="grid grid-cols-1 md:grid-cols-3 gap-4 bg-gray-300 ">
    <div class="p-10 border border-blue-600 bg-blue-100 md:row-span-2 md:col-span-2">item 1</div>
    <div class="p-10 border border-blue-600 bg-blue-100">item 2</div>
    <div class="p-10 border border-blue-600 bg-blue-100">item 3</div>
    <div class="p-10 border border-blue-600 bg-blue-100">item 4</div>
    <div class="p-10 border border-blue-600 bg-blue-100">item 5</div>
    <div class="p-10 border border-blue-600 bg-blue-100">item 6</div>
    <div class="p-10 border border-blue-600 bg-blue-100 md:row-span-2  md:col-span-2">item 7</div>
    <div class="p-10 border border-blue-600 bg-blue-100">item 8</div>
    <div class="p-10 border border-blue-600 bg-blue-100">item 9</div>
    <div class="p-10 border border-blue-600 bg-blue-100 md:col-span-3">item 10</div>
  </div>
```

- grid-col 设置全局列，grid-row设置全局行
- col-span 设置当前元素可以占几个，row-span同理
## 3.6 动画

![13.png](https://cdn.nlark.com/yuque/0/2023/png/27367619/1690630255192-e8600abd-6974-4c34-a6fb-545fc57da42a.png#averageHue=%23e4e4e4&clientId=ufe867cdb-3c5d-4&from=ui&id=ud7714117&originHeight=757&originWidth=1015&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=74701&status=done&style=none&taskId=ub46bb80e-0cc1-4f88-91de-bb4bc18187d&title=)
```html
//自定义数值
<script>
    tailwind.config = {
      theme: {
        extend: {
          transitionDuration: {
            0: '0ms',
            5000: '5000ms',
          },
        },
      },
    }
  </script>
```

Tailwind CSS 的 transition 类是用于设置 CSS 过渡效果的类。它可以让元素在状态改变时平滑地过渡到新状态，而不是突然地改变。
transition 类可以用于设置以下 CSS 属性的过渡效果：

- opacity：元素的不透明度
- background-color：元素的背景颜色
- border-color：元素的边框颜色
- box-shadow：元素的阴影效果
- transform：元素的变换效果，如旋转、缩放、位移等

transition 类可以与其他 Tailwind CSS 类组合使用，以设置过渡效果的持续时间、速度曲线、延迟等。例如，可以使用 duration-500 类设置过渡效果的持续时间为 500 毫秒，使用 ease-in-out 类设置速度曲线为缓进缓出，使用 delay-100 类设置延迟 100 毫秒后再开始过渡效果。
## 3.7 关键帧
![14.png](https://cdn.nlark.com/yuque/0/2023/png/27367619/1690630471248-a7ac2188-b3d9-4bde-8765-d60faad677fb.png#averageHue=%23131b2e&clientId=ufe867cdb-3c5d-4&from=ui&id=u4e0689fc&originHeight=527&originWidth=908&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=14919&status=done&style=none&taskId=ucaf94ab2-8796-4227-bcb6-88a84c7bfec&title=)

```html
<script>
    tailwind.config = {
      theme: {
        extend: {
          animation: {
            'spin-slow': 'spin 3s linear infinite',
            'wiggle': 'wiggle 1s ease-in-out infinite',
          },
          keyframes: {
            wiggle: {
              '0%, 100%': { transform: 'rotate(-12deg)' },
              '50%': { transform: 'rotate(12deg)' },
            },
          }
        }
      }
    }
  </script>
```

- Tailwind CSS 的 animate 类是用于设置 CSS 动画效果的类。它可以让元素在状态改变时以动画的形式过渡到新状态，从而增强页面的交互性和视觉效果。
- 内置了多种效果，可以定制或者修改已有的效果
## 3.8 本地化
```html
  <script>
    tailwind.config = {
      theme: {
        screens: {
          'sm': '600px',
          'md': '800px',
          'lg': '1024px',
          'xl': '1280px',
          '2xl': '1536px',
        },
        extend: {
          colors: {
            'purple': '#3f3cbb',
            'midnight': '#121063',
            'metal': '#565584',
          },
          spacing: {
            '6': '2rem',
          },
          borderRadius: {
            '4xl': '2rem',
          },
        }
      }
    }
  </script>
```
## 3.9 主题切换

![16.png](https://cdn.nlark.com/yuque/0/2023/png/27367619/1690630703451-c428aa04-baa0-4b3f-bf65-d072cc72db0c.png#averageHue=%23f6edde&clientId=ufe867cdb-3c5d-4&from=ui&id=u2dfb23ac&originHeight=433&originWidth=1311&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=18046&status=done&style=none&taskId=u8984d207-84ea-4993-b287-89c29e0165f&title=)
![15.png](https://cdn.nlark.com/yuque/0/2023/png/27367619/1690630689108-a47435e2-c1ae-4caa-96e1-286cb63f8990.png#averageHue=%23ceb89a&clientId=ufe867cdb-3c5d-4&from=ui&id=u7bc0db3a&originHeight=356&originWidth=1359&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=17746&status=done&style=none&taskId=u4109f3a4-2f82-409e-8316-3ca4b8e0efa&title=)

- Tailwind CSS 的 dark 模式是一种用于在网站或应用程序中切换明暗两种主题的功能。它可以让用户根据自己的喜好或环境光线的亮度来选择合适的主题，从而提高用户体验和可用性。
- 需要注意的是，为了实现 dark 模式，需要在 HTML 的 body 元素上添加 class="dark" 属性。
# 四、开发环境设置
## 4.1 基本步骤

![17.png](https://cdn.nlark.com/yuque/0/2023/png/27367619/1690630912176-21870e2b-fed5-4e9c-b6fc-9b2583a12225.png#averageHue=%2322262d&clientId=ufe867cdb-3c5d-4&from=ui&id=uedf67bb9&originHeight=370&originWidth=496&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=23010&status=done&style=none&taskId=u83c44ed0-0e99-4967-bd2f-bcff34b09b0&title=)

[Installation - Tailwind CSS](https://tailwindcss.com/docs/installation)

使用Tailwind CLI tool工具开发
## 4.2 修改配置
```json
{
  "name": "tailwind-starter",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "watch": "tailwindcss -i ./src/input.css -o ./css/style.css --watch",
    "build": "tailwindcss -i ./src/input.css -o ./css/style.css"
  },
  "keywords": [],
  "author": "",
  "license": "ISC",
  "devDependencies": {
    "tailwindcss": "^3.3.3"
  }
}
```

- watch一直监控input.css变化，重构生成到style.css
- build开发完成最后打包
## 4.3 样式定制化
```css
@tailwind base;
@tailwind components;
@tailwind utilities;

@layer base{
  h1 {
    font-size: 3rem;
  }

  h2 {
    @apply text-2xl text-sky-500 font-bold mt-10;
  }

}

@layer components{
  .btn-blue {
    @apply bg-blue-500 text-white font-bold py-2 px-4 rounded m-10;
  }
}


.text-area{
  @apply bg-gray-200 border-2 border-gray-400 rounded-lg p-4;
  height: theme('spacing.128');
}
```
五、小项目


六、大项目
