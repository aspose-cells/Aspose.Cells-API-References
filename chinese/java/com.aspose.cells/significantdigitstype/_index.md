---
title: "SignificantDigitsType"
second_title: "Aspose.Cells for Java API 参考"
description: "表示用于输出数值的有效数字类型。"
type: docs
url: /zh/java/com.aspose.cells/significantdigitstype/
---

**Inheritance:**
java.lang.Object
```
public final class SignificantDigitsType
```

表示用于输出数值的有效数字类型。
## 字段

| 字段 | 描述 |
| --- | --- |
| [DIGITS_15](#DIGITS-15) | 15位 |
| [G_17](#G-17) | 通过使用 "G17" 格式化值来获得 17 位。 |
| [ROUNDING_17](#ROUNDING-17) | 通过对值进行四舍五入来获得 17 位。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DIGITS_15 {#DIGITS-15}
```
public static final int DIGITS_15
```


15位

### G_17 {#G-17}
```
public static final int G_17
```


通过使用 "G17" 格式化值来获得 17 位。

**Remarks**

对于某些 double 值，"G17" 可能会给出与用户输入的原始/文字值不同的结果。例如，double 值 0.15 将输出为 0.14999999999999999；double 值 1.0E-16 将输出为 9.9999999999999998E-17。Ms excel 对这些值的处理不一致，它在 xlsx 文件中将 0.15 保存为 0.15，但对于 1.0E-16，保存的值是 9.9999999999999998E-17。

### ROUNDING_17 {#ROUNDING-17}
```
public static final int ROUNDING_17
```


通过对值进行四舍五入来获得 17 位。

**Remarks**

此类型通常将值输出为用户输入的原始/文字值。对于 0.15，它产生 "0.15"，对于 1.0E-16，它产生 "1.0E-16"。但也有一些特殊情况可能会给出与文字值不同的结果。例如，当将 208435494.96478021 四舍五入为 17 位（"0.\\#\\#\\#\\#\\#\\#\\#\\#\\#\\#\\#\\#\\#\\#\\#\\#"）时，输出为 208435494.96478。

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
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
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

