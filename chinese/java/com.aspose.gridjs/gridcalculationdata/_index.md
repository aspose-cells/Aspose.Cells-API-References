---
title: "GridCalculationData"
second_title: "Aspose.Cells for Java API 参考"
description: "表示在计算单个函数（例如函数名称、参数等）时所需的数据。"
type: docs
url: /zh/java/com.aspose.gridjs/gridcalculationdata/
---

**Inheritance:**
java.lang.Object
```
public class GridCalculationData
```

表示计算单个函数时所需的数据，例如函数名称、参数等。

**Remarks**

此类提供的所有对象仅用于“读取”目的。用户不应在公式计算过程中更改工作簿中的任何数据，否则可能导致意外结果或异常。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | 获取此函数的计算值。 |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | 获取函数所在的单元格列索引。 |
| [getFormula()](#getFormula--) | 获取函数所在的单元格公式。 |
| [getFunctionName()](#getFunctionName--) | 获取要计算的函数名称。 |
| [getParamCount()](#getParamCount--) | 获取参数的数量。 |
| [getParamText(int index)](#getParamText-int-) | 获取给定索引处参数的文字文本。 |
| [getParamValue(int index)](#getParamValue-int-) | 获取给定索引处参数的表示值对象。 |
| [getRow()](#getRow--) | 获取函数所在的单元格行索引。 |
| [getSheetName()](#getSheetName--) | 获取函数所在的工作表名称。 |
| [getStringValue()](#getStringValue--) | 获取函数所在的单元格 DisplayStringValue。 |
| [getValue()](#getValue--) | 获取函数所在的单元格值。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculatedValue(Object value)](#setCalculatedValue-java.lang.Object-) | 设置此函数的计算值。 |
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
### getCalculatedValue() {#getCalculatedValue--}
```
public Object getCalculatedValue()
```


获取此函数的计算值。

**Remarks**

用户应在其自定义计算引擎中为引擎支持的函数设置此属性，获取此属性时将返回已设置的值。在设置之前获取此属性将导致函数使用 Aspose.Cells 的默认计算引擎进行计算，并返回计算后的值。

**Returns:**
java.lang.Object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


获取函数所在的单元格列索引。

**Returns:**
int
### getFormula() {#getFormula--}
```
public String getFormula()
```


获取函数所在的单元格公式。

**Returns:**
java.lang.String
### getFunctionName() {#getFunctionName--}
```
public String getFunctionName()
```


获取要计算的函数名称。

**Returns:**
java.lang.String
### getParamCount() {#getParamCount--}
```
public int getParamCount()
```


获取参数的数量。

**Returns:**
int
### getParamText(int index) {#getParamText-int-}
```
public String getParamText(int index)
```


获取给定索引处参数的文字文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 参数的索引（从 0 开始）。 |

**Returns:**
java.lang.String - 参数的文字文本。
### getParamValue(int index) {#getParamValue-int-}
```
public Object getParamValue(int index)
```


获取给定索引处参数的表示值对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 参数的索引（从 0 开始）。 |

**Returns:**
java.lang.Object - 如果参数是普通值，则返回该普通值；如果参数是引用，则返回 ReferredArea 对象。
### getRow() {#getRow--}
```
public int getRow()
```


获取函数所在的单元格行索引。

**Returns:**
int
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


获取函数所在的工作表名称。

**Returns:**
java.lang.String
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


获取函数所在的单元格 DisplayStringValue。

**Returns:**
java.lang.String
### getValue() {#getValue--}
```
public Object getValue()
```


获取函数所在的单元格值。

**Returns:**
java.lang.Object
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




### setCalculatedValue(Object value) {#setCalculatedValue-java.lang.Object-}
```
public void setCalculatedValue(Object value)
```


设置此函数的计算值。

**Remarks**

用户应在其自定义计算引擎中为引擎支持的函数设置此属性，获取此属性时将返回已设置的值。在设置之前获取此属性将导致函数使用 Aspose.Cells 的默认计算引擎进行计算，并返回计算后的值。

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

