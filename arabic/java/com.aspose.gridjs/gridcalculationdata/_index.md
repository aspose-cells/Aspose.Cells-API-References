---
title: "GridCalculationData"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل البيانات المطلوبة عند حساب دالة واحدة مثل معلمات اسم الدالة ... إلخ."
type: docs
url: /ar/java/com.aspose.gridjs/gridcalculationdata/
---

**Inheritance:**
java.lang.Object
```
public class GridCalculationData
```

يمثل البيانات المطلوبة عند حساب دالة واحدة، مثل اسم الدالة، المعلمات، ... إلخ.

**Remarks**

جميع الكائنات التي توفرها هذه الفئة مخصصة لغرض "القراءة" فقط. يجب على المستخدم عدم تغيير أي بيانات في المصنف أثناء عملية حساب الصيغة، وإلا قد يحدث نتيجة غير متوقعة أو استثناء.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | يحصل على القيمة المحسوبة لهذه الدالة. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | يحصل على فهرس عمود الخلية التي توجد فيها الدالة. |
| [getFormula()](#getFormula--) | يحصل على صيغة الخلية التي توجد فيها الدالة. |
| [getFunctionName()](#getFunctionName--) | يحصل على اسم الدالة التي سيتم حسابها. |
| [getParamCount()](#getParamCount--) | يحصل على عدد المعلمات. |
| [getParamText(int index)](#getParamText-int-) | يحصل على النص الحرفي للمعلمة عند الفهرس المحدد. |
| [getParamValue(int index)](#getParamValue-int-) | يحصل على كائن القيمة الممثلة للمعلمة عند الفهرس المحدد. |
| [getRow()](#getRow--) | يحصل على فهرس صف الخلية التي توجد فيها الدالة. |
| [getSheetName()](#getSheetName--) | يحصل على اسم ورقة العمل التي توجد فيها الدالة. |
| [getStringValue()](#getStringValue--) | يحصل على قيمة عرض السلسلة للخلية التي توجد فيها الدالة. |
| [getValue()](#getValue--) | يحصل على قيمة الخلية التي توجد فيها الدالة. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculatedValue(Object value)](#setCalculatedValue-java.lang.Object-) | يضبط القيمة المحسوبة لهذه الدالة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getCalculatedValue() {#getCalculatedValue--}
```
public Object getCalculatedValue()
```


يحصل على القيمة المحسوبة لهذه الدالة.

**Remarks**

يجب على المستخدم تعيين هذه الخاصية في محرك الحساب المخصص الخاص به لتلك الدوال التي يدعمها المحرك، وسيتم إرجاع القيمة المعينة عند الحصول على هذه الخاصية. الحصول على هذه الخاصية قبل تعيينها سيجعل الدالة تُحسب بواسطة محرك الحساب الافتراضي لـ Aspose.Cells وسيتم إرجاع القيمة المحسوبة.

**Returns:**
java.lang.Object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


يحصل على فهرس عمود الخلية التي توجد فيها الدالة.

**Returns:**
int
### getFormula() {#getFormula--}
```
public String getFormula()
```


يحصل على صيغة الخلية التي توجد فيها الدالة.

**Returns:**
java.lang.String
### getFunctionName() {#getFunctionName--}
```
public String getFunctionName()
```


يحصل على اسم الدالة التي سيتم حسابها.

**Returns:**
java.lang.String
### getParamCount() {#getParamCount--}
```
public int getParamCount()
```


يحصل على عدد المعلمات.

**Returns:**
int
### getParamText(int index) {#getParamText-int-}
```
public String getParamText(int index)
```


يحصل على النص الحرفي للمعلمة عند الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس المعلمة (بدءًا من 0). |

**Returns:**
java.lang.String - النص الحرفي للمعلمة.
### getParamValue(int index) {#getParamValue-int-}
```
public Object getParamValue(int index)
```


يحصل على كائن القيمة الممثلة للمعلمة عند الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس المعلمة (بدءًا من 0). |

**Returns:**
java.lang.Object - إذا كانت المعلمة قيمة عادية، فإنها تُعيد القيمة العادية. إذا كانت المعلمة إشارة، فإنها تُعيد كائن ReferredArea.
### getRow() {#getRow--}
```
public int getRow()
```


يحصل على فهرس صف الخلية التي توجد فيها الدالة.

**Returns:**
int
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


يحصل على اسم ورقة العمل التي توجد فيها الدالة.

**Returns:**
java.lang.String
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


يحصل على قيمة عرض السلسلة للخلية التي توجد فيها الدالة.

**Returns:**
java.lang.String
### getValue() {#getValue--}
```
public Object getValue()
```


يحصل على قيمة الخلية التي توجد فيها الدالة.

**Returns:**
java.lang.Object
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




### setCalculatedValue(Object value) {#setCalculatedValue-java.lang.Object-}
```
public void setCalculatedValue(Object value)
```


يضبط القيمة المحسوبة لهذه الدالة.

**Remarks**

يجب على المستخدم تعيين هذه الخاصية في محرك الحساب المخصص الخاص به لتلك الدوال التي يدعمها المحرك، وسيتم إرجاع القيمة المعينة عند الحصول على هذه الخاصية. الحصول على هذه الخاصية قبل تعيينها سيجعل الدالة تُحسب بواسطة محرك الحساب الافتراضي لـ Aspose.Cells وسيتم إرجاع القيمة المحسوبة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object |  |

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

