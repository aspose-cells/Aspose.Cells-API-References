---
title: "CustomFunctionDefinition"
second_title: "Aspose.Cells for Java API 参考"
description: "使用用户自定义引擎进行计算的自定义函数定义。"
type: docs
url: /zh/java/com.aspose.cells/customfunctiondefinition/
---

**Inheritance:**
java.lang.Object
```
public class CustomFunctionDefinition
```

自定义函数的定义，用于使用用户的自定义引擎进行计算。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [CustomFunctionDefinition()](#CustomFunctionDefinition--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArrayModeParameters(String functionName)](#getArrayModeParameters-java.lang.String-) | 获取给定自定义函数的参数中需要在数组模式下计算的索引。 |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CustomFunctionDefinition() {#CustomFunctionDefinition--}
```
public CustomFunctionDefinition()
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
### getArrayModeParameters(String functionName) {#getArrayModeParameters-java.lang.String-}
```
public int[] getArrayModeParameters(String functionName)
```


获取给定自定义函数的参数中需要在数组模式下计算的索引。

**Remarks**

对于需要计算的表达式，以 A:A+B:B 为例：通常在数值模式下，它会根据当前单元格基准计算为单个值。但在数组模式下，A1+B1、A2+B2、A3+B3、……的所有值都会被计算并用于计算。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| functionName | java.lang.String | 自定义函数的名称。 |

**Returns:**
int[] - 给定自定义函数中需要在数组模式下计算的参数索引。默认值为 null，表示该自定义函数没有需要在数组模式下计算的参数。
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

