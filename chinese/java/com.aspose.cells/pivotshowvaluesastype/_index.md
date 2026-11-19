---
title: "PivotShowValuesAsType"
second_title: "Aspose.Cells for Java API 参考"
description: "表示透视字段值的“显示值为”功能的计算类型。"
type: docs
url: /zh/java/com.aspose.cells/pivotshowvaluesastype/
---

**Inheritance:**
java.lang.Object
```
public final class PivotShowValuesAsType
```

表示数据透视字段值的 "Show Values As" 功能的计算类型。
## 字段

| 字段 | 描述 |
| --- | --- |
| [DIFFERENCE_FROM](#DIFFERENCE-FROM) | 将值显示为与指定基项的差异。 |
| [INDEX](#INDEX) | 索引计算：(Cell Value \\u8133 Grand Total of Grand Totals) / (Row Grand Total \\u8133 Column Grand Total)。 |
| [NORMAL](#NORMAL) | 表示原始值，不进行自定义计算。 |
| [PERCENTAGE_DIFFERENCE_FROM](#PERCENTAGE-DIFFERENCE-FROM) | 将值显示为相对于指定基项的百分比差异。 |
| [PERCENTAGE_OF](#PERCENTAGE-OF) | 将值显示为指定基项的百分比。 |
| [PERCENTAGE_OF_COLUMN](#PERCENTAGE-OF-COLUMN) | 将值显示为列总计的百分比。 |
| [PERCENTAGE_OF_PARENT_COLUMN_TOTAL](#PERCENTAGE-OF-PARENT-COLUMN-TOTAL) | 将值显示为其父列项总计的百分比。 |
| [PERCENTAGE_OF_PARENT_ROW_TOTAL](#PERCENTAGE-OF-PARENT-ROW-TOTAL) | 将值显示为其父行项总计的百分比。 |
| [PERCENTAGE_OF_PARENT_TOTAL](#PERCENTAGE-OF-PARENT-TOTAL) | 将值显示为指定基字段中其父项总计的百分比。 |
| [PERCENTAGE_OF_ROW](#PERCENTAGE-OF-ROW) | 将值显示为行总计的百分比。 |
| [PERCENTAGE_OF_RUNNING_TOTAL_IN](#PERCENTAGE-OF-RUNNING-TOTAL-IN) | 将值显示为沿指定基字段的百分比累计总计。 |
| [PERCENTAGE_OF_TOTAL](#PERCENTAGE-OF-TOTAL) | 将值显示为总体总计的百分比。 |
| [RANK_LARGEST_TO_SMALLEST](#RANK-LARGEST-TO-SMALLEST) | 在指定基字段内对值进行从大到小的排名。 |
| [RANK_SMALLEST_TO_LARGEST](#RANK-SMALLEST-TO-LARGEST) | 在指定基字段内对值进行从小到大的排名。 |
| [RUNNING_TOTAL_IN](#RUNNING-TOTAL-IN) | 将值显示为沿指定基字段的累计总计。 |
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
### DIFFERENCE_FROM {#DIFFERENCE-FROM}
```
public static final int DIFFERENCE_FROM
```


将值显示为与指定基项的差异。

**Remarks**

基字段和基项是必需的。

### INDEX {#INDEX}
```
public static final int INDEX
```


索引计算：(Cell Value \\u8133 Grand Total of Grand Totals) / (Row Grand Total \\u8133 Column Grand Total)。

### NORMAL {#NORMAL}
```
public static final int NORMAL
```


表示原始值，不进行自定义计算。

### PERCENTAGE_DIFFERENCE_FROM {#PERCENTAGE-DIFFERENCE-FROM}
```
public static final int PERCENTAGE_DIFFERENCE_FROM
```


将值显示为相对于指定基项的百分比差异。

**Remarks**

基字段和基项是必需的。

### PERCENTAGE_OF {#PERCENTAGE-OF}
```
public static final int PERCENTAGE_OF
```


将值显示为指定基项的百分比。

**Remarks**

基字段和基项是必需的。

### PERCENTAGE_OF_COLUMN {#PERCENTAGE-OF-COLUMN}
```
public static final int PERCENTAGE_OF_COLUMN
```


将值显示为列总计的百分比。

### PERCENTAGE_OF_PARENT_COLUMN_TOTAL {#PERCENTAGE-OF-PARENT-COLUMN-TOTAL}
```
public static final int PERCENTAGE_OF_PARENT_COLUMN_TOTAL
```


将值显示为其父列项总计的百分比。

### PERCENTAGE_OF_PARENT_ROW_TOTAL {#PERCENTAGE-OF-PARENT-ROW-TOTAL}
```
public static final int PERCENTAGE_OF_PARENT_ROW_TOTAL
```


将值显示为其父行项总计的百分比。

### PERCENTAGE_OF_PARENT_TOTAL {#PERCENTAGE-OF-PARENT-TOTAL}
```
public static final int PERCENTAGE_OF_PARENT_TOTAL
```


将值显示为指定基字段中其父项总计的百分比。

**Remarks**

基字段是必需的。

### PERCENTAGE_OF_ROW {#PERCENTAGE-OF-ROW}
```
public static final int PERCENTAGE_OF_ROW
```


将值显示为行总计的百分比。

### PERCENTAGE_OF_RUNNING_TOTAL_IN {#PERCENTAGE-OF-RUNNING-TOTAL-IN}
```
public static final int PERCENTAGE_OF_RUNNING_TOTAL_IN
```


将值显示为沿指定基字段的百分比累计总计。

**Remarks**

基字段是必需的。

### PERCENTAGE_OF_TOTAL {#PERCENTAGE-OF-TOTAL}
```
public static final int PERCENTAGE_OF_TOTAL
```


将值显示为总体总计的百分比。

### RANK_LARGEST_TO_SMALLEST {#RANK-LARGEST-TO-SMALLEST}
```
public static final int RANK_LARGEST_TO_SMALLEST
```


在指定基字段内对值进行从大到小的排名。

**Remarks**

基字段是必需的。

### RANK_SMALLEST_TO_LARGEST {#RANK-SMALLEST-TO-LARGEST}
```
public static final int RANK_SMALLEST_TO_LARGEST
```


在指定基字段内对值进行从小到大的排名。

**Remarks**

基字段是必需的。

### RUNNING_TOTAL_IN {#RUNNING-TOTAL-IN}
```
public static final int RUNNING_TOTAL_IN
```


将值显示为沿指定基字段的累计总计。

**Remarks**

基字段是必需的。

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

