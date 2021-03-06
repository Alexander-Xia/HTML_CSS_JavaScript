### 技术交流QQ群:1027579432，欢迎你的加入！
#### 1.循环结构
- 循环的目的：在实际问题中，有很多**规律性的重复操作**。因此，在程序中要完成这类操作，就需要**重复执行某些语句**。
#### 2.JS中的循环
- 在JS中主要有三种类型的循环语句：
    - for循环
    - while循环
    - do-while循环
##### for循环
- 在程序中，一组被重复执行的语句被称为**循环体**，能否继续重复执行，取决于循环的**终止条件**。由循环体及循环的终止条件组成的语句，被称为**循环语句**。
- **语法结构**：
    - for循环主要用于把某些代码循环若干次，通常与计数有关，语法结构如下：
    ```
    for (初始化变量; 条件表达式; 操作表达式) {
        // 循环体
    }
    ```
- **断点调试**：
    - 断点调试是指自己在程序的某一行设置一个断点。调试时，程序运动到这一行就停止，然后你可以一步一步往下调试，调试过程可以看每个变量当前的值。出错的话，调试到出错的代码行即显示错误，停止程序运行。
    - **浏览器中按下F12，之后再找到Sources，找到需要可以监视变量的值的变化**。
    - **F11：程序单步执行，让程序一行一行的执行，这个时候，观察Watch中变量的值变化**。
#### 3.双重for循环
- 很多情况下，单层for循环并不能满足我们的需求，例如需要打印出5\*5的图形，打印一个倒直角三角性等，此时就可以通过嵌套来实现。
- **嵌套循环**：是指一个**循环语句中再定义一个循环语句的语法结构**，例如在for循环中可以再嵌套一个for循环，这样的for循环语句我们称为**双重for循环**。
- 双重for循环的语法结构：
    ```
    for (外层的初始化变量; 外层的条件表达式; 外层的操作表达式){
        for (里层的初始化变量; 里层的条件表达式; 里层的操作表达式) {
            // 操作语句;
        }
    }
    ```
- 可以把里层的循环看成是外层循环的语句。
- 外层循环执行一次，里层的循环执行全部。
#### 4.for循环总结
- for循环可以重复执行某些相同的代码；
- for循环可以重复执行一些不同的代码，因为有计数器的存在；
- for循环可以重复执行某些操作，例如算术运算符、加法操作；
- 双层for循环，外层循环执行一次，内层for循环执行全部；
- for循环是循环条件和数字直接相关的循环；
#### 5.while循环
- while语句可以在条件表达式为真的前提下，循环执行特定的一段代码，直到表达式不为真时结束循环。
- while语句的语法结构如下：
    ```
    while (条件表达式) {
        // 循环体代码
    }
    ```
#### 6.do-while循环
- do-while循环实际上是while循环语句的一个变体，该循环会先执行一次代码块，然后对条件表达式进行判断，如果条件为真，则会重复执行循环体，否则退出循环。
- 语法结构：
    ```
    do {
        // 循环体
    } while (条件表达式)
    ```
- **先执行循环体，再判断。因此，do-while循环体至少执行一次**！
#### 7.循环的总结
- JS中的循环有for、while、do-while；
- 三个循环很多情况下都可以相互替换使用；
- 如果是用来计次数的，与数字相关的，三者使用基本相同，但更偏爱使用for循环；
- while和do-while循环可以用来做更复杂的判断条件，比for循环更加灵活；
- while和do-while执行的顺序不一样，while是先判断后执行，do-while是先执行一次，再判断执行；
- while和do-while执行的次数不一样，do-while的循环体至少会被执行一次，而while的循环体可能一次也不执行；
#### 8.continue和break关键字
- **continue关键字是用于立即跳出本次循环，继续下一次循环**，本次循环体中continue之后的代码会少执行一次。
- **break关键字用于立即跳出整个循环**，循环立即结束。
#### 9.JS中的命名规范及语法格式
- **标识符命名规范**
    - 函数名、变量名的命名必须要有意义；
    - 变量的名称一般用名词；
    - 函数的名称一般用动词；
- **操作符规范**
```
// 操作符的左右两侧各保留一个空格
for (var i = 1; i <= 5; i++) {
    if (i === 3) {
        break;
    }
    console.log('我正在吃第' + i + '个包子.');
}
```
- **单行注释规范**
    ```
    
    for (var i = 1; i <= 5; i++) {
        if (i === 3) {
            break;  // 单行注释前面注意有个空格
        }
        console.log('我正在吃第' + i + '个包子.');
    }
    ```
- **其他规范**
    ```
    if (true) {  // 注意括号左右各留有一个空格
        
    }
    
    for (var i = 1; i <= 100; i++) {
        
    }
    ```
#### 10.资料下载
- [笔记及代码，欢迎star,follow,fork......](https://github.com/cdlwhm1217096231/HTML_CSS_JavaScript/tree/master/JavaScript)