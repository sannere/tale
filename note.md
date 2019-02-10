#Tale学习笔记
##•	div
1)	自带格式：换行
2)	可以用id和class标记div，id是唯一的，class是标记这个div的类型的。例如：所有的新闻div，class都可以为news，这样可以识别出一个类型的div。id和class都是可选的。
##•	${}
1)	不指定查找范围，所以它会依序从Page、Request、Session、Application范围查找。如果途中找到了变量，就直接传回来。如果所有都找不到，就返回null。
##  $
1)  除了数据属性，Vue 实例还暴露了一些有用的实例属性与方法。它们都有前缀 $，以便与用户定义的属性区分开来。
##•	Style标签border属性 
1)	三个参数，分别为粗细，形状，颜色
2)	形状有四种：dotted solid double dashed
##•	v-cloak
1)	使用vue框架时，页面加载会闪烁变量名，加入v-cloak指令，会解决这个问题
2)	不需要在所有的标签上都加，只有挂载了标签添加就可以

 

2019/1/18
##•	col-lg-12
1)	是bootstrap的一个属性。Bootstrap是一个前端开发框架。这个属性是用于栅格系统的。
2)	Col-lg/md/sm/col-lg/md/sm/xs，指的是显示屏幕的大小。随着屏幕设备或视口（viewport）尺寸的增加，系统会自动分为最多12列，后面的数字指的是有几个栅格。如果是col-lg-2，就是说一行里可以显示6个标签，如果是col-md-4，就是说一行显示3个标签
##•	嵌套模板语句 #include（jetbrick模板）
1)	语法：#include(file, [parameters], [returnName])
2)	子模板可以共享父模板的context，父模板可以传私有变量“parameters”给子模板。
##•	Jetbrick模板
1)	模板中不同于java的指令，前面会有#
2019年1月25日星期五
##•	Input
1)	Input表示Form表单中的一种输入对象，其又随Type类型的不同而分文本输入框，密码输入框，单选/复选框，提交/重置按钮等.
2)	Text 属性代表 HTML 表单中的单行输入字段。
3)	Hidden 属性，代表一个 HTML 表单中的某个隐藏输入域。这个不可见的表单元素的 value 属性保存了一个要提交给 Web 服务器的任意字符串。如果想要提交并非用户直接输入的数据的话，就是用这种类型的元素。隐藏字段通常会存储一个默认值，它们的值也可以由 JavaScript 进行修改。
4)	placeholder 属性，可描述输入字段预期值的提示信息（hint）。该提示会在输入字段为空时显示，并会在字段获得焦点时消失。适用于以下的 <input> 类型：text, search, url, telephone, email 以及 password。
##•	Margin
1)	margin 简写属性在一个声明中设置所有外边距属性。该属性可以有 1 到 4 个值。
2)	块级元素的垂直相邻外边距会合并，而行内元素实际上不占上下外边距。行内元素的的左右外边距不会合并。同样地，浮动元素的外边距也不会合并。
3)	元素周围生成额外的空白区。“空白区”通常是指其他元素不能出现且父元素背景可见的区域。
##•	Padding
1)	这个简写属性设置元素所有内边距的宽度，或者设置各边上内边距的宽度。
2)	行内非替换元素上设置的内边距不会影响行高计算；因此，如果一个元素既有内边距又有背景，从视觉上看可能会延伸到其他行，有可能还会与其他内容重叠。
3)	补白位于元素框的边界与内容区之间。
##•	Margin vs padding
1)	margin是用来隔开元素与元素的间距；padding是用来隔开元素与内容的间隔。margin用于布局分开元素使元素与元素互不相干；padding用于元素与内容之间的间隔，让内容（文字）与（包裹）元素之间有一段“呼吸距离”。
2)	http://www.hicss.net/use-margin-or-padding/

##•	V-model
1)	在表单控件或者组件上创建双向绑定。
2)	v-model 会忽略所有表单元素的 value、checked、selected 特性的初始值而总是将 Vue 实例的数据作为数据来源。你应该通过 JavaScript 在组件的 data 选项中声明初始值。
3)	
##•	Label
1)	<label> 标签为 input 元素定义标注（标记）。
2)	label 元素不会向用户呈现任何特殊效果。不过，它为鼠标用户改进了可用性。如果您在 label 元素内点击文本，就会触发此控件。就是说，当用户选择该标签时，浏览器就会自动将焦点转到和标签相关的表单控件上。
3)	"for" 属性可把 label 绑定到另外一个元素。请把 "for" 属性的值设置为相关元素的 id 属性的值。


2019年1月27日星期日
##•	Callback
1)	起始函数 中间函数 回调函数：起始函数会给中间函数传一个函数（作为参数），好在合适的时候调用，以完成目标任务。这个被传入的、后又被调用的函数就称为回调函数（callback function）。给中间函数传入什么样的回调函数，是在起始函数里决定的。
2)	在回调中，我们利用某种方式，把回调函数像参数一样传入中间函数。在传入一个回调函数之前，中间函数是不完整的。换句话说，程序可以在运行时，通过登记不同的回调函数，来决定、改变中间函数的行为。这样可以增加程序的灵活性。
3)	示例：![Alt text](/Users/liufanghua/Desktop/git/tale/callback1.png)

         ![Alt text](/Users/liufanghua/Desktop/git/tale/callback2.png)
4)	阻塞式回调和延迟式回调。阻塞式回调里，回调函数的调用一定发生在起始函数返回之前；而延迟式回调里，回调函数的调用有可能是在起始函数返回之后。(https://juejin.im/entry/5aeec4a4518825672033f5d4)
5)	回调函数常规写法：callback && callback();即如果callback有定义，则执行。

##•	时间戳
1)	是一种时间表示方式，定义为从格林威治时间1970年01月01日00时00分00秒起至现在的总秒数。严格来说，不管你处在地球上的哪个地方，任意时间点的时间戳都是相同的。这点有利于线上和客户端分布式应用统一追踪时间信息。

2019年1月29日星期二
##• DOM
1)  文档对象模型（Document Object Model，简称DOM），是W3C组织推荐的处理可扩展标志语言的标准编程接口。
2)  DOM 可被 JavaScript 用来读取、改变 HTML、XHTML 以及 XML 文档。
3)  DOM 连接了js和html。js不能直接改变html的element，通过document.XXX()方法，可以改变DOM，然后DOM会变更html元素。

##  span
1)  <span> 用于对文档中的行内元素进行组合。
2)  div就像一个段落，在视觉上于页面隔离出了文档的一部分，它可以包含段落、标题、表格等。span元素的作用是选择特定文本，以便于指定特殊样式。
3)  div占用一行，span不会占用一行，内容占多大宽度，span就有多宽。
4)  span嵌套在<div>或者<p>里，可以用于更改一行中的一部分text格式，比如着重，加粗。

## vue基本语法
1)  {{}}：用双大括号的普通文本插入。eg:<span>Message: {{ msg }}</span>。双大括号会被替代为对应数据对象上msg属性的值。无论何时，绑定的数据对象上msg属性发生了改变，插值处的内容都会更新。
2)  原始HTML：双大括号会将数据解释为普通文本，而非 HTML 代码。为了输出真正的 HTML，你需要使用 v-html 指令。
3)  指令：指令 (Directives) 是带有 v- 前缀的特殊特性。
4)  v-bind: 可以在html属性中绑定数据，{{}}不能用于HTML特性上。
    缩写：<!--完整语法--> 
         <a v-bind:href="url">..</a>
         <!--缩写-->
         <a :href="url">..</a>  
5)  v-if
6)  v-for：我们用 v-for 指令根据一组数组的选项列表进行渲染。v-for 指令需要使用 item in items 形式的特殊语法，items 是源数据数组并且 item 是数组元素迭代的别名。
    
7)  v-on：添加一个事件监听器，用于监听DOM事件，调用在Vue实例中定义的**方法**
    缩写：<!--完整语法--> 
         <a v-on:click="doSomething">..</a>
         <!--缩写-->
         <a :@click="doSomething">..</a>  
8)  v-model
9)  v-once:一次性的插值，当数据改变时，插值处的内容不会更新.


## 计算属性缓存 VS 方法
1)  计算属性缓存：在computed中声名，当它该属性的依赖发生改变时，它才会重新求值，多次访问计算属性时，如果依赖没有改变，就会立刻返回之前的计算结果，而不必再次执行函数。
2)  调用方法：在methods中声名，每次访问都会再次执行函数。

## watch
1)  当有一些数据需要随着其他数据变动而变动时，需要在数据变化时执行异步，可以使用watch，而也可以使用计算属性。计算属性更简洁。

## AJAX
1)  全称是Asynchronous JavaScript and XML 中文名称定义为异步的JavaScript和XML。由多种技术集合而成，使用Ajax技术不必刷新整个页面，只需对页面的局部进行更新，可以节省网络带宽，提高页面的加载速度，从而缩短用户等待时间，改善用户体验。

## 折行转义字符
1)  https://css-tricks.com/snippets/javascript/multiline-string-variables-in-javascript/

## 模板字符串
1)  `` -> 让多行的模板更易读。
2)  https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/template_strings#%E8%AF%AD%E6%B3%95

## #符号
1)  如果值以#开始，则它将被用作选择符，并使用匹配元素的innerHTML作为模板。

## clearfix
1)  The clearfix allows a container to wrap it's floated children. Without a clearfix or equivalent styling, a container does not wrap around its floated children and collapses, just as if its floated chldren were positioned absolutely.
2)  biezhi大牛引用答案：https://stackoverflow.com/questions/8554043/what-is-a-clearfix，answered by John Slegers
3)  说白了，就是为了兼容老版本的ie浏览器的。

2019年2月7日星期四
## class
1)  html元素中class属性值多个空格:就是指定多个class的意思，在HTML的层面上说的话，这样指定的class是同级的。同级的class需要看CSS文件的先后次序，后加载的css会覆盖前面加载的css。
2)  在 HTML 中, 类名是区分大小写的。

## v-show
1)  根据条件展示元素。
2)  不同的是带有 v-show 的元素始终会被渲染并保留在 DOM 中。v-show 只是简单地切换元素的 CSS 属性 display。如过元素的display为none，就不会被显示出来在

## <a>
1)  <a> 标签的 href 属性用于指定超链接目标的 URL。
2)  href 属性的值可以是任何**有效文档的相对或绝对 URL**，包括片段标识符和 JavaScript 代码段。如果用户选择了 <a> 标签中的内容，那么浏览器会尝试检索并显示 href 属性指定的 URL 所表示的文档，或者执行 JavaScript 表达式、方法和函数的列表。
3)  <a> 标签中必须提供 href 属性或 name 属性。

2019年2月8日星期五

## 模板引擎
1)  模板引擎是为了组件化工作的, 是为了减少重复编写某些代码而出现的.实际上模板引擎是为了实现模板文件与业务数据的结合, 实现界面与数据的分离.
2)  为了生成一个html文件，中间有很多重复的代码，我们可以做一个模板（逻辑部分），然后用模板引擎往里面装数据，这样可以生成一个html文件。
3)  逻辑的部分在js文件中，模板是html文件，中间有的变量需要模板引擎去置换掉。

## HTML中引入js
1)  利用<script type="text/javascript" src="js文件的路径"></script> 引入一个外部的js文件。
2)  使用<script>标签：<script>直接在这添加js代码</script>
3)  直接在HTML标签中插入js代码:<input name="btn" type="button" value="弹出消息框" onclick="javascript:alert('欢迎你');"/>

## aria
1)  Accessible Rich Internet Applications，规定了能够让 Web 内容和 Web 应用（特别是那些由 Ajax 和 JavaScript 开发的）对于残障人士更易使用的各种机制。
2)  aria-hidden="true":图标的可访问性,为了避免 屏幕识读设备抓取非故意的和可能产生混淆的输出内容（尤其是当图标纯粹作为装饰用途时），我们为这些图标设置了 aria-hidden="true" 属性。播放到带此属性的内容时会自动跳过，以免残障人士混淆。

## $.extend(){}
1)  合并对象：函数用于将一个或多个对象的内容合并到目标对象。eg:$.extend( target [, object1 ] [, objectN ] )
2)  方法扩展：如果target缺失那么，功能是：把对象挂载到 jQuery 的 prototype 上以扩展一个新的 jQuery 实例方法/类方法。

## $()
1)  他是document.getElementById() 方法的一个便利的简写，就像这个DOM方法一样，这个方法返回参数传入的id的那个元素。你可以传入多个id作为参数然后 $() 返回一个带有所有要求的元素的一个 Array 对象。
2)  $("id")意思是在DOM中找到并返回id为"id"的元素，通过ID获取Element。

## dropzone.js
1)  是一个开源的 JavaScript 库，提供 AJAX 异步上传功能。
2)  因为我们需要使用dropzone提供的一些样式，比如预览时图片样式等，这样就算手动创建，但也需要使用到dropzone样式类，那这样就会导致初始化两次，在控制台就会报错，这时候就需要在手动初始化之前设置如下代码：Dropzone.autoDiscover = false;

## this.$loading.show()
1)  他是biezhi引用的一个组件：Vue Loading Overlay Component：Vue.js component for full screen loading indicator
2)  ![Alt text](/Users/liufanghua/Desktop/git/tale/vue-loading.jpg)

## el: '#app'(vue)
1)  el属性：把当前Vue对象挂载到 div标签上，#app是id选择器。
2)  在实例挂载之后，元素可以用 vm.$el 访问。



