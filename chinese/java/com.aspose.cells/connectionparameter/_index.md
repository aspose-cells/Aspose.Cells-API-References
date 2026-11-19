---
title: "ConnectionParameter"
second_title: "Aspose.Cells for Java API 参考"
description: "指定外部数据连接中使用的任何参数的属性。参数适用于 ODBC 和 web 查询。"
type: docs
url: /zh/java/com.aspose.cells/connectionparameter/
---

**Inheritance:**
java.lang.Object
```
public class ConnectionParameter
```

指定外部数据连接中使用的任何参数的属性。参数适用于 ODBC 和 web 查询。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellReference()](#getCellReference--) | 单元格引用，指示查询参数应使用哪个单元格的值。 |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | 参数的名称。 |
| [getPrompt()](#getPrompt--) | 参数的提示字符串。 |
| [getRefreshOnChange()](#getRefreshOnChange--) | 标志，指示当提供参数值的单元格内容更改时查询是否应自动刷新。 |
| [getSqlType()](#getSqlType--) | 参数的 SQL 数据类型。 |
| [getType()](#getType--) | 使用的参数类型。 |
| [getValue()](#getValue--) | 用于查询参数的非整数数值、整数值、字符串值或布尔值。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCellReference(String value)](#setCellReference-java.lang.String-) | 单元格引用，指示查询参数应使用哪个单元格的值。 |
| [setName(String value)](#setName-java.lang.String-) | 参数的名称。 |
| [setPrompt(String value)](#setPrompt-java.lang.String-) | 参数的提示字符串。 |
| [setRefreshOnChange(boolean value)](#setRefreshOnChange-boolean-) | 标志，指示当提供参数值的单元格内容更改时查询是否应自动刷新。 |
| [setSqlType(int value)](#setSqlType-int-) | 参数的 SQL 数据类型。 |
| [setType(int value)](#setType-int-) | 使用的参数类型。 |
| [setValue(Object value)](#setValue-java.lang.Object-) | 用于查询参数的非整数数值、整数值、字符串值或布尔值。 |
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
### getCellReference() {#getCellReference--}
```
public String getCellReference()
```


单元格引用，指示查询参数应使用哪个单元格的值。仅在 parameterType 为 cell 时使用。

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getName() {#getName--}
```
public String getName()
```


参数的名称。

**Returns:**
java.lang.String
### getPrompt() {#getPrompt--}
```
public String getPrompt()
```


参数的提示字符串。显示给电子表格用户，并伴随输入 UI 收集参数值，以在刷新外部数据之前使用。仅在 parameterType = prompt 时使用。

**Returns:**
java.lang.String
### getRefreshOnChange() {#getRefreshOnChange--}
```
public boolean getRefreshOnChange()
```


标志，指示当提供参数值的单元格内容更改时查询是否应自动刷新。如果为 true，则每次更改时使用新的参数值刷新外部数据。如果为 false，则仅在用户请求或其他事件触发刷新时（例如打开工作簿）刷新外部数据。

**Returns:**
boolean
### getSqlType() {#getSqlType--}
```
public int getSqlType()
```


参数的 SQL 数据类型。仅对 ODBC 源有效。

参见 [SqlDataType](../../com.aspose.cells/sqldatatype)。

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


使用的参数类型。如果 parameterType = value，则使用布尔、双精度、整数或字符串中的值。在这种情况下，预计只能指定 \{boolean, double, integer, or string\} 中的一个。

参见 [ConnectionParameterType](../../com.aspose.cells/connectionparametertype)。

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


用于查询参数的非整数数值、整数值、字符串值或布尔值。仅在 parameterType 为 value 时使用。

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




### setCellReference(String value) {#setCellReference-java.lang.String-}
```
public void setCellReference(String value)
```


单元格引用，指示查询参数应使用哪个单元格的值。仅在 parameterType 为 cell 时使用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


参数的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setPrompt(String value) {#setPrompt-java.lang.String-}
```
public void setPrompt(String value)
```


参数的提示字符串。显示给电子表格用户，并伴随输入 UI 收集参数值，以在刷新外部数据之前使用。仅在 parameterType = prompt 时使用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setRefreshOnChange(boolean value) {#setRefreshOnChange-boolean-}
```
public void setRefreshOnChange(boolean value)
```


标志，指示当提供参数值的单元格内容更改时查询是否应自动刷新。如果为 true，则每次更改时使用新的参数值刷新外部数据。如果为 false，则仅在用户请求或其他事件触发刷新时（例如打开工作簿）刷新外部数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSqlType(int value) {#setSqlType-int-}
```
public void setSqlType(int value)
```


参数的 SQL 数据类型。仅对 ODBC 源有效。

参见 [SqlDataType](../../com.aspose.cells/sqldatatype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


使用的参数类型。如果 parameterType = value，则使用布尔、双精度、整数或字符串中的值。在这种情况下，预计只能指定 \{boolean, double, integer, or string\} 中的一个。

参见 [ConnectionParameterType](../../com.aspose.cells/connectionparametertype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


用于查询参数的非整数数值、整数值、字符串值或布尔值。仅在 parameterType 为 value 时使用。

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

