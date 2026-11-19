---
title: "AccessCacheOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "数据访问的缓存选项。"
type: docs
url: /zh/java/com.aspose.cells/accesscacheoptions/
---

**Inheritance:**
java.lang.Object
```
public final class AccessCacheOptions
```

数据访问的缓存选项。多个选项可以使用 "\|" 运算符组合。

**Remarks**

对于某些功能，访问大型数据集需要大量重复且复杂的操作，例如搜索、计算等，这些操作会耗费额外时间。对于常见情况，所有依赖的数据在访问期间保持不变，因此可以构建并使用缓存来提升访问性能。为此，我们提供此 API，允许用户指定需要通过可能的缓存机制进行优化的数据访问类型。

请注意，对于不同的选项，可能需要将不同的数据集设为 “只读”。数据访问性能受多方面影响，使用缓存机制并不能保证性能提升。在某些情况下，例如要访问的数据集很小，使用缓存可能会耗费更多时间，因为缓存本身也需要一定的额外开销。
## 字段

| 字段 | 描述 |
| --- | --- |
| [ALL](#ALL) | 对工作簿中的所有数据访问类型应用所有可能的优化。 |
| [CALCULATE_FORMULA](#CALCULATE-FORMULA) | 对公式计算应用可能的优化。 |
| [CELLS_DATA](#CELLS-DATA) | 对获取单元格值应用可能的优化。 |
| [CELL_DISPLAY](#CELL-DISPLAY) | 对获取单元格的显示相关结果应用可能的优化（[Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--)，[Cell.getStyle()](../../com.aspose.cells/cell\#getStyle--)，[Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--)，等）。 |
| [CONDITIONAL_FORMATTING](#CONDITIONAL-FORMATTING) | 对获取条件格式的格式化结果应用可能的优化。 |
| [GET_FORMULA](#GET-FORMULA) | 对获取公式应用可能的优化。 |
| [NONE](#NONE) | 任何数据访问均不使用缓存。 |
| [POSITION_AND_SIZE](#POSITION-AND-SIZE) | 对获取对象（如 Shape）的位置信息和大小应用可能的优化。 |
| [SET_FORMULA](#SET-FORMULA) | 对设置公式应用可能的优化。 |
| [VALIDATION](#VALIDATION) | 对获取验证结果应用可能的优化。 |
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


对工作簿中的所有数据访问类型应用所有可能的优化。在优化访问期间，所有设置和数据均不得更改。

### CALCULATE_FORMULA {#CALCULATE-FORMULA}
```
public static final int CALCULATE_FORMULA
```


对公式计算应用可能的优化。优化访问期间不应更改单元格数据，也不应创建任何新对象（Cell、Row 等），例如通过 [Cells.get(int,int)](../../com.aspose.cells/cells\#get-int-int-)。

### CELLS_DATA {#CELLS-DATA}
```
public static final int CELLS_DATA
```


对获取单元格值应用可能的优化。优化访问期间不应更改单元格数据（包括 Cell、Row 的数据和设置），也不应创建任何新 Cell/Row 对象，例如通过 [Cells.get(int,int)](../../com.aspose.cells/cells\#get-int-int-)。

### CELL_DISPLAY {#CELL-DISPLAY}
```
public static final int CELL_DISPLAY
```


对获取单元格的显示相关结果应用可能的优化（[Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--)，[Cell.getStyle()](../../com.aspose.cells/cell\#getStyle--)，[Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--)，等）。在优化访问期间，不应更改单元格数据以及样式相关对象（Cell/Row/Column 样式、列宽等）。

### CONDITIONAL_FORMATTING {#CONDITIONAL-FORMATTING}
```
public static final int CONDITIONAL_FORMATTING
```


对获取条件格式的格式化结果应用可能的优化。在优化访问期间，所有可能影响条件格式结果的数据和设置（条件格式的设置、依赖的单元格值等）均不得更改。

### GET_FORMULA {#GET-FORMULA}
```
public static final int GET_FORMULA
```


对获取公式应用可能的优化。在优化访问期间，所有可能影响公式表达式的数据和设置（工作表名称、名称文本、表格列等）均不得更改。

### NONE {#NONE}
```
public static final int NONE
```


任何数据访问均不使用缓存。

### POSITION_AND_SIZE {#POSITION-AND-SIZE}
```
public static final int POSITION_AND_SIZE
```


对获取对象（如 Shape）的位置信息和大小应用可能的优化。在优化访问期间，行高和列宽设置不得更改。

### SET_FORMULA {#SET-FORMULA}
```
public static final int SET_FORMULA
```


对设置公式应用可能的优化。在优化访问期间，所有可能影响公式表达式的数据和设置（工作表名称、名称文本、表格列等）均不得更改。

### VALIDATION {#VALIDATION}
```
public static final int VALIDATION
```


对获取验证结果应用可能的优化。在优化访问期间，所有可能影响验证结果的数据和设置（验证的设置、依赖的单元格值等）均不得更改。

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

