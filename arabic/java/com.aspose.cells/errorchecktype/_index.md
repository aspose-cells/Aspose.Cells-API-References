---
title: "ErrorCheckType"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل جميع أنواع فحص الأخطاء."
type: docs
url: /ar/java/com.aspose.cells/errorchecktype/
---

**Inheritance:**
java.lang.Object
```
public final class ErrorCheckType
```

يمثل جميع أنواع فحص الأخطاء.
## حقول

| حقل | الوصف |
| --- | --- |
| [CALC](#CALC) | **ملاحظات** |
| [CALCULATED_COLUMN](#CALCULATED-COLUMN) | تجاهل الأخطاء عندما تحتوي الخلايا على قيمة مختلفة عن صيغة العمود المحسوبة. |
| [EMPTY_CELL_REF](#EMPTY-CELL-REF) | تجاهل الأخطاء عندما تشير الصيغ إلى خلايا فارغة. |
| [EVALUATION_ERROR](#EVALUATION-ERROR) | تجاهل الأخطاء عندما تحتوي الخلايا على صيغ تؤدي إلى خطأ. |
| [INCONSIST_FORMULA](#INCONSIST-FORMULA) | تجاهل الأخطاء عندما تختلف صيغة في منطقة من ورقة العمل عن صيغ أخرى في نفس المنطقة. |
| [INCONSIST_RANGE](#INCONSIST-RANGE) | تجاهل الأخطاء عندما تتغاضى الصيغ عن خلايا معينة في منطقة. |
| [NUMBER_STORED_AS_TEXT](#NUMBER-STORED-AS-TEXT) | تجاهل الأخطاء عندما تكون الأرقام مُنسقة كنص أو يسبقها علامة اقتباس مفردة |
| [TABLE_DATA_VALIDATION](#TABLE-DATA-VALIDATION) | تجاهل الأخطاء عندما لا يتوافق قيمة الخلية في جدول مع قواعد التحقق من البيانات المحددة. |
| [TEXT_DATE](#TEXT-DATE) | تجاهل الأخطاء عندما تحتوي الصيغ على خلايا منسقة كنص مع سنوات ممثلة برقمين. |
| [TEXT_NUMBER](#TEXT-NUMBER) | تجاهل الأخطاء عندما تكون الأرقام مُنسقة كنص أو يسبقها علامة اقتباس مفردة |
| [TWO_DIGIT_TEXT_YEAR](#TWO-DIGIT-TEXT-YEAR) | تجاهل الأخطاء عندما تحتوي الصيغ على خلايا منسقة كنص مع سنوات ممثلة برقمين. |
| [UNLOCKED_FORMULA](#UNLOCKED-FORMULA) | تجاهل الأخطاء عندما تحتوي الخلايا غير المقفلة على صيغ. |
| [UNPROCTED_FORMULA](#UNPROCTED-FORMULA) | تجاهل الأخطاء عندما تحتوي الخلايا غير المقفلة على صيغ. |
| [VALIDATION](#VALIDATION) | تجاهل الأخطاء عندما لا يتوافق قيمة الخلية في جدول مع قواعد التحقق من البيانات المحددة. |
## الطرق

| طريقة | الوصف |
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

ملاحظة: هذا العضو الآن غير مستخدم. بدلاً من ذلك، يرجى استخدام تعداد ErrorCheckType.EvaluationError. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أكتوبر 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### CALCULATED_COLUMN {#CALCULATED-COLUMN}
```
public static final int CALCULATED_COLUMN
```


تجاهل الأخطاء عندما تحتوي الخلايا على قيمة مختلفة عن صيغة العمود المحسوبة.

### EMPTY_CELL_REF {#EMPTY-CELL-REF}
```
public static final int EMPTY_CELL_REF
```


تجاهل الأخطاء عندما تشير الصيغ إلى خلايا فارغة.

### EVALUATION_ERROR {#EVALUATION-ERROR}
```
public static final int EVALUATION_ERROR
```


تجاهل الأخطاء عندما تحتوي الخلايا على صيغ تؤدي إلى خطأ.

### INCONSIST_FORMULA {#INCONSIST-FORMULA}
```
public static final int INCONSIST_FORMULA
```


تجاهل الأخطاء عندما تختلف صيغة في منطقة من ورقة العمل عن صيغ أخرى في نفس المنطقة.

### INCONSIST_RANGE {#INCONSIST-RANGE}
```
public static final int INCONSIST_RANGE
```


تجاهل الأخطاء عندما تتغاضى الصيغ عن خلايا معينة في منطقة.

### NUMBER_STORED_AS_TEXT {#NUMBER-STORED-AS-TEXT}
```
public static final int NUMBER_STORED_AS_TEXT
```


تجاهل الأخطاء عندما تكون الأرقام مُنسقة كنص أو يسبقها علامة اقتباس مفردة

### TABLE_DATA_VALIDATION {#TABLE-DATA-VALIDATION}
```
public static final int TABLE_DATA_VALIDATION
```


تجاهل الأخطاء عندما لا يتوافق قيمة الخلية في جدول مع قواعد التحقق من البيانات المحددة.

### TEXT_DATE {#TEXT-DATE}
```
public static final int TEXT_DATE
```


تجاهل الأخطاء عندما تحتوي الصيغ على خلايا منسقة كنص مع سنوات ممثلة برقمين.

**Remarks**

ملاحظة: هذا العضو الآن غير مستخدم. بدلاً من ذلك، يرجى استخدام تعداد ErrorCheckType.TwoDigitTextYear. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أكتوبر 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### TEXT_NUMBER {#TEXT-NUMBER}
```
public static final int TEXT_NUMBER
```


تجاهل الأخطاء عندما تكون الأرقام مُنسقة كنص أو يسبقها علامة اقتباس مفردة

**Remarks**

ملاحظة: هذا العضو الآن غير مستخدم. بدلاً من ذلك، يرجى استخدام تعداد ErrorCheckType.NumberStoredAsText. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أكتوبر 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### TWO_DIGIT_TEXT_YEAR {#TWO-DIGIT-TEXT-YEAR}
```
public static final int TWO_DIGIT_TEXT_YEAR
```


تجاهل الأخطاء عندما تحتوي الصيغ على خلايا منسقة كنص مع سنوات ممثلة برقمين.

### UNLOCKED_FORMULA {#UNLOCKED-FORMULA}
```
public static final int UNLOCKED_FORMULA
```


تجاهل الأخطاء عندما تحتوي الخلايا غير المقفلة على صيغ.

### UNPROCTED_FORMULA {#UNPROCTED-FORMULA}
```
public static final int UNPROCTED_FORMULA
```


تجاهل الأخطاء عندما تحتوي الخلايا غير المقفلة على صيغ.

**Remarks**

ملاحظة: هذا العضو الآن غير مستخدم. بدلاً من ذلك، يرجى استخدام تعداد ErrorCheckType.UnproctedFormula. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أكتوبر 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### VALIDATION {#VALIDATION}
```
public static final int VALIDATION
```


تجاهل الأخطاء عندما لا يتوافق قيمة الخلية في جدول مع قواعد التحقق من البيانات المحددة.

**Remarks**

ملاحظة: هذا العضو الآن غير مستخدم. بدلاً من ذلك، يرجى استخدام تعداد ErrorCheckType.TableDataValidation. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أكتوبر 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

