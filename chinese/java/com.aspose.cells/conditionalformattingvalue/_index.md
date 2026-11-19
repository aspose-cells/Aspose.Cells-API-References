---
title: "ConditionalFormattingValue"
second_title: "Aspose.Cells for Java API 参考"
description: "描述渐变刻度 dataBar 或 iconSet 中插值点的值。"
type: docs
url: /zh/java/com.aspose.cells/conditionalformattingvalue/
---

**Inheritance:**
java.lang.Object
```
public class ConditionalFormattingValue
```

描述渐变刻度、dataBar 或 iconSet 中插值点的值。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | 获取此条件格式化值对象的类型。 |
| [getValue()](#getValue--) | 获取此条件格式化值对象的值。 |
| [hashCode()](#hashCode--) |  |
| [isGTE()](#isGTE--) | 获取 Greater Than Or Equal 标志。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setGTE(boolean value)](#setGTE-boolean-) | 设置 Greater Than Or Equal 标志。 |
| [setType(int value)](#setType-int-) | 设置此条件格式化值对象的类型。 |
| [setValue(Object value)](#setValue-java.lang.Object-) | 设置此条件格式化值对象的值。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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


获取此条件格式化值对象的类型。将类型设置为 FormatConditionValueType.Min 或 FormatConditionValueType.Max 将自动将 "Value" 设为 null。

参见 [FormatConditionValueType](../../com.aspose.cells/formatconditionvaluetype)。

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


获取此条件格式化值对象的值。它应与 Type 结合使用。

**Remarks**

如果值是字符串且以 "=" 开头，它将被处理为公式，否则我们将把它作为普通值处理。

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGTE() {#isGTE--}
```
public boolean isGTE()
```


获取 Greater Than Or Equal 标志。仅用于图标集，决定此阈值是否使用大于等于运算符。'false' 表示使用大于而不是大于等于。默认值为 true。

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




### setGTE(boolean value) {#setGTE-boolean-}
```
public void setGTE(boolean value)
```


设置 Greater Than Or Equal 标志。仅用于图标集，决定此阈值是否使用大于等于运算符。'false' 表示使用大于而不是大于等于。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


设置此条件格式化值对象的类型。将类型设置为 FormatConditionValueType.Min 或 FormatConditionValueType.Max 将自动将 "Value" 设为 null。

参见 [FormatConditionValueType](../../com.aspose.cells/formatconditionvaluetype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


设置此条件格式化值对象的值。它应与 Type 结合使用。

**Remarks**

如果值是字符串且以 "=" 开头，它将被处理为公式，否则我们将把它作为普通值处理。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object |  |

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

