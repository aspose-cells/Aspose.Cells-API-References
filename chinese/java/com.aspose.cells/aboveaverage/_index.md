---
title: "AboveAverage"
second_title: "Aspose.Cells for Java API 参考"
description: "描述 AboveAverage 条件格式规则。"
type: docs
url: /zh/java/com.aspose.cells/aboveaverage/
---

**Inheritance:**
java.lang.Object
```
public class AboveAverage
```

描述 AboveAverage 条件格式规则。此条件格式规则突出显示范围内所有值的高于或低于平均值的单元格。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [AboveAverage()](#AboveAverage--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getStdDev()](#getStdDev--) | 获取在条件格式规则中包含的高于或低于平均值的标准差数量。 |
| [hashCode()](#hashCode--) |  |
| [isAboveAverage()](#isAboveAverage--) | 获取指示规则是否为"above average"规则的标志。 |
| [isEqualAverage()](#isEqualAverage--) | 获取指示 'aboveAverage' 和 'belowAverage' 条件是包含平均值本身还是排除该值的标志。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAboveAverage(boolean value)](#setAboveAverage-boolean-) | 设置指示规则是否为"above average"规则的标志。 |
| [setEqualAverage(boolean value)](#setEqualAverage-boolean-) | 设置指示 'aboveAverage' 和 'belowAverage' 条件是否包含平均值本身，或排除该值的标志。 |
| [setStdDev(int value)](#setStdDev-int-) | 设置在条件格式规则中包含平均值上方或下方的标准差数量。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AboveAverage() {#AboveAverage--}
```
public AboveAverage()
```


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
### getStdDev() {#getStdDev--}
```
public int getStdDev()
```


获取在条件格式规则中包含平均值上方或下方的标准差数量。输入值必须在 0 到 3 之间（包括 0 和 3）。将此值设为 0 表示未设置 stdDev。默认值为 0。

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAboveAverage() {#isAboveAverage--}
```
public boolean isAboveAverage()
```


获取指示规则是否为“above average”（高于平均）规则的标志。'true' 表示“above average”。默认值为 true。

**Returns:**
boolean
### isEqualAverage() {#isEqualAverage--}
```
public boolean isEqualAverage()
```


获取指示 'aboveAverage' 和 'belowAverage' 条件是否包含平均值本身，或排除该值的标志。'true' 表示在条件中包含平均值。默认值为 false。

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAboveAverage(boolean value) {#setAboveAverage-boolean-}
```
public void setAboveAverage(boolean value)
```


设置指示规则是否为“above average”（高于平均）规则的标志。'true' 表示“above average”。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEqualAverage(boolean value) {#setEqualAverage-boolean-}
```
public void setEqualAverage(boolean value)
```


设置指示 'aboveAverage' 和 'belowAverage' 条件是否包含平均值本身，或排除该值的标志。'true' 表示在条件中包含平均值。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setStdDev(int value) {#setStdDev-int-}
```
public void setStdDev(int value)
```


设置在条件格式规则中包含平均值上方或下方的标准差数量。输入值必须在 0 到 3 之间（包括 0 和 3）。将此值设为 0 表示未设置 stdDev。默认值为 0。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

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

