---
title: "ErrorCheckType"
second_title: "Aspose.Cells for Java API 参考"
description: "表示所有错误检查类型。"
type: docs
url: /zh/java/com.aspose.cells/errorchecktype/
---

**Inheritance:**
java.lang.Object
```
public final class ErrorCheckType
```

表示所有错误检查类型。
## 字段

| 字段 | 描述 |
| --- | --- |
| [CALC](#CALC) | **备注** |
| [CALCULATED_COLUMN](#CALCULATED-COLUMN) | 当单元格的值与计算列公式不同时时，忽略错误。 |
| [EMPTY_CELL_REF](#EMPTY-CELL-REF) | 当公式引用空单元格时，忽略错误。 |
| [EVALUATION_ERROR](#EVALUATION-ERROR) | 当单元格包含导致错误的公式时，忽略错误。 |
| [INCONSIST_FORMULA](#INCONSIST-FORMULA) | 当工作表区域中的公式与同一区域的其他公式不同时，忽略错误。 |
| [INCONSIST_RANGE](#INCONSIST-RANGE) | 当公式在区域中省略某些单元格时，忽略错误。 |
| [NUMBER_STORED_AS_TEXT](#NUMBER-STORED-AS-TEXT) | 当数字被格式化为文本或前面带有撇号时，忽略错误。 |
| [TABLE_DATA_VALIDATION](#TABLE-DATA-VALIDATION) | 当表格中单元格的值不符合指定的数据验证规则时，忽略错误。 |
| [TEXT_DATE](#TEXT-DATE) | 当公式包含以两位数字表示年份的文本格式单元格时，忽略错误。 |
| [TEXT_NUMBER](#TEXT-NUMBER) | 当数字被格式化为文本或前面带有撇号时，忽略错误。 |
| [TWO_DIGIT_TEXT_YEAR](#TWO-DIGIT-TEXT-YEAR) | 当公式包含以两位数字表示年份的文本格式单元格时，忽略错误。 |
| [UNLOCKED_FORMULA](#UNLOCKED-FORMULA) | 当未锁定的单元格包含公式时，忽略错误。 |
| [UNPROCTED_FORMULA](#UNPROCTED-FORMULA) | 当未锁定的单元格包含公式时，忽略错误。 |
| [VALIDATION](#VALIDATION) | 当表格中单元格的值不符合指定的数据验证规则时，忽略错误。 |
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
### CALC {#CALC}
```
public static final int CALC
```


**Remarks**

注意：此成员已过时。请改用 ErrorCheckType.EvaluationError 枚举。此方法将在自2023年10月起的12个月后移除。Aspose 对您可能遇到的不便表示歉意。

### CALCULATED_COLUMN {#CALCULATED-COLUMN}
```
public static final int CALCULATED_COLUMN
```


当单元格的值与计算列公式不同时时，忽略错误。

### EMPTY_CELL_REF {#EMPTY-CELL-REF}
```
public static final int EMPTY_CELL_REF
```


当公式引用空单元格时，忽略错误。

### EVALUATION_ERROR {#EVALUATION-ERROR}
```
public static final int EVALUATION_ERROR
```


当单元格包含导致错误的公式时，忽略错误。

### INCONSIST_FORMULA {#INCONSIST-FORMULA}
```
public static final int INCONSIST_FORMULA
```


当工作表区域中的公式与同一区域的其他公式不同时，忽略错误。

### INCONSIST_RANGE {#INCONSIST-RANGE}
```
public static final int INCONSIST_RANGE
```


当公式在区域中省略某些单元格时，忽略错误。

### NUMBER_STORED_AS_TEXT {#NUMBER-STORED-AS-TEXT}
```
public static final int NUMBER_STORED_AS_TEXT
```


当数字被格式化为文本或前面带有撇号时，忽略错误。

### TABLE_DATA_VALIDATION {#TABLE-DATA-VALIDATION}
```
public static final int TABLE_DATA_VALIDATION
```


当表格中单元格的值不符合指定的数据验证规则时，忽略错误。

### TEXT_DATE {#TEXT-DATE}
```
public static final int TEXT_DATE
```


当公式包含以两位数字表示年份的文本格式单元格时，忽略错误。

**Remarks**

注意：此成员已过时。请改用 ErrorCheckType.TwoDigitTextYear 枚举。此方法将在自2023年10月起的12个月后移除。Aspose 对您可能遇到的不便表示歉意。

### TEXT_NUMBER {#TEXT-NUMBER}
```
public static final int TEXT_NUMBER
```


当数字被格式化为文本或前面带有撇号时，忽略错误。

**Remarks**

注意：此成员已过时。请改用 ErrorCheckType.NumberStoredAsText 枚举。此方法将在自2023年10月起的12个月后移除。Aspose 对您可能遇到的不便表示歉意。

### TWO_DIGIT_TEXT_YEAR {#TWO-DIGIT-TEXT-YEAR}
```
public static final int TWO_DIGIT_TEXT_YEAR
```


当公式包含以两位数字表示年份的文本格式单元格时，忽略错误。

### UNLOCKED_FORMULA {#UNLOCKED-FORMULA}
```
public static final int UNLOCKED_FORMULA
```


当未锁定的单元格包含公式时，忽略错误。

### UNPROCTED_FORMULA {#UNPROCTED-FORMULA}
```
public static final int UNPROCTED_FORMULA
```


当未锁定的单元格包含公式时，忽略错误。

**Remarks**

注意：此成员已过时。请改用 ErrorCheckType.UnproctedFormula 枚举。此方法将在自2023年10月起的12个月后移除。Aspose 对您可能遇到的不便表示歉意。

### VALIDATION {#VALIDATION}
```
public static final int VALIDATION
```


当表格中单元格的值不符合指定的数据验证规则时，忽略错误。

**Remarks**

注意：此成员已过时。请改用 ErrorCheckType.TableDataValidation 枚举。此方法将在自2023年10月起的12个月后移除。Aspose 对您可能遇到的不便表示歉意。

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

