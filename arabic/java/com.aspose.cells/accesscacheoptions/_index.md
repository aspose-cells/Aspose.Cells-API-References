---
title: "AccessCacheOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "خيارات التخزين المؤقت للوصول إلى البيانات."
type: docs
url: /ar/java/com.aspose.cells/accesscacheoptions/
---

**Inheritance:**
java.lang.Object
```
public final class AccessCacheOptions
```

خيارات التخزين المؤقت للوصول إلى البيانات. يمكن دمج خيارات متعددة باستخدام عامل "\|".

**Remarks**

لبعض الميزات، يتطلب الوصول إلى مجموعة بيانات كبيرة الكثير من العمليات المتكررة والمعقدة مثل البحث، الحساب، ...إلخ، وهذه العمليات ستستغرق وقتًا إضافيًا كبيرًا. في الحالات الشائعة، تظل جميع البيانات التابعة غير متغيرة أثناء الوصول، لذا يمكن إنشاء بعض التخزينات المؤقتة واستخدامها لتحسين أداء الوصول. لهذا الغرض، نوفر هذه الواجهة البرمجية (API) حتى يتمكن المستخدم من تحديد نوع الوصول إلى البيانات الذي يحتاج إلى تحسين باستخدام آلية التخزين المؤقت الممكنة.

يرجى ملاحظة أنه بالنسبة للخيارات المختلفة، قد يتطلب مجموعة بيانات مختلفة أن تكون "للقراءة فقط". وتعتمد أداء الوصول إلى البيانات على العديد من الجوانب، ولا يضمن استخدام آلية التخزين المؤقت تحسين الأداء. في بعض الحالات، مثل عندما تكون مجموعة البيانات التي يتم الوصول إليها صغيرة، قد يؤدي استخدام التخزين المؤقت إلى زيادة الوقت لأن التخزين المؤقت نفسه يحتاج أيضًا إلى وقت إضافي.
## حقول

| حقل | الوصف |
| --- | --- |
| [ALL](#ALL) | تطبيق جميع التحسينات الممكنة لجميع أنواع الوصول إلى البيانات في دفتر العمل. |
| [CALCULATE_FORMULA](#CALCULATE-FORMULA) | تطبيق التحسين الممكن لحساب الصيغ. |
| [CELLS_DATA](#CELLS-DATA) | تطبيق التحسين الممكن للحصول على قيم الخلايا. |
| [CELL_DISPLAY](#CELL-DISPLAY) | تطبيق التحسين الممكن للحصول على النتائج المتعلقة بالعرض للخلايا([Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), [Cell.getStyle()](../../com.aspose.cells/cell\#getStyle--), [Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--), إلخ). |
| [CONDITIONAL_FORMATTING](#CONDITIONAL-FORMATTING) | تطبيق التحسين الممكن للحصول على نتيجة التنسيق للتنسيقات الشرطية. |
| [GET_FORMULA](#GET-FORMULA) | تطبيق التحسين الممكن للحصول على الصيغ. |
| [NONE](#NONE) | لا تخزين مؤقت لأي وصول إلى البيانات. |
| [POSITION_AND_SIZE](#POSITION-AND-SIZE) | تطبيق التحسين الممكن للحصول على موضع وحجم الكائن (مثل الشكل). |
| [SET_FORMULA](#SET-FORMULA) | تطبيق التحسين الممكن لتعيين الصيغ. |
| [VALIDATION](#VALIDATION) | تطبيق التحسين الممكن للحصول على نتيجة التحقق. |
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
### ALL {#ALL}
```
public static final int ALL
```


تطبيق جميع التحسينات الممكنة لجميع أنواع الوصول إلى البيانات في دفتر العمل. يجب عدم تغيير أي إعدادات أو بيانات أثناء الوصول المحسن.

### CALCULATE_FORMULA {#CALCULATE-FORMULA}
```
public static final int CALCULATE_FORMULA
```


تطبيق التحسين الممكن لحساب الصيغ. يجب عدم تغيير بيانات الخلايا أثناء الوصول المحسن، ولا ينبغي إنشاء أي كائنات جديدة (خلية، صف، إلخ) أيضًا (مثل باستخدام [Cells.get(int,int)](../../com.aspose.cells/cells\#get-int-int-)).

### CELLS_DATA {#CELLS-DATA}
```
public static final int CELLS_DATA
```


تطبيق التحسين الممكن للحصول على قيم الخلايا. يجب عدم تغيير بيانات الخلايا (البيانات وإعدادات الخلية والصف) أثناء الوصول المحسن، ولا ينبغي إنشاء أي كائنات جديدة من نوع خلية/صف أيضًا (مثل باستخدام [Cells.get(int,int)](../../com.aspose.cells/cells\#get-int-int-)).

### CELL_DISPLAY {#CELL-DISPLAY}
```
public static final int CELL_DISPLAY
```


تطبيق التحسين الممكن للحصول على النتائج المتعلقة بالعرض للخلايا([Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), [Cell.getStyle()](../../com.aspose.cells/cell\#getStyle--), [Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--), إلخ). يجب عدم تغيير بيانات الخلايا والكائنات المتعلقة بالنمط (أنماط الخلية/الصف/العمود، عرض العمود، إلخ) أثناء الوصول المحسن.

### CONDITIONAL_FORMATTING {#CONDITIONAL-FORMATTING}
```
public static final int CONDITIONAL_FORMATTING
```


تطبيق تحسين ممكن للحصول على نتيجة تنسيق الصيغ الشرطية. يجب عدم تغيير أي بيانات أو إعدادات قد تؤثر على نتيجة التنسيقات الشرطية (إعدادات التنسيقات الشرطية، قيم الخلايا التابعة، إلخ) أثناء الوصول المحسن.

### GET_FORMULA {#GET-FORMULA}
```
public static final int GET_FORMULA
```


تطبيق تحسين ممكن للحصول على الصيغ. يجب عدم تغيير أي بيانات أو إعدادات قد تؤثر على تعبير الصيغة (اسم ورقة العمل، نص الاسم، عمود الجدول، إلخ) أثناء الوصول المحسن.

### NONE {#NONE}
```
public static final int NONE
```


لا تخزين مؤقت لأي وصول إلى البيانات.

### POSITION_AND_SIZE {#POSITION-AND-SIZE}
```
public static final int POSITION_AND_SIZE
```


تطبيق تحسين ممكن للحصول على موضع وحجم الكائن (مثل الشكل). يجب عدم تغيير إعدادات ارتفاع الصف وعرض العمود أثناء الوصول المحسن.

### SET_FORMULA {#SET-FORMULA}
```
public static final int SET_FORMULA
```


تطبيق تحسين ممكن لتعيين الصيغ. يجب عدم تغيير أي بيانات أو إعدادات قد تؤثر على تعبير الصيغة (اسم ورقة العمل، نص الاسم، عمود الجدول، إلخ) أثناء الوصول المحسن.

### VALIDATION {#VALIDATION}
```
public static final int VALIDATION
```


تطبيق تحسين ممكن للحصول على نتيجة التحقق. يجب عدم تغيير أي بيانات أو إعدادات قد تؤثر على نتيجة التحقق (إعدادات التحقق، قيم الخلايا التابعة، إلخ) أثناء الوصول المحسن.

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

