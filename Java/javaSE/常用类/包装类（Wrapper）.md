
![[Pasted image 20230323184142.png]]


# 包装类

## 基本数据类型的转换

1. jdk5以前用的手动装箱，以后用的是自动装箱
2. 自动装箱用的是 **valueOf** 方法，比如 **Intereger.valueOf ( )**


## String 类型的转换

与基本数据类型类似

其中 Character 有些重要的方法

```java
System.out.println(Integer.MIN_VALUE); //返回最小值
System.out.println(Integer.MAX_VALUE);//返回最大值
System.out.println(Character.isDigit('a'));//判断是不是数字
System.out.println(Character.isLetter('a'));//判断是不是字母
System.out.println(Character.isUpperCase('a'));//判断是不是大写
System.out.println(Character.isLowerCase('a'));//判断是不是小写
System.out.println(Character.isWhitespace('a'));//判断是不是空格
System.out.println(Character.toUpperCase('a'));//转成大写
System.out.println(Character.toLowerCase('A'));//转成小写
```



## String

1. string 对象用来保存字符串

![[Pasted image 20230323190349.png]]

![[Pasted image 20230323190804.png]]

### 字符串的特性

1. string 是一个 final 类

### String 的常见方法

![[Pasted image 20230323191510.png]]

![[Pasted image 20230323191553.png]]

#### **StringBuffer**

![[Pasted image 20230323192224.png]]

```java

String str = "hello tom";

//方式1 使用构造器
StringBuffer stringBuffer = new StringBuffer(str);

//方式2 使用的是append 方法
StringBuffer stringBuffer1 = new StringBuffer();
stringBuffer1 = stringBuffer1.append(str);

//看看StringBuffer ->String
StringBuffer stringBuffer3 = new StringBuffer("韩顺平教育");

//方式1 使用StringBuffer 提供的toString 方法
String s = stringBuffer3.toString();

//方式2: 使用构造器来搞定
String s1 = new String(stringBuffer3);

```

StringBuffer 常用方法

```java

StringBuffer s = new StringBuffer("hello");
//增
s.append(',');// "hello,"
s.append("张三丰");//"hello,张三丰"
s.append("赵敏").append(100).append(true).append(10.5);//"hello,张三丰赵敏100true10.5"
System.out.println(s);//"hello,张三丰赵敏100true10.5"
//删
/*
* 删除索引为>=start && <end 处的字符
* 解读: 删除11~14 的字符[11, 14)
*/
s.delete(11, 14);
System.out.println(s);//"hello,张三丰赵敏true10.5"
//改
//老韩解读，使用周芷若替换索引9-11 的字符[9,11)
s.replace(9, 11, "周芷若");
System.out.println(s);//"hello,张三丰周芷若true10.5"
//查找指定的子串在字符串第一次出现的索引，如果找不到返回-1
int indexOf = s.indexOf("张三丰");
System.out.println(indexOf);//6

```


### StringBuilder

![[Pasted image 20230323194907.png]]

![[Pasted image 20230323195150.png]]

### Math

![[Pasted image 20230323195212.png]]

### Array

![[Pasted image 20230323195417.png]]


![[Pasted image 20230323195421.png]]

