### 命名规范

- js/ts文件，全小写命名
- 组件jsx/tsx，Pascal 命名法，例如 ReservationCard.jsx
- 组件文件也可以js/ts后缀，建议jsx/tsx后缀

为什么建议组件使用jsx后缀，因为有些团队认为，jsx严格意义上不算是js的语法，所以纯js语法的文件就以js后缀结束，使用jsx语法的就以jsx后缀结束。但实际上没什么区别，都可以编译

### 基本书写

- 使用两个空格进行缩进
- 除了缩进，其他地方不使用多个空格
- 不在句末使用分号
- 字符串统一使用单引号
- 代码块中避免多余空格
- 函数声明时，参数小括号前后带空格
- 展开运算符与表达式之间不用空格
- 遇到分号，空格后留前不留
- 代码块{}首尾留空格
- 圆括号中间不留空格
- 注释收尾留空格
- 模板字符串变量前后不留空格
- 逗号后面加空格
- 单行代码块两边加空格{ a }
- 键值对中冒号与值之间留空格，与键之间不留空格
- 一个const/let关键字只声明一个变量
- 不使用undefined初始化变量
- 变量和函数名统一使用驼峰命名法

### 基本类型

- 字符串拼接操作符前后留空格
- 检查NaN使用isNaN()

### 对象与数组

- 与存值器(set)就要有取值器(get)
- 使用数组字面量，不使用构造器
- 不解构空值
- 不扩展原生变量
- 外部变量不与对象属性重名

### 函数

- 不使用eval()
- 嵌套代码块中禁止再定义函数
- 禁止使用Function和Object构造器
- 自调用匿名函数时使用小括号包裹
- 不使用generator函数

### 类定义

- 类名大写字母开头
- 子类构造器中一定要调用super
- 使用this前确保super已调用

### 模块

- 同一模块有多个导入时一次性写完

### 语句

- 避免在return语句中出现赋值语句
- 禁止使用with
- 使用===代替==
- if/else关键字要与花括号在同一行
- if语句花括号不省略
- 三元运算符的?和:要与他们负责的代码处于同一行
- 尽量不适用三元表达式
- 使用Promise一定要捕捉错误

### 组件及JSX书写规范

- 组件创建，组件以类的形式进行创建，单个文件中只存在单个组件
- jsx属性均使用单引号
- 多个属性多行书写，标签结束另起一行
- 始终在闭合标签前面加一个空格
- 属性名使用驼峰命名法
- 当标签没有子元素时使用自闭合标签
- 注意书写顺序，看官方文档
- 组件最好定义defaultProps

### Taro自身限制

- 不能使用Array#map之外的方法操作JSX数组，forEach，filter
