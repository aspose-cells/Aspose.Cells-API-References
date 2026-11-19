---
title: "CalculationPrecisionStrategy"
second_title: "Aspose.Cells for Java API 参考"
description: "枚举处理计算精度的策略。"
type: docs
url: /zh/java/com.aspose.cells/calculationprecisionstrategy/
---

**Inheritance:**
java.lang.Object
```
public final class CalculationPrecisionStrategy
```

枚举处理计算精度的策略。由于 IEEE 754 浮点运算的精度问题，一些\"看似简单\"的公式可能无法得到预期结果。例如公式 \"=-0.45+0.43+0.02\"，直接使用 '+' 运算符计算操作数时，结果不是零。针对这种精度问题，某些特殊策略可能会得到预期结果。
## 字段

| 字段 | 描述 |
| --- | --- |
| [DECIMAL](#DECIMAL) | 在可能的情况下使用十进制作为操作数。 |
| [NONE](#NONE) | 未对计算应用任何策略。 |
| [ROUND](#ROUND) | 根据有效数字对计算结果进行四舍五入。 |
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
### DECIMAL {#DECIMAL}
```
public static final int DECIMAL
```


在可能的情况下使用 decimal 作为操作数。性能最差。

### NONE {#NONE}
```
public static final int NONE
```


未对计算应用任何策略。计算时仅使用原始 double 值作为操作数并直接返回结果。性能最高，适用于大多数情况。

### ROUND {#ROUND}
```
public static final int ROUND
```


根据有效数字对计算结果进行四舍五入。

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

