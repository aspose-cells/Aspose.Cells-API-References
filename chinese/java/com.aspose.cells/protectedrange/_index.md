---
title: "ProtectedRange"
second_title: "Aspose.Cells for Java API 参考"
description: "在工作表保护开启时，允许编辑的指定范围。"
type: docs
url: /zh/java/com.aspose.cells/protectedrange/
---

**Inheritance:**
java.lang.Object
```
public class ProtectedRange
```

在工作表保护开启时，允许编辑的指定范围。
## 方法

| 方法 | 描述 |
| --- | --- |
| [addArea(int startRow, int startColumn, int endRow, int endColumn)](#addArea-int-int-int-int-) | 向此对象添加引用区域 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAreas()](#getAreas--) | 获取所有引用的区域。 |
| [getCellArea()](#getCellArea--) | 获取表示要受保护的单元格区域的 [getCellArea()](../../com.aspose.cells/protectedrange\#getCellArea--) 对象。 |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | 获取范围标题。 |
| [getPassword()](#getPassword--) | 表示用于保护范围的密码。 |
| [getSecurityDescriptor()](#getSecurityDescriptor--) | 安全描述符定义了可以在不提供密码的情况下编辑此范围的用户账户。 |
| [hashCode()](#hashCode--) |  |
| [isProtectedWithPassword()](#isProtectedWithPassword--) | 指示工作表是否已使用密码受保护。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setName(String value)](#setName-java.lang.String-) | 获取范围标题。 |
| [setPassword(String value)](#setPassword-java.lang.String-) | 表示用于保护范围的密码。 |
| [setSecurityDescriptor(String value)](#setSecurityDescriptor-java.lang.String-) | 安全描述符定义了可以在不提供密码的情况下编辑此范围的用户账户。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addArea(int startRow, int startColumn, int endRow, int endColumn) {#addArea-int-int-int-int-}
```
public void addArea(int startRow, int startColumn, int endRow, int endColumn)
```


向此对象添加引用区域

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 起始行。 |
| startColumn | int | 起始列。 |
| endRow | int | 结束行。 |
| endColumn | int | 结束列。 |

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
### getAreas() {#getAreas--}
```
public CellArea[] getAreas()
```


获取所有引用的区域。

**Returns:**
com.aspose.cells.CellArea[] - 返回所有引用的区域。
### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


获取表示要受保护的单元格区域的 [getCellArea()](../../com.aspose.cells/protectedrange\#getCellArea--) 对象。

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
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


获取 Range 标题。此用作描述符，而不是命名范围定义。

**Returns:**
java.lang.String
### getPassword() {#getPassword--}
```
public String getPassword()
```


表示用于保护范围的密码。

**Returns:**
java.lang.String
### getSecurityDescriptor() {#getSecurityDescriptor--}
```
public String getSecurityDescriptor()
```


安全描述符定义了可以在不提供密码的情况下编辑此范围的用户账户。

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isProtectedWithPassword() {#isProtectedWithPassword--}
```
public boolean isProtectedWithPassword()
```


指示工作表是否已使用密码受保护。

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




### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


获取 Range 标题。此用作描述符，而不是命名范围定义。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


表示用于保护范围的密码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setSecurityDescriptor(String value) {#setSecurityDescriptor-java.lang.String-}
```
public void setSecurityDescriptor(String value)
```


安全描述符定义了可以在不提供密码的情况下编辑此范围的用户账户。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

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

