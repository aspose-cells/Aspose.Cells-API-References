---
title: "FormatConditionType"
second_title: "Aspose.Cells for Java API 参考"
description: "条件格式规则类型。"
type: docs
url: /zh/java/com.aspose.cells/formatconditiontype/
---

**Inheritance:**
java.lang.Object
```
public final class FormatConditionType
```

条件格式规则类型。
## 字段

| 字段 | 描述 |
| --- | --- |
| [ABOVE_AVERAGE](#ABOVE-AVERAGE) | 此条件格式规则突出显示范围内所有值的平均值以上或以下的单元格。 |
| [BEGINS_WITH](#BEGINS-WITH) | 此条件格式规则突出显示范围内以给定文本开头的单元格。 |
| [CELL_VALUE](#CELL-VALUE) | 此条件格式规则使用运算符将单元格值与公式计算结果进行比较。 |
| [COLOR_SCALE](#COLOR-SCALE) | 此条件格式规则在单元格上创建渐变颜色刻度。 |
| [CONTAINS_BLANKS](#CONTAINS-BLANKS) | 此条件格式规则突出显示完全为空的单元格。 |
| [CONTAINS_ERRORS](#CONTAINS-ERRORS) | 此条件格式规则突出显示包含公式错误的单元格。 |
| [CONTAINS_TEXT](#CONTAINS-TEXT) | 此条件格式规则突出显示包含给定文本的单元格。 |
| [DATA_BAR](#DATA-BAR) | 此条件格式规则在单元格范围内显示渐变数据条。 |
| [DUPLICATE_VALUES](#DUPLICATE-VALUES) | 此条件格式规则突出显示重复的值。 |
| [ENDS_WITH](#ENDS-WITH) | 此条件格式规则突出显示以给定文本结尾的单元格。 |
| [EXPRESSION](#EXPRESSION) | 此条件格式规则包含一个用于评估的公式。 |
| [ICON_SET](#ICON-SET) | 此条件格式规则根据单元格的值为其应用图标。 |
| [NOT_CONTAINS_BLANKS](#NOT-CONTAINS-BLANKS) | 此条件格式规则突出显示非空的单元格。 |
| [NOT_CONTAINS_ERRORS](#NOT-CONTAINS-ERRORS) | 此条件格式规则突出显示没有公式错误的单元格。 |
| [NOT_CONTAINS_TEXT](#NOT-CONTAINS-TEXT) | 此条件格式规则突出显示不包含给定文本的单元格。 |
| [TIME_PERIOD](#TIME-PERIOD) | 此条件格式规则突出显示在指定时间段内包含日期的单元格。 |
| [TOP_10](#TOP-10) | 此条件格式规则突出显示其值位于指定的前 N 或后 N 区间的单元格。 |
| [UNIQUE_VALUES](#UNIQUE-VALUES) | 此条件格式规则突出显示范围内唯一的值。 |
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
### ABOVE_AVERAGE {#ABOVE-AVERAGE}
```
public static final int ABOVE_AVERAGE
```


此条件格式规则突出显示范围内所有值的平均值以上或以下的单元格。

### BEGINS_WITH {#BEGINS-WITH}
```
public static final int BEGINS_WITH
```


此条件格式规则突出显示范围内以给定文本开头的单元格。等同于使用 LEFT() 工作表函数并比较值。

### CELL_VALUE {#CELL-VALUE}
```
public static final int CELL_VALUE
```


此条件格式规则使用运算符将单元格值与公式计算结果进行比较。

### COLOR_SCALE {#COLOR-SCALE}
```
public static final int COLOR_SCALE
```


此条件格式规则在单元格上创建渐变颜色刻度。

### CONTAINS_BLANKS {#CONTAINS-BLANKS}
```
public static final int CONTAINS_BLANKS
```


此条件格式规则突出显示完全为空的单元格。等同于使用 LEN(TRIM())。这意味着如果单元格仅包含 TRIM() 会删除的字符，则视为空白。空单元格也视为空白。

### CONTAINS_ERRORS {#CONTAINS-ERRORS}
```
public static final int CONTAINS_ERRORS
```


此条件格式规则突出显示包含公式错误的单元格。等同于使用 ISERROR() 工作表函数来判断是否存在公式错误。

### CONTAINS_TEXT {#CONTAINS-TEXT}
```
public static final int CONTAINS_TEXT
```


此条件格式规则突出显示包含给定文本的单元格。等同于使用 SEARCH() 工作表函数来判断单元格是否包含该文本。

### DATA_BAR {#DATA-BAR}
```
public static final int DATA_BAR
```


此条件格式规则在单元格范围内显示渐变数据条。

### DUPLICATE_VALUES {#DUPLICATE-VALUES}
```
public static final int DUPLICATE_VALUES
```


此条件格式规则突出显示重复的值。

### ENDS_WITH {#ENDS-WITH}
```
public static final int ENDS_WITH
```


此条件格式规则突出显示以给定文本结尾的单元格。等同于使用 RIGHT() 工作表函数并比较值。

### EXPRESSION {#EXPRESSION}
```
public static final int EXPRESSION
```


此条件格式规则包含一个需要评估的公式。当公式结果为真时，单元格将被突出显示。

### ICON_SET {#ICON-SET}
```
public static final int ICON_SET
```


此条件格式规则根据单元格的值为其应用图标。

### NOT_CONTAINS_BLANKS {#NOT-CONTAINS-BLANKS}
```
public static final int NOT_CONTAINS_BLANKS
```


此条件格式规则突出显示非空单元格。相当于使用 LEN(TRIM())。这意味着如果单元格仅包含 TRIM() 会删除的字符，则视为空白。空单元格也视为空白。

### NOT_CONTAINS_ERRORS {#NOT-CONTAINS-ERRORS}
```
public static final int NOT_CONTAINS_ERRORS
```


此条件格式规则突出显示没有公式错误的单元格。相当于使用 ISERROR() 工作表函数来判断是否存在公式错误。

### NOT_CONTAINS_TEXT {#NOT-CONTAINS-TEXT}
```
public static final int NOT_CONTAINS_TEXT
```


此条件格式规则突出显示不包含指定文本的单元格。相当于使用 SEARCH() 工作表函数来判断单元格是否包含该文本。

### TIME_PERIOD {#TIME-PERIOD}
```
public static final int TIME_PERIOD
```


此条件格式规则突出显示在指定时间段内包含日期的单元格。会评估单元格的底层数值，因此单元格不需要设置为日期格式即可进行评估。例如，若单元格的值为 38913，则当规则要求的值为 2006/7/14 时，将应用此条件格式。

### TOP_10 {#TOP-10}
```
public static final int TOP_10
```


此条件格式规则突出显示其值位于指定的前 N 或后 N 区间的单元格。

### UNIQUE_VALUES {#UNIQUE-VALUES}
```
public static final int UNIQUE_VALUES
```


此条件格式规则突出显示范围内唯一的值。

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

