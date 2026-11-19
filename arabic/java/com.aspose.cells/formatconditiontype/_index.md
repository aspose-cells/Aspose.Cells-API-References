---
title: "FormatConditionType"
second_title: "Aspose.Cells for Java API Reference"
description: "نوع قاعدة التنسيق الشرطي."
type: docs
url: /ar/java/com.aspose.cells/formatconditiontype/
---

**Inheritance:**
java.lang.Object
```
public final class FormatConditionType
```

نوع قاعدة التنسيق الشرطي.
## حقول

| حقل | الوصف |
| --- | --- |
| [ABOVE_AVERAGE](#ABOVE-AVERAGE) | تُبرز قاعدة تنسيق الخلايا الشرطية هذه الخلايا التي تكون أعلى أو أقل من المتوسط لجميع القيم في النطاق. |
| [BEGINS_WITH](#BEGINS-WITH) | تُبرز قاعدة تنسيق الخلايا الشرطية هذه الخلايا في النطاق التي تبدأ بالنص المحدد. |
| [CELL_VALUE](#CELL-VALUE) | تقارن قاعدة تنسيق الخلايا الشرطية هذه قيمة الخلية بنتيجة حسابية مستندة إلى صيغة، باستخدام عامل. |
| [COLOR_SCALE](#COLOR-SCALE) | تنشئ قاعدة تنسيق الخلايا الشرطية هذه مقياس ألوان متدرج على الخلايا. |
| [CONTAINS_BLANKS](#CONTAINS-BLANKS) | تُبرز قاعدة تنسيق الخلايا الشرطية هذه الخلايا التي تكون فارغة تمامًا. |
| [CONTAINS_ERRORS](#CONTAINS-ERRORS) | تُبرز قاعدة تنسيق الخلايا الشرطية هذه الخلايا التي تحتوي على أخطاء في الصيغة. |
| [CONTAINS_TEXT](#CONTAINS-TEXT) | تُبرز قاعدة تنسيق الخلايا الشرطية هذه الخلايا التي تحتوي على النص المحدد. |
| [DATA_BAR](#DATA-BAR) | تعرض قاعدة تنسيق الخلايا الشرطية هذه شريط بيانات متدرج في نطاق الخلايا. |
| [DUPLICATE_VALUES](#DUPLICATE-VALUES) | تُبرز قاعدة تنسيق الخلايا الشرطية هذه القيم المكررة. |
| [ENDS_WITH](#ENDS-WITH) | تُبرز قاعدة تنسيق الخلايا الشرطية هذه الخلايا التي تنتهي بالنص المحدد. |
| [EXPRESSION](#EXPRESSION) | تحتوي قاعدة تنسيق الخلايا الشرطية هذه على صيغة للتقييم. |
| [ICON_SET](#ICON-SET) | تطبق قاعدة تنسيق الخلايا الشرطية هذه أيقونات على الخلايا وفقًا لقيمها. |
| [NOT_CONTAINS_BLANKS](#NOT-CONTAINS-BLANKS) | تُبرز قاعدة تنسيق الخلايا الشرطية هذه الخلايا التي ليست فارغة. |
| [NOT_CONTAINS_ERRORS](#NOT-CONTAINS-ERRORS) | تُبرز قاعدة تنسيق الخلايا الشرطية هذه الخلايا التي لا تحتوي على أخطاء في الصيغة. |
| [NOT_CONTAINS_TEXT](#NOT-CONTAINS-TEXT) | تُبرز قاعدة تنسيق الخلايا الشرطية هذه الخلايا التي لا تحتوي على النص المحدد. |
| [TIME_PERIOD](#TIME-PERIOD) | تُبرز قاعدة تنسيق الخلايا الشرطية هذه الخلايا التي تحتوي على تواريخ في الفترة الزمنية المحددة. |
| [TOP_10](#TOP-10) | تُبرز قاعدة تنسيق الخلايا الشرطية هذه الخلايا التي تقع قيمها في الفئة العليا N أو الفئة السفلى N، حسب التحديد. |
| [UNIQUE_VALUES](#UNIQUE-VALUES) | تُبرز قاعدة تنسيق الخلايا الشرطية هذه القيم الفريدة في النطاق. |
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
### ABOVE_AVERAGE {#ABOVE-AVERAGE}
```
public static final int ABOVE_AVERAGE
```


تُبرز قاعدة تنسيق الخلايا الشرطية هذه الخلايا التي تكون أعلى أو أقل من المتوسط لجميع القيم في النطاق.

### BEGINS_WITH {#BEGINS-WITH}
```
public static final int BEGINS_WITH
```


تُبرز قاعدة تنسيق الخلايا الشرطية هذه الخلايا في النطاق التي تبدأ بالنص المحدد. يعادل استخدام دالة LEFT() في الورقة ومقارنة القيم.

### CELL_VALUE {#CELL-VALUE}
```
public static final int CELL_VALUE
```


تقارن قاعدة تنسيق الخلايا الشرطية هذه قيمة الخلية بنتيجة حسابية مستندة إلى صيغة، باستخدام عامل.

### COLOR_SCALE {#COLOR-SCALE}
```
public static final int COLOR_SCALE
```


تنشئ قاعدة تنسيق الخلايا الشرطية هذه مقياس ألوان متدرج على الخلايا.

### CONTAINS_BLANKS {#CONTAINS-BLANKS}
```
public static final int CONTAINS_BLANKS
```


تُبرز قاعدة تنسيق الخلايا الشرطية هذه الخلايا التي تكون فارغة تمامًا. يعادل استخدام LEN(TRIM()). يعني ذلك أنه إذا كانت الخلية تحتوي فقط على أحرف ستزيلها الدالة TRIM()، فستُعتبر فارغة. الخلية الفارغة أيضًا تُعتبر فارغة.

### CONTAINS_ERRORS {#CONTAINS-ERRORS}
```
public static final int CONTAINS_ERRORS
```


تُبرز قاعدة تنسيق الخلايا الشرطية هذه الخلايا التي تحتوي على أخطاء في الصيغة. يعادل استخدام دالة ISERROR() في الورقة لتحديد ما إذا كان هناك خطأ في الصيغة.

### CONTAINS_TEXT {#CONTAINS-TEXT}
```
public static final int CONTAINS_TEXT
```


تُبرز قاعدة تنسيق الخلايا الشرطية هذه الخلايا التي تحتوي على النص المحدد. يعادل استخدام دالة SEARCH() في الورقة لتحديد ما إذا كانت الخلية تحتوي على النص.

### DATA_BAR {#DATA-BAR}
```
public static final int DATA_BAR
```


تعرض قاعدة تنسيق الخلايا الشرطية هذه شريط بيانات متدرج في نطاق الخلايا.

### DUPLICATE_VALUES {#DUPLICATE-VALUES}
```
public static final int DUPLICATE_VALUES
```


تُبرز قاعدة تنسيق الخلايا الشرطية هذه القيم المكررة.

### ENDS_WITH {#ENDS-WITH}
```
public static final int ENDS_WITH
```


تُبرز قاعدة تنسيق الخلايا الشرطية هذه الخلايا التي تنتهي بالنص المحدد. يعادل استخدام دالة RIGHT() في الورقة ومقارنة القيم.

### EXPRESSION {#EXPRESSION}
```
public static final int EXPRESSION
```


تحتوي قاعدة تنسيق الخلايا الشرطية هذه على صيغة للتقييم. عندما تكون نتيجة الصيغة صحيحة، يتم تمييز الخلية.

### ICON_SET {#ICON-SET}
```
public static final int ICON_SET
```


تطبق قاعدة تنسيق الخلايا الشرطية هذه أيقونات على الخلايا وفقًا لقيمها.

### NOT_CONTAINS_BLANKS {#NOT-CONTAINS-BLANKS}
```
public static final int NOT_CONTAINS_BLANKS
```


تُبرز قاعدة تنسيق الخلايا الشرطية هذه الخلايا التي ليست فارغة. ما يعادل استخدام LEN(TRIM()). يعني ذلك أنه إذا احتوت الخلية على أحرف فقط سيزيلها TRIM()، فستُعتبر فارغة. الخلية الفارغة تُعتبر أيضًا فارغة.

### NOT_CONTAINS_ERRORS {#NOT-CONTAINS-ERRORS}
```
public static final int NOT_CONTAINS_ERRORS
```


تُبرز قاعدة تنسيق الخلايا الشرطية هذه الخلايا التي لا تحتوي على أخطاء في الصيغة. ما يعادل استخدام دالة ISERROR() في الورقة لتحديد ما إذا كان هناك خطأ في الصيغة.

### NOT_CONTAINS_TEXT {#NOT-CONTAINS-TEXT}
```
public static final int NOT_CONTAINS_TEXT
```


تُبرز قاعدة تنسيق الخلايا الشرطية هذه الخلايا التي لا تحتوي على النص المحدد. ما يعادل استخدام دالة SEARCH() في الورقة لتحديد ما إذا كانت الخلية تحتوي على النص أم لا.

### TIME_PERIOD {#TIME-PERIOD}
```
public static final int TIME_PERIOD
```


تُبرز قاعدة تنسيق الخلايا الشرطية هذه الخلايا التي تحتوي على تواريخ في الفترة الزمنية المحددة. يتم تقييم القيمة الأساسية للخلية، لذلك لا يلزم تنسيق الخلية ك تاريخ لتقييمها. على سبيل المثال، إذا كانت الخلية تحتوي على القيمة 38913 فسيتم تطبيق التنسيق الشرطي إذا كانت القاعدة تتطلب قيمة 7/14/2006.

### TOP_10 {#TOP-10}
```
public static final int TOP_10
```


تُبرز قاعدة تنسيق الخلايا الشرطية هذه الخلايا التي تقع قيمها في الفئة العليا N أو الفئة السفلى N، حسب التحديد.

### UNIQUE_VALUES {#UNIQUE-VALUES}
```
public static final int UNIQUE_VALUES
```


تُبرز قاعدة تنسيق الخلايا الشرطية هذه القيم الفريدة في النطاق.

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

