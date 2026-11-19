---
title: "LoadDataFilterOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "表示从模板加载工作簿时用于过滤数据的选项。"
type: docs
url: /zh/java/com.aspose.cells/loaddatafilteroptions/
---

**Inheritance:**
java.lang.Object
```
public final class LoadDataFilterOptions
```

表示从模板加载工作簿时用于过滤数据的选项。
## 字段

| 字段 | 描述 |
| --- | --- |
| [ALL](#ALL) | 加载全部 |
| [BOOK_SETTINGS](#BOOK-SETTINGS) | 加载工作簿的设置 |
| [CELL_BLANK](#CELL-BLANK) | 加载值为空的单元格 |
| [CELL_BOOL](#CELL-BOOL) | 加载值为布尔型的单元格 |
| [CELL_DATA](#CELL-DATA) | 加载单元格数据，包括值、公式和格式 |
| [CELL_ERROR](#CELL-ERROR) | 加载值为错误的单元格 |
| [CELL_NUMERIC](#CELL-NUMERIC) | 加载值为数值（包括日期时间）的单元格 |
| [CELL_STRING](#CELL-STRING) | 加载值为字符串的单元格 |
| [CELL_VALUE](#CELL-VALUE) | 仅加载单元格值（所有值类型） |
| [CHART](#CHART) | 加载图表 |
| [CONDITIONAL_FORMATTING](#CONDITIONAL-FORMATTING) | 加载条件格式 |
| [DATA_VALIDATION](#DATA-VALIDATION) | 加载数据验证 |
| [DEFINED_NAMES](#DEFINED-NAMES) | 加载已定义的名称对象 |
| [DOCUMENT_PROPERTIES](#DOCUMENT-PROPERTIES) | 加载文档属性 |
| [DRAWING](#DRAWING) | 绘图对象（包括图表、图片、OleObject 以及所有其他绘图对象） |
| [FORMULA](#FORMULA) | 加载单元格公式。 |
| [HYPERLINKS](#HYPERLINKS) | 加载超链接 |
| [MERGED_AREA](#MERGED-AREA) | 加载合并单元格 |
| [NONE](#NONE) | 不加载工作表数据 |
| [OLE_OBJECT](#OLE-OBJECT) | 加载 OleObject |
| [PICTURE](#PICTURE) | 加载图片 |
| [PIVOT_TABLE](#PIVOT-TABLE) | 加载数据透视表 |
| [REVISION](#REVISION) | 加载修订日志 |
| [SETTINGS](#SETTINGS) | 加载工作簿和工作表的设置 |
| [SHAPE](#SHAPE) | 加载形状 |
| [SHEET_DATA](#SHEET-DATA) | 加载工作表的所有数据，例如单元格数据、设置、对象等 |
| [SHEET_SETTINGS](#SHEET-SETTINGS) | 加载工作表的设置 |
| [STRUCTURE](#STRUCTURE) | 加载工作簿结构 |
| [STYLE](#STYLE) | 加载单元格格式的样式 |
| [TABLE](#TABLE) | 加载表格 |
| [VBA](#VBA) | 加载 VBA 项目 |
| [XML_MAP](#XML-MAP) | 加载 XmlMap |
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
### ALL {#ALL}
```
public static final int ALL
```


加载全部

### BOOK_SETTINGS {#BOOK-SETTINGS}
```
public static final int BOOK_SETTINGS
```


加载工作簿的设置

### CELL_BLANK {#CELL-BLANK}
```
public static final int CELL_BLANK
```


加载值为空的单元格

### CELL_BOOL {#CELL-BOOL}
```
public static final int CELL_BOOL
```


加载值为布尔型的单元格

### CELL_DATA {#CELL-DATA}
```
public static final int CELL_DATA
```


加载单元格数据，包括值、公式和格式

### CELL_ERROR {#CELL-ERROR}
```
public static final int CELL_ERROR
```


加载值为错误的单元格

### CELL_NUMERIC {#CELL-NUMERIC}
```
public static final int CELL_NUMERIC
```


加载值为数值（包括日期时间）的单元格

### CELL_STRING {#CELL-STRING}
```
public static final int CELL_STRING
```


加载值为字符串的单元格

### CELL_VALUE {#CELL-VALUE}
```
public static final int CELL_VALUE
```


仅加载单元格值（所有值类型）

### CHART {#CHART}
```
public static final int CHART
```


加载图表

### CONDITIONAL_FORMATTING {#CONDITIONAL-FORMATTING}
```
public static final int CONDITIONAL_FORMATTING
```


加载条件格式

### DATA_VALIDATION {#DATA-VALIDATION}
```
public static final int DATA_VALIDATION
```


加载数据验证

### DEFINED_NAMES {#DEFINED-NAMES}
```
public static final int DEFINED_NAMES
```


加载已定义的名称对象

### DOCUMENT_PROPERTIES {#DOCUMENT-PROPERTIES}
```
public static final int DOCUMENT_PROPERTIES
```


加载文档属性

### DRAWING {#DRAWING}
```
public static final int DRAWING
```


绘图对象（包括图表、图片、OleObject 以及所有其他绘图对象）

### FORMULA {#FORMULA}
```
public static final int FORMULA
```


加载单元格公式。

**Remarks**

通常在加载公式时也需要加载已定义的名称对象（DefinedNames），因为它们可能被公式引用。因此，Formula 或 CellData 选项应与 DefinedNames 选项一起使用（Formula\|DefinedNames 或 CellData\|DefinedNames），以适用于大多数场景。

### HYPERLINKS {#HYPERLINKS}
```
public static final int HYPERLINKS
```


加载超链接

### MERGED_AREA {#MERGED-AREA}
```
public static final int MERGED_AREA
```


加载合并单元格

### NONE {#NONE}
```
public static final int NONE
```


不加载工作表数据

**Remarks**

注意：此成员已过时，请改用 Structure。此属性将在自 2017 年 12 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### OLE_OBJECT {#OLE-OBJECT}
```
public static final int OLE_OBJECT
```


加载 OleObject

### PICTURE {#PICTURE}
```
public static final int PICTURE
```


加载图片

### PIVOT_TABLE {#PIVOT-TABLE}
```
public static final int PIVOT_TABLE
```


加载数据透视表

### REVISION {#REVISION}
```
public static final int REVISION
```


加载修订日志

### SETTINGS {#SETTINGS}
```
public static final int SETTINGS
```


加载工作簿和工作表的设置

### SHAPE {#SHAPE}
```
public static final int SHAPE
```


加载形状

**Remarks**

注意：此成员已过时，请改用 Drawing。此属性将在自 2019 年 11 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### SHEET_DATA {#SHEET-DATA}
```
public static final int SHEET_DATA
```


加载工作表的所有数据，例如单元格数据、设置、对象等

### SHEET_SETTINGS {#SHEET-SETTINGS}
```
public static final int SHEET_SETTINGS
```


加载工作表的设置

### STRUCTURE {#STRUCTURE}
```
public static final int STRUCTURE
```


加载工作簿结构

### STYLE {#STYLE}
```
public static final int STYLE
```


加载单元格格式的样式

### TABLE {#TABLE}
```
public static final int TABLE
```


加载表格

### VBA {#VBA}
```
public static final int VBA
```


加载 VBA 项目

### XML_MAP {#XML-MAP}
```
public static final int XML_MAP
```


加载 XmlMap

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

