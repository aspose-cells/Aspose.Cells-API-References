---
title: "CellValue"
second_title: "Aspose.Cells for Java API 参考"
description: "表示单元格的值及其对应类型。"
type: docs
url: /zh/java/com.aspose.cells/cellvalue/
---

**Inheritance:**
java.lang.Object
```
public class CellValue
```

表示单元格的值及其对应类型。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [CellValue()](#CellValue--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | 获取单元格值的类型。 |
| [getValue()](#getValue--) | 获取单元格值。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setType(int value)](#setType-int-) | 设置单元格值的类型。 |
| [setValue(Object value)](#setValue-java.lang.Object-) | 设置单元格值。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CellValue() {#CellValue--}
```
public CellValue()
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
### getType() {#getType--}
```
public int getType()
```


获取单元格值的类型。

参见 [CellValueType](../../com.aspose.cells/cellvaluetype)。

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


获取单元格值。

**Remarks**

该值必须是对应于 [getType()](../../com.aspose.cells/cellvalue\#getType--) 的正确对象类型：

| 类型 | 值 |
| --------------------------------------------------------------------------------- | ----------------------------------------------- |
| [CellValueType.IS\_NULL](../../com.aspose.cells/cellvaluetype\#IS-NULL) | null，其他任何对象将被忽略 |
| [CellValueType.IS\_NUMERIC](../../com.aspose.cells/cellvaluetype\#IS-NUMERIC) | double |
| [CellValueType.IS\_DATE\_TIME](../../com.aspose.cells/cellvaluetype\#IS-DATE-TIME) | DateTime |
| [CellValueType.IS\_STRING](../../com.aspose.cells/cellvaluetype\#IS-STRING) | string |
| [CellValueType.IS\_BOOL](../../com.aspose.cells/cellvaluetype\#IS-BOOL) | bool |
| [CellValueType.IS\_ERROR](../../com.aspose.cells/cellvaluetype\#IS-ERROR) | 错误字符串，例如 \"\\#VALUE!\", \"\\#NAME?\", ... |

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




### setType(int value) {#setType-int-}
```
public void setType(int value)
```


设置单元格值的类型。

参见 [CellValueType](../../com.aspose.cells/cellvaluetype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


设置单元格值。

**Remarks**

该值必须是对应于 [getType()](../../com.aspose.cells/cellvalue\#getType--) 的正确对象类型：

| 类型 | 值 |
| --------------------------------------------------------------------------------- | ----------------------------------------------- |
| [CellValueType.IS\_NULL](../../com.aspose.cells/cellvaluetype\#IS-NULL) | null，其他任何对象将被忽略 |
| [CellValueType.IS\_NUMERIC](../../com.aspose.cells/cellvaluetype\#IS-NUMERIC) | double |
| [CellValueType.IS\_DATE\_TIME](../../com.aspose.cells/cellvaluetype\#IS-DATE-TIME) | DateTime |
| [CellValueType.IS\_STRING](../../com.aspose.cells/cellvaluetype\#IS-STRING) | string |
| [CellValueType.IS\_BOOL](../../com.aspose.cells/cellvaluetype\#IS-BOOL) | bool |
| [CellValueType.IS\_ERROR](../../com.aspose.cells/cellvaluetype\#IS-ERROR) | 错误字符串，例如 \"\\#VALUE!\", \"\\#NAME?\", ... |

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

