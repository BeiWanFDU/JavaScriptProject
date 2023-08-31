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
![](./images/QQ截图20230825151754.png)
`prompt('input your name')`

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
// 语法1
(function (){})()
// 语法2
(function(){}())
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