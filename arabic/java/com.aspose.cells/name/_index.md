---
title: "Name"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل اسمًا معرفًا لنطاق من الخلايا."
type: docs
url: /ar/java/com.aspose.cells/name/
---

**Inheritance:**
java.lang.Object
```
public class Name
```

يمثل اسمًا معرفًا لنطاق من الخلايا.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Creating a named range
         Range range = worksheet.getCells().createRange("B4", "G14");
         //Setting the name of the named range
         range.setName("TestRange");
         //Saving the modified Excel file in default (that is Excel 2000) format
         workbook.save("output.xls");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getComment()](#getComment--) | يحصل على تعليق الاسم. |
| [getFullText()](#getFullText--) | يحصل على النص الكامل لاسم الكائن مع إعداد النطاق. |
| [getR1C1RefersTo()](#getR1C1RefersTo--) | يحصل على إشارة R1C1 للـ [Name](../../com.aspose.cells/name). |
| [getRange()](#getRange--) | يحصل على النطاق إذا كان هذا الاسم يشير إلى نطاق. |
| [getRange(boolean recalculate)](#getRange-boolean-) | يحصل على النطاق إذا كان هذا الاسم يشير إلى نطاق |
| [getRange(int sheetIndex, int row, int column)](#getRange-int-int-int-) | يحصل على النطاق إذا كان هذا الاسم يشير إلى نطاق. |
| [getRanges()](#getRanges--) | يحصل على جميع النطاقات التي يشير إليها هذا الاسم. |
| [getRanges(boolean recalculate)](#getRanges-boolean-) | يحصل على جميع النطاقات التي يشير إليها هذا الاسم. |
| [getReferredAreas(boolean recalculate)](#getReferredAreas-boolean-) | يحصل على جميع الإشارات التي يشير إليها هذا الاسم. |
| [getRefersTo()](#getRefersTo--) | يرجع أو يعيّن الصيغة التي يُعرّف الاسم للإشارة إليها، وتبدأ بعلامة مساواة. |
| [getRefersTo(boolean isR1C1, boolean isLocal)](#getRefersTo-boolean-boolean-) | احصل على مرجع هذا الاسم. |
| [getRefersTo(boolean isR1C1, boolean isLocal, int row, int column)](#getRefersTo-boolean-boolean-int-int-) | احصل على مرجع هذا الاسم بناءً على الخلية المحددة. |
| [getSheetIndex()](#getSheetIndex--) | يشير إلى أن هذا الاسم ينتمي إلى المصنف أو ورقة العمل. 0 = اسم عالمي، وإلا فالفهرس إلى الورقة (مبني على الواحد). |
| [getText()](#getText--) | يحصل على نص الاسم للكائن. |
| [hashCode()](#hashCode--) |  |
| [isReferred()](#isReferred--) | يشير إلى ما إذا كان هذا الاسم مُشارًا إليه من قبل صيغ أخرى. |
| [isVisible()](#isVisible--) | يشير إلى ما إذا كان الاسم مرئيًا. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setComment(String value)](#setComment-java.lang.String-) | يضبط تعليق الاسم. |
| [setR1C1RefersTo(String value)](#setR1C1RefersTo-java.lang.String-) | يضبط مرجع R1C1 لـ [Name](../../com.aspose.cells/name). |
| [setRefersTo(String value)](#setRefersTo-java.lang.String-) | يرجع أو يعيّن الصيغة التي يُعرّف الاسم للإشارة إليها، وتبدأ بعلامة مساواة. |
| [setRefersTo(String refersTo, boolean isR1C1, boolean isLocal)](#setRefersTo-java.lang.String-boolean-boolean-) | اضبط مرجع هذا الاسم. |
| [setSheetIndex(int value)](#setSheetIndex-int-) | يشير إلى أن هذا الاسم ينتمي إلى المصنف أو ورقة العمل. 0 = اسم عالمي، وإلا فالفهرس إلى الورقة (مبني على الواحد). |
| [setText(String value)](#setText-java.lang.String-) | يحصل على نص الاسم للكائن. |
| [setVisible(boolean value)](#setVisible-boolean-) | يشير إلى ما إذا كان الاسم مرئيًا. |
| [toString()](#toString--) | يرجع سلسلة تمثل كائن النطاق الحالي. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getComment() {#getComment--}
```
public String getComment()
```


يحصل على تعليق الاسم. ينطبق فقط على Excel 2007 أو الإصدارات الأحدث.

**Returns:**
java.lang.String
### getFullText() {#getFullText--}
```
public String getFullText()
```


يحصل على النص الكامل لاسم الكائن مع إعداد النطاق.

**Returns:**
java.lang.String
### getR1C1RefersTo() {#getR1C1RefersTo--}
```
public String getR1C1RefersTo()
```


يحصل على إشارة R1C1 للـ [Name](../../com.aspose.cells/name).

**Returns:**
java.lang.String
### getRange() {#getRange--}
```
public Range getRange()
```


يحصل على النطاق إذا كان هذا الاسم يشير إلى نطاق.

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRange(boolean recalculate) {#getRange-boolean-}
```
public Range getRange(boolean recalculate)
```


يحصل على النطاق إذا كان هذا الاسم يشير إلى نطاق

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| إعادة حساب | boolean | ما إذا كان يجب إعادة حسابه إذا تم حساب هذا الاسم مسبقًا قبل هذا الاستدعاء. |

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRange(int sheetIndex, int row, int column) {#getRange-int-int-int-}
```
public Range getRange(int sheetIndex, int row, int column)
```


يحصل على النطاق إذا كان هذا الاسم يشير إلى نطاق. إذا لم يكن مرجع هذا الاسم مطلقًا، قد يختلف النطاق بين الخلايا المختلفة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetIndex | int | فهرس الورقة المقابل. |
| صف | int | فهرس الصف المقابل. |
| عمود | int | فهرس العمود المقابل |

**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRanges() {#getRanges--}
```
public Range[] getRanges()
```


يحصل على جميع النطاقات التي يشير إليها هذا الاسم.

**Returns:**
com.aspose.cells.Range[] - جميع النطاقات.
### getRanges(boolean recalculate) {#getRanges-boolean-}
```
public Range[] getRanges(boolean recalculate)
```


يحصل على جميع النطاقات التي يشير إليها هذا الاسم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| إعادة حساب | boolean | ما إذا كان يجب إعادة حسابه إذا تم حساب هذا الاسم مسبقًا قبل هذا الاستدعاء. |

**Returns:**
com.aspose.cells.Range[] - جميع النطاقات.
### getReferredAreas(boolean recalculate) {#getReferredAreas-boolean-}
```
public ReferredArea[] getReferredAreas(boolean recalculate)
```


يحصل على جميع الإشارات التي يشير إليها هذا الاسم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| إعادة حساب | boolean | ما إذا كان يجب إعادة حسابه إذا تم حساب هذا الاسم مسبقًا قبل هذا الاستدعاء. |

**Returns:**
com.aspose.cells.ReferredArea[] - جميع النطاقات.
### getRefersTo() {#getRefersTo--}
```
public String getRefersTo()
```


يرجع أو يعيّن الصيغة التي يُعرّف الاسم للإشارة إليها، وتبدأ بعلامة مساواة.

**Returns:**
java.lang.String
### getRefersTo(boolean isR1C1, boolean isLocal) {#getRefersTo-boolean-boolean-}
```
public String getRefersTo(boolean isR1C1, boolean isLocal)
```


احصل على مرجع هذا الاسم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isR1C1 | boolean | ما إذا كان المرجع يحتاج إلى تنسيق كـ R1C1. |
| isLocal | boolean | ما إذا كان المرجع يحتاج إلى تنسيق حسب اللغة. |

**Returns:**
java.lang.String
### getRefersTo(boolean isR1C1, boolean isLocal, int row, int column) {#getRefersTo-boolean-boolean-int-int-}
```
public String getRefersTo(boolean isR1C1, boolean isLocal, int row, int column)
```


احصل على مرجع هذا الاسم بناءً على الخلية المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isR1C1 | boolean | ما إذا كان المرجع يحتاج إلى تنسيق كـ R1C1. |
| isLocal | boolean | ما إذا كان المرجع يحتاج إلى تنسيق حسب اللغة. |
| صف | int | فهرس الصف للخلية. |
| عمود | int | فهرس العمود للخلية. |

**Returns:**
java.lang.String
### getSheetIndex() {#getSheetIndex--}
```
public int getSheetIndex()
```


يشير إلى أن هذا الاسم ينتمي إلى المصنف أو ورقة العمل. 0 = اسم عالمي، وإلا فالفهرس إلى الورقة (مبني على الواحد).

**Returns:**
int
### getText() {#getText--}
```
public String getText()
```


يحصل على نص الاسم للكائن.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isReferred() {#isReferred--}
```
public boolean isReferred()
```


يشير إلى ما إذا كان هذا الاسم مُشارًا إليه من قبل صيغ أخرى.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


يشير إلى ما إذا كان الاسم مرئيًا.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setComment(String value) {#setComment-java.lang.String-}
```
public void setComment(String value)
```


يضبط تعليق الاسم. ينطبق فقط على Excel 2007 أو الإصدارات الأحدث.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setR1C1RefersTo(String value) {#setR1C1RefersTo-java.lang.String-}
```
public void setR1C1RefersTo(String value)
```


يضبط مرجع R1C1 لـ [Name](../../com.aspose.cells/name).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setRefersTo(String value) {#setRefersTo-java.lang.String-}
```
public void setRefersTo(String value)
```


يرجع أو يعيّن الصيغة التي يُعرّف الاسم للإشارة إليها، وتبدأ بعلامة مساواة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setRefersTo(String refersTo, boolean isR1C1, boolean isLocal) {#setRefersTo-java.lang.String-boolean-boolean-}
```
public void setRefersTo(String refersTo, boolean isR1C1, boolean isLocal)
```


اضبط مرجع هذا الاسم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| refersTo | java.lang.String | المرجع. |
| isR1C1 | boolean | ما إذا كان المرجع بتنسيق R1C1. |
| isLocal | boolean | ما إذا كان المرجع مُنسقًا حسب اللغة. |

### setSheetIndex(int value) {#setSheetIndex-int-}
```
public void setSheetIndex(int value)
```


يشير إلى أن هذا الاسم ينتمي إلى المصنف أو ورقة العمل. 0 = اسم عالمي، وإلا فالفهرس إلى الورقة (مبني على الواحد).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


يحصل على نص الاسم للكائن.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


يشير إلى ما إذا كان الاسم مرئيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### toString() {#toString--}
```
public String toString()
```


يرجع سلسلة تمثل كائن النطاق الحالي.

**Returns:**
java.lang.String -
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

