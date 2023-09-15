# JS 基础
## 一、JS简介
### 1、定义
![](./images/QQ截图20230824180333.png)  

### 2、组成
![](./images/QQ截图20230824180618.png)  
`https://developer.mozilla.org/zh-CN/`

### 3、书写位置
#### (1)行内JavaScript  
![](./images/QQ截图20230824201942.png)
#### (2)外部
![](./images/QQ截图20230824202252.png)
#### (3)内联
![](./images/QQ截图20230824204550.png)

### 4、注释
![](./images/QQ截图20230824204729.png)

### 5、结束符
![](./images/QQ截图20230824204951.png)

### 6、输入和输出语法
#### (1)输出语法
![](./images/QQ截图20230824210749.png)
```
// 显示在网页中
document.write('i am h1')
// 以标题格式显示在网页中
document.write('<h1>i am h1</h1>')
// 显示在弹框中
alert('help')
// 显示在控制台中
console.log('console print')
```
#### (2)输入语法
##### promp
![](./images/QQ截图20230825151754.png)
`prompt('input your name')`
##### confirm
`if (confirm('你确定要执行此次操作么?'))`，confirm会跳出弹框，根据用户的选择返回true or false  

### 7、代码执行循序
按照HTML文档流执行JS代码  
alert()和prompt()会跳过页面渲染而先被执行

### 8、字面量
![](./images/QQ截图20230825152232.png)

## 二、变量
### 1、定义
![](./images/QQ截图20230825152610.png)

### 2、基本使用
#### (1)变量的声明
![](./images/QQ截图20230825152803.png)
#### (2)变量的赋值
![](./images/QQ截图20230825153150.png)
#### (3)更新变量
let不允许多次申明一个变量
#### (4)声明多个变量
`let age = 18, name = 'kang'`
`console.log(age, name)`
![](./images/QQ截图20230825160052.png)

### 3、本质
![](./images/QQ截图20230825192732.png)

### 4、命名规则与规范
![](./images/QQ截图20230825193035.png)

### 5、let和var的区别
![](./images/QQ截图20230825193447.png)

### 6、数组
#### (1)声明
![](./images/QQ截图20230825193934.png)
#### (2)一些术语
![](./images/QQ截图20230825194159.png)

## 三、常量
![](./images/QQ截图20230825194848.png)

## 四、数据类型
js弱数据类型语言,只有赋值以后，才能确认 
### 1、数字类型
![](./images/QQ截图20230827144310.png)  
NAN not a number  
![](./images/QQ截图20230827144801.png)  

### 2、字符串类型string
#### (1)定义
![](./images/QQ截图20230827145257.png)
#### (2)字符串拼接
可使用加号进行字符串拼接 
```
let age = 20
document.write('I am ' + age +' years old')
``` 
#### (3)模板字符串
![](./images/QQ截图20230827150013.png)

#### (4)trim()方法
字符串的trim方法可以去除字符串左右两侧的空格，字符串中间的空格被保存  
```
const str = '     pink   '
console.log(str.trim())       //输出pink，两侧的空格被去除
```

### 3、布尔类型boolen
![](./images/QQ截图20230827150618.png)

### 4、未定义类型undefined
![](./images/QQ截图20230827150745.png)

### 5、null空类型
![](./images/QQ截图20230827150912.png)  
null与undefined的区别  
![](./images/QQ截图20230827150912.png)

### 6、检测数据类型typeof
![](./images/QQ截图20230827151418.png)

## 五、类型转换
### 1、定义
![](./images/QQ截图20230827155119.png)
### 2、隐式转换
![](./images/QQ截图20230827155417.png)  
`console.log(+'12')    //输出数字类型12`  
`let num = +prompt("input your age")    //num此时转变为数字型`
### 3、显式转换
![](./images/QQ截图20230827160404.png)  
parseInt和parseFloat只能截取字符串前段数字，如果字符串以字母开头，则会返回NaN
```
let a = prompt("first one")
let b = prompt("second one")
alert(Number(a)+Number(b))

let a = +prompt("first one")
let b = +prompt("second one")
alert(a+b)
```

## 六、运算符
### 1、赋值运算符
![](./images/QQ截图20230827172910.png)

### 2、一元运算符
自增运算符：i++和++i,与cpp相同

### 3、比较运算符
![](./images/QQ截图20230827191551.png)
`console.log(2=='2');    //true，比较运算符存在隐式转换，把'2'转换为2 `  
判断是否相等用===  
![](./images/QQ截图20230827192546.png )
  
### 4、逻辑运算符
![](./images/QQ截图20230827193013.png)

### 5、运算符优先级
![](./images/QQ截图20230827193825.png)

## 七、分支语句
语句和表达式的区别
![](./images/QQ截图20230827194516.png)
### 1、if语句
![](./images/QQ截图20230827194851.png)  
![](./images/QQ截图20230827195028.png)   
![](./images/QQ截图20230827195503.png)

### 2、三元运算符
![](./images/QQ截图20230827200055.png)

### 3、switch语句
![](./images/QQ截图20230827210823.png)

### 4、断点调试
![](./images/QQ截图20230827211608.png)

## 八、循环语句
### 1、while循环
#### (1)基本语法
![](./images/QQ截图20230827211741.png)
#### (2)循环三要素
![](./images/QQ截图20230827212049.png)
#### (3)循环推出
![](./images/QQ截图20230827214336.png)

### 2、for循环
#### (1)for循环的基本使用
![](./images/QQ截图20230829151011.png)
#### (2)循环嵌套
![](./images/QQ截图20230829151736.png)

## 九、数组
### 1、基本使用
![](./images/QQ截图20230829160656.png)
### 2、遍历数组
![](./images/QQ截图20230829160809.png)
### 3、数组操作
![](./images/QQ截图20230829161501.png)
#### (1)增
![](./images/QQ截图20230829162550.png)  
![](./images/QQ截图20230829162917.png)
#### (2)删
##### pop
![](./images/QQ截图20230829163126.png)
##### shift
![](./images/QQ截图20230829163419.png)
##### splice
![](./images/QQ截图20230829163620.png)

## 十、函数
![](./images/QQ截图20230829164838.png)

### 1、函数使用
#### (1)函数声明
![](./images/QQ截图20230829165059.png)
#### (2)命名规范
![](./images/QQ截图20230829165126.png)
#### (3)函数使用
![](./images/QQ截图20230829165237.png)

### 2、函数传参
![](./images/QQ截图20230829170608.png)  
![](./images/QQ截图20230829170801.png)
#### 默认参数
![](./images/QQ截图20230829171159.png)

### 3、函数返回值
***如何返回多个数据：数组***  
![](./images/QQ截图20230829172309.png)  
![](./images/QQ截图20230829172411.png) 

### 4、细节补充
![](./images/QQ截图20230829173916.png)   

### 5、作用域
#### (1)全局作用域和局部作用域
![](./images/QQ截图20230829174208.png)  
#### (2)全局变量和局部变量
```
let num = 10                     //num为全局变量,可在函数内部访问
console.log(num)
function fn(){
  console.log(num)
}
fn()
```
![](./images/QQ截图20230829174313.png)
![](./images/QQ截图20230829174929.png)  
#### (3)变量访问原则
![](./images/QQ截图20230829175159.png)

### 6、匿名函数
匿名函数无法直接使用  
#### (1)函数表达式
```
// 具名函数的调用可以写到任何位置
// 函数表达式，必须先声明函数表达式，后调用
let fn = function(){
  console.log();
}
fn()
```
![](./images/QQ截图20230829180800.png)
#### (2)立即执行函数
无需调用，直接执行,多个立即执行函数直接必须使用分号隔开  
![](./images/QQ截图20230831141625.png)
```
立即执行函数的几种写法
(function(){}());
(function(){})();
!function(){}();
```
![](./images/QQ截图20230831142433.png)

### 7、逻辑中断
![](./images/QQ截图20230831145218.png)
```
//给a的赋值不是true or false，而是a或0，在逻辑运算中，undefined被当做false，而进行右边的运算，给a赋值0，函数是为了防止没有实参而导致报错，可用默认参数代替实现
function fn(a, b) {
  a = a || 0                    
  b = b || 0
  console.log(x + y);
}
```

### 8、bool类型转换
![](./images/QQ截图20230831150208.png)
![](./images/QQ截图20230831150443.png)

## 十一、对象
### 1、定义
![](./images/QQ截图20230831151248.png)

### 2、对象使用-属性
#### (1)声明语法
![](./images/QQ截图20230831151523.png)
#### (2)属性
![](./images/QQ截图20230831155648.png)
#### (3)查
```
// 查的两种方式
对象名.属性民  obj.age
对象名['属性名']  obj['age']
```  
![](./images/QQ截图20230831160158.png)  
![](./images/QQ截图20230831161824.png)
#### (4)改
![](./images/QQ截图20230831160310.png)
#### (5)增
![](./images/QQ截图20230831160424.png)
#### (6)删
![](./images/QQ截图20230831160526.png)

### 3、对象使用-方法
![](./images/QQ截图20230831162505.png)

### 4、遍历对象
![](./images/QQ截图20230831163212.png)
![](./images/QQ截图20230831165025.png)  
只能使用obj[k]这一方法来遍历对象，相当于查操作的第二种方式，因为k的本质上是一个string型变量  
很少使用for-in语法来遍历数组  
```
let arr = [ 'pink','red', 'blue']
for (let k in arr) {
  console.log(k)                // 数组的下标 索引号 但是,此时k是字符串型
  console.log(arr[k])           // arr[k]
}
```
### 5、内置对象
#### (1)定义
JavaScript内部提供的对象，包含各种属性和方法给开发者调用
#### (2)内置对象-Math
![](./images/QQ截图20230831192533.png)
`https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Math#%E5%B1%9E%E6%80%A7`
#### (3)内置对象-生成任意范围随机数
![](./images/QQ截图20230831194846.png)

## 十二、一些扩展
### 1、术语解释
![](./images/QQ截图20230831204237.png)

### 2、基本数据类型/引用数据类型
![](./images/QQ截图20230831204350.png)   
![](./images/QQ截图20230831204642.png)  
```
let num = 10
let num2 = num
num = 20
console.log(num2)                               // 10

let obj1 = {age: 18}
let obj2 = obj1
obj1.age = 20
console.log(obj2)                               // 20
```

### 3、变量声明和const优先
![](./images/QQ截图20230901133803.png)   
![](./images/QQ截图20230901134348.png)  

# WEB APIs
## 一、Web API基本认知
### 1、作用和分类
![](./images/QQ截图20230901134943.png)

### 2、DOM定义
Document Object Model 文档对象模型
![](./images/QQ截图20230901135108.png)

### 3、DOM树
![](./images/QQ截图20230901135459.png)

### 4、DOM对象(重要)
![](./images/QQ截图20230901140007.png)

## 二、获取DOM对象
### 1、根据CSS选择器来获取DOM元素(重点)
#### (1)doucument.querySelector('CSS 选择器')
![](./images/QQ截图20230901140652.png)
#### (2)doucument.querySelectorALL('CSS 选择器')
![](./images/QQ截图20230901140731.png)  
![](./images/QQ截图20230901142152.png)

### 2、其他获取DOM元素方法(了解)
![](./images/QQ截图20230901142459.png)

## 三、操作元素内容
### 1、对象.innerText属性
![](./images/QQ截图20230901150328.png)  
```
const box = document.querySelector('.box')
console.log(box.innerText)                   
box.innerText='<strong>我是一个盒子</strong>'
console.log(box.innerText)         //显示<strong>我是一个盒子</strong>，innerText不解析标签
```
### 2、对象.innerHTML属性
innerHTML与innerText属性基本相同，只是innerText会解析标签  
![](./images/QQ截图20230901153346.png)
```
const box = document.querySelector('.box')
console.log(box.innerTHTML)                   
box.innerText='<strong>我是一个盒子</strong>'
console.log(box.innerText)         //加粗显示'我是一个盒子'，innerHTML解析标签
```

## 四、操作元素属性
### 1、操作元素常用属性
![](./images/QQ截图20230901155437.png)
```
<img src="../JS笔记/images/QQ截图20230824180333.png" alt="">

<script>
  const img = document.querySelector('img')
  img.src='../JS笔记/images/QQ截图20230824180618.png'
  img.title='qq截图'
</script>
```

### 2、操作元素样式属性
![](./images/QQ截图20230901160825.png)
#### (1)通过style属性操作CSS
![](./images/QQ截图20230901162557.png)  
document.body可以直接获得，不需要使用querySelector方法
```
<div class="box"></div>
<script>
  const box = document.querySelector('.box')
  box.style.width = '400px'
  // 多组单词的采取小驼峰命名法，background-color中的-会被解析成减号从而报错
  // box.style.background-color='blue'，会报错
  box.style.backgroundColor='blue'
</script>
```

#### (2)通过操作类名(className)操作CSS
使用className可以同时修改多个样式，但是，直接使用className赋值会覆盖以前的类名  
如果需要保留多个属性，在赋值时需要加上多个类名
![](./images/QQ截图20230901163710.png)  
```
<style>
  div {
    width: 200px;
    height: 200px;
  }

  .one {
    background-color: blue;
  }

  .two {
    border: 2px solid black;
  }
</style>

<body>
  <div>111</div>
  <div class="one two"></div>
  <script>
    const div = document.querySelector('div')
    div.className = 'one'            //div会添加类名，相当于变成<div class="one"></div>
    div.className = 'two'            //会覆盖原来的类名，相当于变成<div class="one"></div>,会覆盖原来所有的类名
    div.className = 'one two'        //标签<div class="one two"></div>
  </script>
</body>
```
#### (3)通过classList操作类控制CSS
`div.classList.add('one')`此时类名不用加点，因为classList追踪的对象只能是类名
![](./images/QQ截图20230901170007.png)  
toggle()切换类，有就删掉，没有就加上  
`box.calssList.toggle('active')`
#### (4)className和classList的区别
![](./images/QQ截图20230901171859.png)  

### 3、操作表单元素属性
表单的值由`表单.value`得到，而非`表单.innerHTML`
![](./images/QQ截图20230904182132.png)  
![](./images/QQ截图20230904182849.png)  
![](./images/QQ截图20230904183452.png)  


```
<button>按钮</button>
<input type="checkbox">

<script>
  const bt = document.querySelector('button')
  bt.disabled = true
  const ipt = document.querySelector('input')
  ipt.checked = true
</script>
```

### 4、自定义属性
`let i = +e.target.dataset.id                     //此时id为字符串，隐式转换`  
`document.querySelector('[data-name="new"]')      //属性选择器，属性名的引号可以省略`  
`document.querySelector('[data-name=new]')        //属性选择器，属性名的引号可以省略`  
![](./images/QQ截图20230904202707.png)

## 五、定时器-间歇函数
### 1、定时器函数介绍
![](./images/QQ截图20230904203603.png)

### 2、定时器函数基本使用
`setInterval(函数,间隔时间)    //函数名不需要加小括号`
#### (1)开启定时器
![](./images/QQ截图20230904205945.png)
#### (2)关闭定时器
![](./images/QQ截图20230904210204.png)
#### (3)实例代码
```
const btn = document.querySelector('.btn')
    let i = 5
    const n = setInterval(function () {
        i--
        btn.innerHTML = `我已经阅读用户协议(${i})`
        if (i === 0) {
            clearInterval(n)
            btn.disabled = false
            btn.innerHTML = '同意'
        }
    }, 1000)
```

## 六、事件监听
### 1、定义
![](./images/QQ截图20230905142320.png)  

### 2、语法
![](./images/QQ截图20230905142748.png)  
![](./images/QQ截图20230905142826.png)  
 
```
// 点击关闭
const box1 = document.querySelector('.box1')
const box = document.querySelector('.box')

box1.addEventListener('click',function(){
  box.style.display = 'none'
})
```

### 3、事件监听版本(了解)
![](./images/QQ截图20230905154411.png)  
![](./images/QQ截图20230905154701.png)  

### 4、事件类型
![](./images/QQ截图20230905155009.png)
#### (1)鼠标触发
#### (2)焦点事件
```
const input = document.querySelector('input')
input.addEventListener('focus',function(){
  console.log('有焦点');
})
input.addEventListener('blur',function(){
  console.log('失去焦点');
})
```
#### (3)键盘事件
```
// 键盘上按下任意键则会触发keydown事件，抬起键盘则会触发keyup事件 
const input = document.querySelector('input')
input.addEventListener('keydown',function(){
  console.log('keydown');
})

input.addEventListener('keyup',function(){
  console.log('keyup');
})
```

#### (4)用户输入
```
const input = document.querySelector('input')
input.addEventListener('input',function(){
  console.log(input.value);                         //用户的输入通过input.value得到，类型为字符串，可以通过length属性得到
})
```

### 5、事件监听的调用
```
next.addEventListener('click', function () {
  i = (i + 1) % sliderData.length
  toggle()
})

next.click()   //相当于触发了一次click事件
```

### 6、M端事件(了解)
![](./images/QQ截图20230911152743.png)  
```
const div = document.querySelector('div')
div.addEventListener('touchstart',function(){
  console.log('start');
})
div.addEventListener('touchend',function(){ 
  console.log('end');
})
div.addEventListener('touchmove',function(){
  console.log('move');
})
```

## 七、事件对象、环境对象及回调函数
### 1、事件对象
#### (1)定义及使用场景
![](./images/QQ截图20230905173648.png)  

#### (2)语法
![](./images/QQ截图20230905173946.png)

#### (3)事件对象的常用属性
![](./images/QQ截图20230906132320.png)  
![](./images/QQ截图20230906133451.png) ( )
#### (4)示例代码
```
const input = document.querySelector('input')
input.addEventListener('keyup',function(e){        //事件绑定的回调函数的第一个参数，e就是事件对象
  if(e.key === 'Enter')
  console.log('press enter');
})
```

### 2、环境对象
#### (1)定义
![](./images/QQ截图20230906134010.png)

#### (2)指代规则(粗略)
```
const btn = document.querySelector('button')
btn.addEventListener('click', function () {
  console.log(this);                         //此时，this指向button对象
  this.style.color = 'red'                  
})
function fn(){
  console.log(this);                         //此时，this指向windows
}
fn()
```

### 3、回调函数
![](./images/QQ截图20230906144133.png)

## 八、DOM事件
### 1、事件流
#### (1)事件流的两个阶段说明
![](./images/QQ截图20230907165053.png)

#### (2)事件捕获(了解)
![](./images/QQ截图20230907165408.png)
```
//DOM.addEventListener(事件类型,事件处理函数,是否使用捕获机制)，第三个参数为true代表使用事件捕获
//事件捕获代表事件从外到里执行，分别alert document fa son
document.addEventListener('click', function () {
  alert('document')
}, true)
fa.addEventListener('click', function () {
  alert('fa')
}, true)
son.addEventListener('click', function () {
  alert('son')
}, true)
```

#### (3)事件冒泡
mouseenter和mouseleave没有事件冒泡
![](./images/QQ截图20230907171702.png)
```
//DOM.addEventListener(事件类型,事件处理函数,是否使用捕获机制)，默认为冒泡
//事件冒泡代表事件从里到外执行，分别alert son fa document  
document.addEventListener('click', function () {
  alert('document')
})
fa.addEventListener('click', function () {
  alert('fa')
})
son.addEventListener('click', function () {
  alert('son')
})
```

#### (4)阻止冒泡(阻止事件传播)
![](./images/QQ截图20230907172010.png)  
```
// e.stopPropagation()会阻止事件传播，只会alert son
document.addEventListener('click', function () {
  alert('document')
})
fa.addEventListener('click', function () {
  alert('fa')
})
son.addEventListener('click', function (e) {
  alert('son')
  e.stopPropagation()
})
```
### (5)阻止元素默认行为
![](./images/QQ截图20230908132709.png)
```
<a href="http://www.baidu.com">百度一下</a>
const a = document.querySelector('a')
a.addEventListener('click', function (e) {
  e.preventDefault()
})
```

#### (6)解绑事件
![](./images/QQ截图20230907172546.png)  
```
const btn = document.querySelector('button')
function fn() {
  alert('点击了')
}
btn.addEventListener('click', fn)
btn.removeEventListener('click', fn)           // 事件解绑
```

#### (7)传统on注册和事件监听注册的区别
![](./images/QQ截图20230907173310.png)

### 2、事件委托
#### (1)引入
![](./images/QQ截图20230907173648.png)

#### (2)原理及实现
![](./images/QQ截图20230907174904.png)
![](./images/QQ截图20230907175127.png)

#### (3)示例代码
```
<ul>
  <li>第1个孩子</li>
  <li>第2个孩子</li>
  <li>第3个孩子</li>
  <li>第4个孩子</li>
  <li>第5个孩子</li>
  <p>我不需要变色</p>
</ul>
<script>
  // 点击每个小li 当前li 文字变为红色
  // 按照事件委托的方式  委托给父级，事件写到父级身上
  // 1. 获得父元素
  const ul = document.querySelector('ul')
  ul.addEventListener('click', function (e) {
    this.style.color = 'red'         //这会导致所有的li都变为红色
    console.dir(e.target)            //就是我们点击的那个对象，使用的是dir而非log，他俩的区别在下面
    e.target.style.color = 'red'
   
    if (e.target.tagName === 'LI') {    //只要点击li才会有效果,点击p则不会变红
      e.target.style.color = 'red'
    }
  })
```

#### (4)dir与log的区别
`log`语句打印的是结果，直接显示信息；  
`dir`语句打印的是内容，对显示对象的所有属性和方法。  
这样的区别在输出普通数据时没有区别，打印的内容完全一样，在打印对象时就有区别了。  
`console.log()`输出的是对象源代码，
`console.dir()`则输出该对象的内容，所有属性和方法。

### 3、其他事件
### (1)页面加载事件
![](./images/QQ截图20230908133745.png)  
```
// 等待页面所有资源加载完毕，就回去执行回调函数
window.addEventListener('load', function () {
  const btn = document.querySelector('button')
  btn.addEventListener('click', function () {
    alert(11)
  })
})

// 等待图片加载完毕，再去执行里面的代码
img.addEventListener('load', function () {
  //要执行的代码
})
```
![](./images/QQ截图20230908134051.png)
![](./images/QQ截图20230908134424.png)

### (2)元素滚动事件
```
/* 页面滑动 */
html {
  /* 让滚动条丝滑的滚动,不会突兀地跳转 */
  scroll-behavior: smooth;
}
```
![](./images/QQ截图20230908134806.png)   
`scrollTop`和`scrollLeft`是可读写的，返回的数据是数字型的  
![](./images/QQ截图20230908140406.png)  
![](./images/QQ截图20230908135804.png)  
`document.documentElement`是针对整个窗口滚动距离的固定写法，对于某个具体的盒子，可直接写为`DOM.scrollTop`，除此之外，还可以使用`scrollTo(横坐标,纵坐标)`方法使得内容滚动到指定的坐标，与使用`scrollTop`和`scrollLeft`属性来改变位置可以得到相同的效果    
```
window.addEventListener('scroll', function () {
  console.log('我滚了')
  // 我想知道页面到底滚动了多少像素， 被卷去了多少scrollTop
  // 获取html元素写法  
  document.documentElement  
  console.log(document.documentElement.scrollTop)
  const n = document.documentElement.scrollTop
})
```
### (3)页面尺寸事件
![](./images/QQ截图20230908143238.png)  
![](./images/QQ截图20230908143659.png)

### 4、元素尺寸与位置
#### (1)元素尺寸
`offsetWidth,offsetHeight`与`clientWidth,clientHeight`的区别就=在于是否包含边框的宽度
![](./images/QQ截图20230908144145.png)  
#### (2)元素位置
`offsetLeft`和`offsetTop`是距离自己有定位的父级元素的距离，若父级元素没有被定位，则向更高一级的父元素寻找  
![](./images/QQ截图20230908144313.png)   
相对于视口的位置，如果发生滚动，盒子的位置发生改变    
![](./images/QQ截图20230908162401.png)

### 5、总结
![](./images/QQ截图20230908162728.png)  

## 九、日期对象
### (1)实例化
![](./images/QQ截图20230909144716.png)
```
// 得到当前时间
const date = new Date()
console.log(date);

// 指定时间
const date1 = new Date('2022-5-6')
console.log(date1);
```


### (2)日期对象方法
![](./images/QQ截图20230909144837.png)  
```
const date = new Date()
console.log(date.getFullYear())    // 得到年份
console.log(date.getMonth()+1)     // 获得月份，注意要加1
console.log(date.getDate())        // 获取月份中的某一天
console.log(date.getDay())         // 周日的取值为0，取值为0~9
console.log(date.toLocaleString()) // 返回2023/9/9 14:59:40这种格式的时间 
console.log(date.toLocaleDateString())   //返回2023/9/9
console.log(date.toLocaleTimeString())   //返回14:59:40
```

### (3)时间戳
#### 定义
![](./images/QQ截图20230909150611.png)  
#### 语法
![](./images/QQ截图20230909150944.png)  
`new Date()`返回的字符串通过隐式转换转换为时间戳
```
console.log(+new Date())                          // 获取当前时间的时间戳
console.log(+new Date('2022-4-1 18:30:00'))       // 获取指定时间的时间戳
```

## 十、节点操作
### 1、DOM节点
![](./images/QQ截图20230909171637.png)

### 2、查找节点
![](./images/QQ截图20230909171839.png)
#### (1)父节点查找
![](./images/QQ截图20230911142931.png)
#### (2)子节点查找
![](./images/QQ截图20230911143357.png)
#### (3)兄弟节点查找
![](./images/QQ截图20230911143926.png)

### 3、增加节点
![](./images/QQ截图20230911144326.png)  
#### (1)创建节点
![](./images/QQ截图20230911144828.png)
#### (2)追加节点
![](./images/QQ截图20230911144750.png)
```
// append插入最后一个位置
const div =document.createElement('div')
document.body.append(div)

// 插入某个元素前面
const ul = document.querySelector('ul')
const li =document.createElement('li')
li.innerHTML='I am li'
ul.insertBefore(li,ul.children[0])
```
#### (3)克隆节点
布尔值选择false，则只会克隆标签，不会克隆后代节点，也不会克隆其内容  
![](./images/QQ截图20230911151136.png)
```
// 先克隆，再追加
const ul = document.querySelector('ul')
const li1 = ul.children[0].cloneNode(true)
ul.append(li1)
```
### 4、删除节点
![](./images/QQ截图20230911152444.png)  


### 5、swiper插件
![](./images/QQ截图20230911153348.png)
`https://www.bilibili.com/video/BV1Y84y1L7Nn?t=1822.0&p=124`

## 十一、Window对象
### 1、BOM(浏览器对象模型)
![](./images/QQ截图20230911200955.png)

### 2、定时器-延时函数
#### (1)语法
![](./images/QQ截图20230913134837.png)
#### (2)与间歇函数的区别
![](./images/QQ截图20230913135009.png)

### 3、JS执行机制
#### (1)单线程
![](./images/QQ截图20230913135203.png)
#### (2)同步和异步
![](./images/QQ截图20230913135339.png)  
![](./images/QQ截图20230913135424.png)
#### (3)同步任务和异步任务的执行机制
![](./images/QQ截图20230913135615.png)
![](./images/QQ截图20230913140045.png)

### 4、location对象
#### (1)location.href属性
获取完整的url地址，对其赋值网页会直接跳转，不需使用a标签的点击  
![](./images/QQ截图20230913141624.png)
#### (2)location.search属性
![](./images/QQ截图20230913153256.png)
#### (3)location.hash属性
hash属性获取地址中的哈希值，符号#后面部分  
![](./images/QQ截图20230913153843.png)  
`https://music.163.com/#/friend`  
`https://music.163.com/#/my/`  
`https://music.163.com/#/download`  
#### (4)location.reload()方法
![](./images/QQ截图20230913154013.png)  
```
location.reload()
location.reload(true)
```
### 5、navigator对象
![](./images/QQ截图20230913155208.png)  

### 6、history对象
![](./images/QQ截图20230913155849.png)

## 十二、本地存储
### 1、本地存储介绍
![](./images/QQ截图20230913161710.png)  

### 2、本地存储分类
#### (1)localStorage 
##### 作用及特性
本地存储只能存储字符串型数据，即使是数字型数据也会修改为字符串型   
![](./images/QQ截图20230913161805.png)  
##### 存
`localStorage.setItem('uname','pink')`  
![](./images/QQ截图20230913162234.png)
##### 取
`console.log(localStorage.getItem('uname'))`  
##### 删
`localStorage.removeItem('uname')`
##### 改
`localStorage.setItem('uname','red')           // 有则改，无则增`  

#### (2)session-Storage
#### 特性
![](./images/QQ截图20230913163510.png)  

### 3、存储复杂数据类型
#### (1)无法直接存储复杂数据类型
![](./images/QQ截图20230913164015.png)
#### (2)解决方案 
![](./images/QQ截图20230913165627.png)
![](./images/QQ截图20230913165443.png)  
`const arr = JSON.parse(localStorage.getItem('data')) || []`，若localStorage为空，则使数组为空，这种写法利用了逻辑中断，简化了代码量  
```
const obj = {
  uname: 'pink',
  age: 18
}
// JSON对象，属性和值都有统一有双引号
localStorage.setItem('obj',JSON.stringify(obj))
//得到JSON类型字符串{"uname":"pink","age":18}
console.log(localStorage.getItem('obj'))      
// 将JSON字符串转换为对象 
console.log(JSON.parse(localStorage.getItem('obj')))      
```

### 4、利用map()和join()数组方法实现字符串拼接
#### (1)map()
![](./images/QQ截图20230913171727.png)  
```
const arr = ['red', 'blue', 'pink']
const newArr = arr.map(function (ele, index) {
  console.log(ele)
  console.log(index)
  return ele + 'color'
})

console.log(arr)
console.log(newArr)
```
#### (2)join()
小括号为空，则元素之间无分割，无参数则默认用逗号分隔  
![](./images/QQ截图20230914145623.png)

#### (3)数组中map()和join()方法渲染页面思路
![](./images/QQ截图20230914150213.png)  
```
function render() {
  // (1)利用map遍历数组，返回对应tr的数组
  const trArr = arr.map(function (ele, index) {
    return `<tr>
              <td>${ele.stuId}</td>
              <td>${ele.uname}</td>
              <td>${ele.age}</td>
              <td>${ele.stuId}</td>
              <td>${ele.salary}</td>
              <td>${ele.city}</td>
              <td>
                <a href="javascript:" data-ID='${index}'>删除</a>
              </td>
            </tr> 
            `
  })
  // (2)把数组转换为字符串join()
  // (3)把生成的字符串追加给tbody
  tbody.innerHTML = trArr.join('')
}
```

## 十三、正则表达式
### 1、介绍
#### (1)定义
![](./images/QQ截图20230914181812.png)
#### (2)使用场景
![](./images/QQ截图20230914181854.png)  

### 2、语法
![](./images/QQ截图20230914182311.png)  
#### (1)定义规则
![](./images/QQ截图20230914182541.png)  
#### (2)匹配
![](./images/QQ截图20230914182819.png)  
```
const str = '正在学习前端'
// 定义规则
const reg = /前端/
// 是否匹配
console.log(reg.test(str))
// 简便写法
console.log(/前端/.test('正在学习前端'))
```
#### (3)exec()
![](./images/QQ截图20230914183032.png)  

### 3、元字符
#### (1)定义
![](./images/QQ截图20230914183527.png)  
#### (2)边界符
![](./images/QQ截图20230914184540.png)  
```
console.log(/^哈/.test('哈'))           //true
console.log(/^哈/.test('二哈'))         //false
console.log(/^哈$/.test('哈'))          //true 只有这种情况为true
console.log(/^哈$/.test('哈哈'))        //false 精确匹配，只能有一个‘哈’
``` 
![](./images/QQ截图20230914191844.png)  

#### (3)量词(表示重复次数)
![](./images/QQ截图20230914200055.png)  
![](./images/QQ截图20230914200120.png)  


#### (4)[]匹配字符集合
![](./images/QQ截图20230915141339.png)  
![](./images/QQ截图20230915141929.png)  
![](./images/QQ截图20230915142004.png)  
![](./images/QQ截图20230915142102.png)  
.匹配换行符之外的任何单个字符

#### (5)预定义
![](./images/QQ截图20230915153748.png)  

### 4、修饰符
![](./images/QQ截图20230915153952.png)  
```
console.log(/^java$/.test('java'))
console.log(/^java$/i.test('JAVA'))
console.log(/^java$/i.test('Java'))
const str = 'java是一门编程语言， 学完JAVA工资很高'
// const re = str.replace(/java|JAVA/g, '前端')
const re = str.replace(/java/ig, '前端')
console.log(re)  // 前端是一门编程语言， 学完前端工资很高
```
```
<textarea name="" id="" cols="30" rows="10"></textarea>
<button>发布</button>
<div></div>
<script>
  const tx = document.querySelector('textarea')
  const btn = document.querySelector('button')
  const div = document.querySelector('div')
  btn.addEventListener('click', function () {
    // console.log(tx.value)
    div.innerHTML = tx.value.replace(/激情|基情/g, '**')
    tx.value = ''
  })
</script>
```

# JS进阶









