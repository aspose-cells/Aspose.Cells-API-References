---
title: AccessCacheOptions
second_title: Aspose.Cells for Java API Reference
description: Caching options for data access.
type: docs
url: /java/com.aspose.cells/accesscacheoptions/
---

**Inheritance:**
java.lang.Object
```
public final class AccessCacheOptions
```

Caching options for data access. Multiple options can be combined using the "\|" operator.

**Remarks**

For some features, accessing large dataset requires a lot of repeated and complicated operations such as search, calculation, ...etc and those operations will take a lot of extra time. For common situations, all dependent data remains unchanged during the access, so some caches can be built and used to improve the access performance. For this purpose, we provide this API so that user can specify which kind of data access needs to be optimized by possible caching mechanism.

Please note, for different options, different data set may be required to be "read-only". And performance of accessing data depends on many aspects, the use of caching mechanism does not guarantee that performance will be improved. For some situations, such as the dataset to be accessed is small, using cache may cause even more time because caching itself also needs certain extra time.
## Fields

| Field | Description |
| --- | --- |
| [ALL](#ALL) | Apply all possible optimizations for all kinds of data access in the workbook. |
| [CALCULATE_FORMULA](#CALCULATE-FORMULA) | Apply possible optimization for calculating formulas. |
| [CELLS_DATA](#CELLS-DATA) | Apply possible optimization for getting cells' values. |
| [CELL_DISPLAY](#CELL-DISPLAY) | Apply possible optimization for getting display-related results of cells([Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), [Cell.getStyle()](../../com.aspose.cells/cell\#getStyle--), [Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--), etc.). |
| [CONDITIONAL_FORMATTING](#CONDITIONAL-FORMATTING) | Apply possible optimization for getting formatting result of conditional formattings. |
| [GET_FORMULA](#GET-FORMULA) | Apply possible optimization for getting formulas. |
| [NONE](#NONE) | No cache for any data access. |
| [POSITION_AND_SIZE](#POSITION-AND-SIZE) | Apply possible optimization for getting object(such as Shape)'s position and size. |
| [SET_FORMULA](#SET-FORMULA) | Apply possible optimization for setting formulas. |
| [VALIDATION](#VALIDATION) | Apply possible optimization for getting validation result. |
## Methods

| Method | Description |
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


Apply all possible optimizations for all kinds of data access in the workbook. All settings and data should not be changed during the optimized access.

### CALCULATE_FORMULA {#CALCULATE-FORMULA}
```
public static final int CALCULATE_FORMULA
```


Apply possible optimization for calculating formulas. Cells data should not be changed during the optimized access, none new objects(Cell, Row, etc.) should be created either(such as by [Cells.get(int,int)](../../com.aspose.cells/cells\#get-int-int-)).

### CELLS_DATA {#CELLS-DATA}
```
public static final int CELLS_DATA
```


Apply possible optimization for getting cells' values. Cells data(data and settings of Cell, Row) should not be changed during the optimized access, no new Cell/Row objects should be created either(such as by [Cells.get(int,int)](../../com.aspose.cells/cells\#get-int-int-)).

### CELL_DISPLAY {#CELL-DISPLAY}
```
public static final int CELL_DISPLAY
```


Apply possible optimization for getting display-related results of cells([Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), [Cell.getStyle()](../../com.aspose.cells/cell\#getStyle--), [Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--), etc.). Cells data and style-related objects(Cell/Row/Column styles, column width, etc.) should not be changed during the optimized access.

### CONDITIONAL_FORMATTING {#CONDITIONAL-FORMATTING}
```
public static final int CONDITIONAL_FORMATTING
```


Apply possible optimization for getting formatting result of conditional formattings. All data and settings which may affect the result of conditional formattings(settings of conditional formattings, dependent cell values, etc.) should not be changed during the optimized access.

### GET_FORMULA {#GET-FORMULA}
```
public static final int GET_FORMULA
```


Apply possible optimization for getting formulas. All data and settings which may affect the formula expression(Worksheet's name, Name's text, table's column, etc.) should not be changed during the optimized access.

### NONE {#NONE}
```
public static final int NONE
```


No cache for any data access.

### POSITION_AND_SIZE {#POSITION-AND-SIZE}
```
public static final int POSITION_AND_SIZE
```


Apply possible optimization for getting object(such as Shape)'s position and size. Row height and column width settings should not be changed during the optimized access.

### SET_FORMULA {#SET-FORMULA}
```
public static final int SET_FORMULA
```


Apply possible optimization for setting formulas. All data and settings which may affect the formula expression(Worksheet's name, Name's text, table's column, etc.) should not be changed during the optimized access.

### VALIDATION {#VALIDATION}
```
public static final int VALIDATION
```


Apply possible optimization for getting validation result. All data and settings which may affect the result of validation(settings of the validation, dependent cell values, etc.) should not be changed during the optimized access.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

