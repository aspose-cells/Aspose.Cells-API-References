---
title: "DeleteBlankOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل إعداد حذف الخلايا/الصفوف/الأعمدة الفارغة."
type: docs
url: /ar/java/com.aspose.cells/deleteblankoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.DeleteOptions](../../com.aspose.cells/deleteoptions)
```
public class DeleteBlankOptions extends DeleteOptions
```

يمثل إعداد حذف الخلايا/الصفوف/الأعمدة الفارغة.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [DeleteBlankOptions()](#DeleteBlankOptions--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDrawingsAsBlank()](#getDrawingsAsBlank--) | يشير إلى ما إذا كانت الكائنات المتعلقة بالرسم مثل الصورة، الشكل، المخطط... ستُعامل كفارغة. |
| [getEmptyFormulaValueAsBlank()](#getEmptyFormulaValueAsBlank--) | ما إذا كانت الخلية الواحدة ستُعامل كفارغة عندما تكون صيغة والنتيجة المحسوبة هي null أو سلسلة فارغة. |
| [getEmptyStringAsBlank()](#getEmptyStringAsBlank--) | يشير إلى ما إذا كانت الخلية الواحدة ستُعامل كفارغة عندما تكون قيمتها سلسلة فارغة. |
| [getEndIndex()](#getEndIndex--) | يحدد فهرس الصف/العمود النهائي (شامل) للنطاق الذي سيتم فحصه وحذف الصفوف/الأعمدة الفارغة. |
| [getFormulaChangeMonitor()](#getFormulaChangeMonitor--) | يحصل على المراقب لتتبع التغييرات الناتجة عن الحذف. |
| [getMergedCellsShrinkType()](#getMergedCellsShrinkType--) | يشير إلى كيفية معالجة الخلايا المدمجة عند حذف الصفوف/الأعمدة الفارغة. |
| [getStartIndex()](#getStartIndex--) | يحدد فهرس الصف/العمود الابتدائي للنطاق الذي سيتم فحصه وحذف الصف/العمود الفارغ. |
| [getUpdateReference()](#getUpdateReference--) | يشير إلى ما إذا كان سيتم تحديث المراجع في أوراق العمل الأخرى. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDrawingsAsBlank(boolean value)](#setDrawingsAsBlank-boolean-) | يشير إلى ما إذا كانت الكائنات المتعلقة بالرسم مثل الصورة، الشكل، المخطط... ستُعامل كفارغة. |
| [setEmptyFormulaValueAsBlank(boolean value)](#setEmptyFormulaValueAsBlank-boolean-) | ما إذا كانت الخلية الواحدة ستُعامل كفارغة عندما تكون صيغة والنتيجة المحسوبة هي null أو سلسلة فارغة. |
| [setEmptyStringAsBlank(boolean value)](#setEmptyStringAsBlank-boolean-) | يشير إلى ما إذا كانت الخلية الواحدة ستُعامل كفارغة عندما تكون قيمتها سلسلة فارغة. |
| [setEndIndex(int value)](#setEndIndex-int-) | يحدد فهرس الصف/العمود النهائي (شامل) للنطاق الذي سيتم فحصه وحذف الصفوف/الأعمدة الفارغة. |
| [setFormulaChangeMonitor(AbstractFormulaChangeMonitor value)](#setFormulaChangeMonitor-com.aspose.cells.AbstractFormulaChangeMonitor-) | يضبط المراقب لتتبع التغييرات الناتجة عن الحذف. |
| [setMergedCellsShrinkType(int value)](#setMergedCellsShrinkType-int-) | يشير إلى كيفية معالجة الخلايا المدمجة عند حذف الصفوف/الأعمدة الفارغة. |
| [setStartIndex(int value)](#setStartIndex-int-) | يحدد فهرس الصف/العمود الابتدائي للنطاق الذي سيتم فحصه وحذف الصف/العمود الفارغ. |
| [setUpdateReference(boolean value)](#setUpdateReference-boolean-) | يشير إلى ما إذا كان سيتم تحديث المراجع في أوراق العمل الأخرى. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DeleteBlankOptions() {#DeleteBlankOptions--}
```
public DeleteBlankOptions()
```


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
### getDrawingsAsBlank() {#getDrawingsAsBlank--}
```
public boolean getDrawingsAsBlank()
```


يشير إلى ما إذا كانت الكائنات المتعلقة بالرسم مثل الصورة، الشكل، المخطط... ستُعامل كفارغة. القيمة الافتراضية هي true.

**Remarks**

عند ضبط هذه الخاصية على false، جميع الصفوف/الأعمدة التي تغطيها كائنات الرسم لن تُعامل كفارغة ولن يتم حذفها.

**Returns:**
boolean
### getEmptyFormulaValueAsBlank() {#getEmptyFormulaValueAsBlank--}
```
public boolean getEmptyFormulaValueAsBlank()
```


ما إذا كان سيتم اعتبار خلية واحدة فارغة عندما تكون صيغة والنتيجة المحسوبة هي null أو سلسلة فارغة. القيمة الافتراضية هي false.

**Remarks**

بشكل عام يجب على المستخدم التأكد من أن الصيغ قد تم حسابها قبل عملية الحذف مع ضبط هذه الخاصية إلى true. وإلا فإن جميع الصيغ التي تم إنشاؤها حديثًا بواسطة واجهات برمجة التطبيقات العادية مثل [Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--) سيتم اعتبارها فارغة وقد تُحذف لأن نتائجها المحسوبة قبل الحساب هي جميعها null.

**Returns:**
boolean
### getEmptyStringAsBlank() {#getEmptyStringAsBlank--}
```
public boolean getEmptyStringAsBlank()
```


يشير إلى ما إذا كان سيتم اعتبار خلية واحدة فارغة عندما تكون قيمتها سلسلة فارغة. القيمة الافتراضية هي true.

**Returns:**
boolean
### getEndIndex() {#getEndIndex--}
```
public int getEndIndex()
```


يحدد فهرس الصف/العمود النهائي (شامل) للنطاق الذي يتم فحصه وحذف الصفوف/الأعمدة الفارغة. القيمة الافتراضية هي -1 و -1 تعني النطاق الأقصى لجميع الكائنات (الخلايا، الرسومات، ...) التي تحتاج إلى الفحص.

**Returns:**
int
### getFormulaChangeMonitor() {#getFormulaChangeMonitor--}
```
public AbstractFormulaChangeMonitor getFormulaChangeMonitor()
```


يحصل على المراقب لتتبع التغييرات الناتجة عن الحذف.

**Returns:**
[AbstractFormulaChangeMonitor](../../com.aspose.cells/abstractformulachangemonitor)
### getMergedCellsShrinkType() {#getMergedCellsShrinkType--}
```
public int getMergedCellsShrinkType()
```


يشير إلى كيفية معالجة الخلايا المدمجة عند حذف الصفوف/الأعمدة الفارغة.

انظر [MergedCellsShrinkType](../../com.aspose.cells/mergedcellsshrinktype).

**Remarks**

بالنسبة إلى [MergedCellsShrinkType.KEEP\_HEADER\_ONLY](../../com.aspose.cells/mergedcellsshrinktype\#KEEP-HEADER-ONLY)، سيتم اعتبار جميع الخلايا فيه فارغة باستثناء الخلية العلوية اليسرى غير الفارغة. وهي القيمة الافتراضية لهذه الخاصية.

بالنسبة إلى [MergedCellsShrinkType.NONE](../../com.aspose.cells/mergedcellsshrinktype\#NONE)، سيتم اعتبار جميع الخلايا فيه غير فارغة.

بالنسبة إلى [MergedCellsShrinkType.SHRINK\_TO\_FIT](../../com.aspose.cells/mergedcellsshrinktype\#SHRINK-TO-FIT)، سيتم اعتبار جميع الخلايا خارج منطقة عرض المحتوى فارغة.



**Returns:**
int
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


يحدد فهرس الصف/العمود الابتدائي للنطاق الذي سيتم فحصه وحذف الصف/العمود الفارغ.

**Returns:**
int
### getUpdateReference() {#getUpdateReference--}
```
public boolean getUpdateReference()
```


يشير إلى ما إذا كان سيتم تحديث المراجع في أوراق العمل الأخرى.

**Remarks**

بدءًا من الإصدار 26.7 قمنا بتعيين القيمة الافتراضية لهذه الخاصية إلى true.

**Returns:**
boolean
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




### setDrawingsAsBlank(boolean value) {#setDrawingsAsBlank-boolean-}
```
public void setDrawingsAsBlank(boolean value)
```


يشير إلى ما إذا كانت الكائنات المتعلقة بالرسم مثل الصورة، الشكل، المخطط... ستُعامل كفارغة. القيمة الافتراضية هي true.

**Remarks**

عند ضبط هذه الخاصية على false، جميع الصفوف/الأعمدة التي تغطيها كائنات الرسم لن تُعامل كفارغة ولن يتم حذفها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEmptyFormulaValueAsBlank(boolean value) {#setEmptyFormulaValueAsBlank-boolean-}
```
public void setEmptyFormulaValueAsBlank(boolean value)
```


ما إذا كان سيتم اعتبار خلية واحدة فارغة عندما تكون صيغة والنتيجة المحسوبة هي null أو سلسلة فارغة. القيمة الافتراضية هي false.

**Remarks**

بشكل عام يجب على المستخدم التأكد من أن الصيغ قد تم حسابها قبل عملية الحذف مع ضبط هذه الخاصية إلى true. وإلا فإن جميع الصيغ التي تم إنشاؤها حديثًا بواسطة واجهات برمجة التطبيقات العادية مثل [Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--) سيتم اعتبارها فارغة وقد تُحذف لأن نتائجها المحسوبة قبل الحساب هي جميعها null.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEmptyStringAsBlank(boolean value) {#setEmptyStringAsBlank-boolean-}
```
public void setEmptyStringAsBlank(boolean value)
```


يشير إلى ما إذا كان سيتم اعتبار خلية واحدة فارغة عندما تكون قيمتها سلسلة فارغة. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEndIndex(int value) {#setEndIndex-int-}
```
public void setEndIndex(int value)
```


يحدد فهرس الصف/العمود النهائي (شامل) للنطاق الذي يتم فحصه وحذف الصفوف/الأعمدة الفارغة. القيمة الافتراضية هي -1 و -1 تعني النطاق الأقصى لجميع الكائنات (الخلايا، الرسومات، ...) التي تحتاج إلى الفحص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setFormulaChangeMonitor(AbstractFormulaChangeMonitor value) {#setFormulaChangeMonitor-com.aspose.cells.AbstractFormulaChangeMonitor-}
```
public void setFormulaChangeMonitor(AbstractFormulaChangeMonitor value)
```


يضبط المراقب لتتبع التغييرات الناتجة عن الحذف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [AbstractFormulaChangeMonitor](../../com.aspose.cells/abstractformulachangemonitor) |  |

### setMergedCellsShrinkType(int value) {#setMergedCellsShrinkType-int-}
```
public void setMergedCellsShrinkType(int value)
```


يشير إلى كيفية معالجة الخلايا المدمجة عند حذف الصفوف/الأعمدة الفارغة.

انظر [MergedCellsShrinkType](../../com.aspose.cells/mergedcellsshrinktype).

**Remarks**

بالنسبة إلى [MergedCellsShrinkType.KEEP\_HEADER\_ONLY](../../com.aspose.cells/mergedcellsshrinktype\#KEEP-HEADER-ONLY)، سيتم اعتبار جميع الخلايا فيه فارغة باستثناء الخلية العلوية اليسرى غير الفارغة. وهي القيمة الافتراضية لهذه الخاصية.

بالنسبة إلى [MergedCellsShrinkType.NONE](../../com.aspose.cells/mergedcellsshrinktype\#NONE)، سيتم اعتبار جميع الخلايا فيه غير فارغة.

بالنسبة إلى [MergedCellsShrinkType.SHRINK\_TO\_FIT](../../com.aspose.cells/mergedcellsshrinktype\#SHRINK-TO-FIT)، سيتم اعتبار جميع الخلايا خارج منطقة عرض المحتوى فارغة.



**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setStartIndex(int value) {#setStartIndex-int-}
```
public void setStartIndex(int value)
```


يحدد فهرس الصف/العمود الابتدائي للنطاق الذي سيتم فحصه وحذف الصف/العمود الفارغ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setUpdateReference(boolean value) {#setUpdateReference-boolean-}
```
public void setUpdateReference(boolean value)
```


يشير إلى ما إذا كان سيتم تحديث المراجع في أوراق العمل الأخرى.

**Remarks**

بدءًا من الإصدار 26.7 قمنا بتعيين القيمة الافتراضية لهذه الخاصية إلى true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

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

