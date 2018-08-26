# Java 命名

<!-- toc -->

## 网址
* [industry-glossary](https://github.com/biezhi/industry-glossary)
* [CodeLF](https://unbug.github.io/codelf/)

## 字面命名（typographical）
摘自 effective java

### 包
* 包名的元素应该比较简短，通常不超过 8 个 字符，鼓励有意义的缩写

### 类和接口
* 类和接口应该尽量避免使用缩写

### 类型参数
* 类型参数通常由单个字母表示，通常使用几个字母
    - `T` 表示任意的类型
    - `E` 表示集合的元素类型
    - `K` `V` 表示键和值
    - `X` 表示异常
    - `R` 函数式方法的返回值
    - `T` `U` `V` 或者 `T1` `T2` `T3` 任意类型序列

## 语法命名
### 类
+ 类通常用一个名词或者名词短语来命名
    - `Timer` `BufferWriter`
+ 接口命名和类似，也可以以 `-able` 或者 `-ible` 结尾
    - `Collection` `Compatator`
    - `Runnable` `Iterable` `Accessible`
+ 注解没有固定的词类，名词、动词、形容词、介词都可以使用
    - `BindingAnnotation` `Inject` `ImplementedBy` `Singleton`

### 方法
+ 执行某个动作的方法通常用动词或者动词短语来命名
    - `append` `drawImage`
+ 对于返回 boolean 值的一般使用 `is`（或者 `has`，不太常用）加名词、名词短语或者具有形容词功能的单词和短语    
    - `isDigit` `isProbablePrime` `isEmpty` `isEnabled` `hasSiblings`
+ 如果方法返回对象的非 boolean 属性，通常以名词、名词短语或者以 `get` 开头的动词短
    - `size` `hashCode` `getTime`
+ 返回转换对象的或者返回不同独立类型对象的方法，通常以 `to<Type>` 命名
    - `toArray` `toString`
+ 如果方法返回一个 view 类型，通常以 `as<Type>` 命名
    - `asList`
+ 返回和调用对象相同值的基本类型，通常以 `<Type>Value` 命名
    - `intValue`
+ 静态工厂方法
    - `from` `of` `valueOf` `instance` `getInstance` `newInstance` `get<Type>` `new<Type>`
