---
title: "Unit"
second_title: "Aspose.Cells for Java API 参考"
description: "表示长度测量"
type: docs
url: /zh/java/com.aspose.gridweb/unit/
---

**Inheritance:**
java.lang.Object
```
public class Unit
```

表示长度测量
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Unit()](#Unit--) | 默认构造函数 |
| [Unit(double value, int type)](#Unit-double-int-) | 使用指定的双精度浮点数和 UnitType 初始化 Unit 结构的新实例。 |
| [Unit(double value)](#Unit-double-) | 使用指定的双精度浮点数初始化 Unit 结构的新实例。 |
| [Unit(int value)](#Unit-int-) | 使用指定的 32 位有符号整数初始化 Unit 结构的新实例。 |
| [Unit(String value)](#Unit-java.lang.String-) | 使用指定的长度初始化 Unit 结构的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [GetExtension(int type)](#GetExtension-int-) | 根据类型获取字符串，可能得到 "px"、"pt"、"%" 等； |
| [Parse(String s)](#Parse-java.lang.String-) | 将指定的字符串转换为 Unit。 |
| [Percentage(double n)](#Percentage-double-) | 根据指定的双精度浮点数创建 Percentage 类型的 Unit。 |
| [Pixel(int n)](#Pixel-int-) | 根据指定的 32 位有符号整数创建 Pixel 类型的 Unit。 |
| [Point(int n)](#Point-int-) | 根据指定的 32 位有符号整数创建 Point 类型的 Unit。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | 获取 Unit 的单位类型。 |
| [getValue()](#getValue--) | 获取 Unit 的长度。 |
| [hashCode()](#hashCode--) |  |
| [isEmpty()](#isEmpty--) | 获取指示 Unit 是否为空的值。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | 获取单位的字符串表示形式。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Unit() {#Unit--}
```
public Unit()
```


默认构造函数

### Unit(double value, int type) {#Unit-double-int-}
```
public Unit(double value, int type)
```


使用指定的双精度浮点数和 UnitType 初始化 Unit 结构的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |
| 类型 | int |  |

### Unit(double value) {#Unit-double-}
```
public Unit(double value)
```


使用指定的双精度浮点数初始化 Unit 结构的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### Unit(int value) {#Unit-int-}
```
public Unit(int value)
```


使用指定的 32 位有符号整数初始化 Unit 结构的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### Unit(String value) {#Unit-java.lang.String-}
```
public Unit(String value)
```


使用指定的长度初始化 Unit 结构的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### GetExtension(int type) {#GetExtension-int-}
```
public static String GetExtension(int type)
```


根据类型获取字符串，可能得到 "px"、"pt"、"%" 等；

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 类型 | int |  |

**Returns:**
java.lang.String
### Parse(String s) {#Parse-java.lang.String-}
```
public static Unit Parse(String s)
```


将指定的字符串转换为 Unit。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| s | java.lang.String |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Percentage(double n) {#Percentage-double-}
```
public static Unit Percentage(double n)
```


根据指定的双精度浮点数创建 Percentage 类型的 Unit。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| n | double |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Pixel(int n) {#Pixel-int-}
```
public static Unit Pixel(int n)
```


根据指定的 32 位有符号整数创建 Pixel 类型的 Unit。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| n | int |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Point(int n) {#Point-int-}
```
public static Unit Point(int n)
```


根据指定的 32 位有符号整数创建 Point 类型的 Unit。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| n | int |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getType() {#getType--}
```
public int getType()
```


获取 Unit 的单位类型。

**Returns:**
int
### getValue() {#getValue--}
```
public double getValue()
```


获取 Unit 的长度。

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


获取指示 Unit 是否为空的值。

**Returns:**
boolean -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### toString() {#toString--}
```
public String toString()
```


获取单位的字符串表示形式。

**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

