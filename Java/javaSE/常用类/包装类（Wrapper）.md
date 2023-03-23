
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
