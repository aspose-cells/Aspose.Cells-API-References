---
title: "GridValidationType"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل نوع التحقق من صحة البيانات."
type: docs
url: /ar/java/com.aspose.gridweb/gridvalidationtype/
---

**Inheritance:**
java.lang.Object
```
public final class GridValidationType
```

يمثل نوع التحقق من صحة البيانات.
## حقول

| حقل | الوصف |
| --- | --- |
| [ANY_VALUE](#ANY-VALUE) | نوع التحقق من أي قيمة. |
| [BOOLEAN](#BOOLEAN) | صحيح أو خطأ |
| [CHECK_BOX](#CHECK-BOX) | عرض الخلية كخانة اختيار. |
| [CUSTOM](#CUSTOM) | نوع التحقق المخصص. |
| [CUSTOM_EXPRESSION](#CUSTOM-EXPRESSION) | نوع التحقق المخصص، باستخدام التعبير النمطي. |
| [CUSTOM_FUNCTION](#CUSTOM-FUNCTION) | التحقق باستخدام دالة جافاسكريبت مخصصة. |
| [CUSTOM_SERVER_FUNCTION](#CUSTOM-SERVER-FUNCTION) | التحقق باستخدام دالة مخصصة على الخادم. |
| [DATE](#DATE) | نوع التحقق من التاريخ. |
| [DATE_TIME](#DATE-TIME) | DateTime (yyyy-MM-dd أو yyyy-MM-dd hh:mm:ss). |
| [DECIMAL](#DECIMAL) | نوع التحقق العشري. |
| [DROP_DOWN_LIST](#DROP-DOWN-LIST) | إظهار قائمة منسدلة. |
| [FREE_LIST](#FREE-LIST) | نوع التحقق القائمة الحرة. |
| [LIST](#LIST) | نوع التحقق من القائمة. |
| [TEXT_LENGTH](#TEXT-LENGTH) | نوع التحقق من طول النص. |
| [TIME](#TIME) | نوع التحقق من الوقت. |
| [WHOLE_NUMBER](#WHOLE-NUMBER) | نوع التحقق من العدد الصحيح. |
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
### ANY_VALUE {#ANY-VALUE}
```
public static final int ANY_VALUE
```


نوع التحقق من أي قيمة.

### BOOLEAN {#BOOLEAN}
```
public static final int BOOLEAN
```


صحيح أو خطأ

### CHECK_BOX {#CHECK-BOX}
```
public static final int CHECK_BOX
```


عرض الخلية كخانة اختيار. وقيمة الخلية هي True أو False.

### CUSTOM {#CUSTOM}
```
public static final int CUSTOM
```


نوع التحقق المخصص.

### CUSTOM_EXPRESSION {#CUSTOM-EXPRESSION}
```
public static final int CUSTOM_EXPRESSION
```


نوع التحقق المخصص، باستخدام التعبير النمطي.

### CUSTOM_FUNCTION {#CUSTOM-FUNCTION}
```
public static final int CUSTOM_FUNCTION
```


التحقق باستخدام دالة جافاسكريبت مخصصة.

**Remarks**

استخدم الخاصية ClientValidationFunction لتحديد اسم دالة التحقق من العميل. يجب إعلان الدالة بهذه الصيغة:
function customValicationFunction(source, value)
المعامل "source" هو كائن الخلية. المعامل "value" هو قيمة النص لخلية يتم فحصها. يجب أن تُرجع الدالة true إذا كانت القيمة صالحة.

### CUSTOM_SERVER_FUNCTION {#CUSTOM-SERVER-FUNCTION}
```
public static final int CUSTOM_SERVER_FUNCTION
```


التحقق باستخدام دالة مخصصة على الخادم.

**Remarks**

استخدم الخاصية CustomServerFunction لتحديد التحقق من جانب الخادم. أدناه مثال على الشيفرة:
أولاً عرّف الفئة التي تنفّذ GridCustomServerValidation كالتالي: myservervali : GridCustomServerValidation
...... ثم أضف التحقق var gridValidationCollection = this.GridWeb.ActiveSheet.Validations;
GridValidation gv = gridValidationCollection.Add(new GridCellArea(1, 1, 2, 2));
gv.ValidationType = GridValidationType.CustomServerFunction; gv.ServerValidation = new myservervali(); ثم اضبط ClientValidationFunction للتعامل مع منطق العميل عندما يفشل التحقق من الخادم وإرجاع الرسالة gv.ClientValidationFunction = "ValidationErrorClientFunction"; يجب إعلان دالة العميل هكذا: function ValidationErrorClientFunction(cell,msg) يرجى مراجعة صفحة العرض للحصول على مرجع تفصيلي

### DATE {#DATE}
```
public static final int DATE
```


نوع التحقق من التاريخ.

### DATE_TIME {#DATE-TIME}
```
public static final int DATE_TIME
```


DateTime (yyyy-MM-dd أو yyyy-MM-dd hh:mm:ss).

### DECIMAL {#DECIMAL}
```
public static final int DECIMAL
```


نوع التحقق العشري.

### DROP_DOWN_LIST {#DROP-DOWN-LIST}
```
public static final int DROP_DOWN_LIST
```


إظهار قائمة منسدلة.

### FREE_LIST {#FREE-LIST}
```
public static final int FREE_LIST
```


نوع التحقق القائمة الحرة.

### LIST {#LIST}
```
public static final int LIST
```


نوع التحقق من القائمة.

### TEXT_LENGTH {#TEXT-LENGTH}
```
public static final int TEXT_LENGTH
```


نوع التحقق من طول النص.

### TIME {#TIME}
```
public static final int TIME
```


نوع التحقق من الوقت.

### WHOLE_NUMBER {#WHOLE-NUMBER}
```
public static final int WHOLE_NUMBER
```


نوع التحقق من العدد الصحيح.

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

