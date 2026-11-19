---
title: "GridCalculationData"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل البيانات المطلوبة عند حساب دالة واحدة مثل معلمات اسم الدالة ... إلخ."
type: docs
url: /ar/java/com.aspose.gridweb/gridcalculationdata/
---

**Inheritance:**
java.lang.Object
```
public class GridCalculationData
```

يمثل البيانات المطلوبة عند حساب دالة واحدة، مثل اسم الدالة، المعلمات، ... إلخ.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | يحصل على القيمة المحسوبة لهذه الدالة. |
| [getCell()](#getCell--) | يحصل على كائن Cell حيث توجد الدالة. |
| [getClass()](#getClass--) |  |
| [getFunctionName()](#getFunctionName--) | يحصل على اسم الدالة التي سيتم حسابها. |
| [getParamCount()](#getParamCount--) | يحصل على عدد المعلمات |
| [getParamText(int index)](#getParamText-int-) | يحصل على النص الحرفي للمعلمة عند الفهرس المحدد. |
| [getParamValue(int index)](#getParamValue-int-) | يحصل على كائن القيمة الممثلة للمعلمة عند الفهرس المحدد. |
| [getWorkbook()](#getWorkbook--) | يحصل على كائن Workbook حيث توجد الدالة. |
| [getWorksheet()](#getWorksheet--) | يحصل على كائن Workbook حيث توجد الدالة. |
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
### getCell() {#getCell--}
```
public GridCell getCell()
```


يحصل على كائن Cell حيث توجد الدالة.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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


يحصل على عدد المعلمات

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
| الفهرس | int | فهرس المعلمة (بدءًا من 0) |

**Returns:**
java.lang.String - النص الحرفي للمعلمة
### getParamValue(int index) {#getParamValue-int-}
```
public Object getParamValue(int index)
```


يحصل على كائن القيمة الممثلة للمعلمة عند الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس المعلمة (بدءًا من 0) |

**Returns:**
java.lang.Object - إذا كانت المعلمة قيمة عادية، فإنها تُعيد القيمة العادية. إذا كانت المعلمة إشارة، فإنها تُعيد كائن ReferredArea.
### getWorkbook() {#getWorkbook--}
```
public GridWorkbook getWorkbook()
```


يحصل على كائن Workbook حيث توجد الدالة.

**Returns:**
[GridWorkbook](../../com.aspose.gridweb/gridworkbook)
### getWorksheet() {#getWorksheet--}
```
public GridWorksheet getWorksheet()
```


يحصل على كائن Workbook حيث توجد الدالة.

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet)
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

