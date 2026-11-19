---
title: "CellValueFormatStrategy"
second_title: "Aspose.Cells for Java API 参考"
description: "指定如何为单元格的值应用样式。"
type: docs
url: /zh/java/com.aspose.cells/cellvalueformatstrategy/
---

**Inheritance:**
java.lang.Object
```
public final class CellValueFormatStrategy
```

指定如何为单元格的值应用样式。
## 字段

| 字段 | 描述 |
| --- | --- |
| [CELL_STYLE](#CELL-STYLE) | 仅使用单元格的原始样式进行格式化。 |
| [DISPLAY_STRING](#DISPLAY-STRING) | 获取在 MS Excel 中显示的字符串。 |
| [DISPLAY_STYLE](#DISPLAY-STYLE) | 使用单元格的显示样式进行格式化。 |
| [NONE](#NONE) | 未格式化。 |
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
### CELL_STYLE {#CELL-STYLE}
```
public static final int CELL_STYLE
```


仅使用单元格的原始样式进行格式化。

### DISPLAY_STRING {#DISPLAY-STRING}
```
public static final int DISPLAY_STRING
```


获取在 MS Excel 中显示的字符串。与 [DISPLAY\_STYLE](../../com.aspose.cells/cellvalueformatstrategy\#DISPLAY-STYLE) 的主要区别在于此选项还会考虑列宽的影响。如果列宽过小而无法完整显示格式化后的字符串，可能会显示 "\\#"，这与 MS Excel 的行为相同。

### DISPLAY_STYLE {#DISPLAY-STYLE}
```
public static final int DISPLAY_STYLE
```


使用单元格的显示样式进行格式化。

### NONE {#NONE}
```
public static final int NONE
```


未格式化。

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

