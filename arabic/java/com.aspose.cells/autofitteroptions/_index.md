---
title: "AutoFitterOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل جميع خيارات التلائم التلقائي."
type: docs
url: /ar/java/com.aspose.cells/autofitteroptions/
---

**Inheritance:**
java.lang.Object
```
public class AutoFitterOptions
```

يمثل جميع خيارات التلائم التلقائي.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [AutoFitterOptions()](#AutoFitterOptions--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFitMergedCells()](#getAutoFitMergedCells--) | يشير إلى ما إذا كان يتم ضبط ارتفاع الصف تلقائيًا عندما يتم دمج الخلايا في صف. |
| [getAutoFitMergedCellsType()](#getAutoFitMergedCellsType--) | يحصل على نوع ضبط ارتفاع الصف تلقائيًا للخلايا المدمجة. |
| [getAutoFitWrappedTextType()](#getAutoFitWrappedTextType--) | يحصل على نوع ضبط النص الملتف تلقائيًا. |
| [getClass()](#getClass--) |  |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | يحصل على لغة التحرير الافتراضية. |
| [getForRendering()](#getForRendering--) | يشير إلى ما إذا كان الضبط لأغراض العرض. |
| [getFormatStrategy()](#getFormatStrategy--) | يحصل على استراتيجية التنسيق. |
| [getIgnoreHidden()](#getIgnoreHidden--) | يتجاهل الصفوف/الأعمدة المخفية. |
| [getMaxRowHeight()](#getMaxRowHeight--) | يحصل على الحد الأقصى لارتفاع الصف (بوحدة النقطة) عند ضبط الصفوف تلقائيًا. |
| [getOnlyAuto()](#getOnlyAuto--) | يشير إلى ما إذا كان يتم تعديل ارتفاع الصفوف فقط التي لم يتم تخصيص ارتفاعها. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFitMergedCells(boolean value)](#setAutoFitMergedCells-boolean-) | يشير إلى ما إذا كان يتم ضبط ارتفاع الصف تلقائيًا عندما يتم دمج الخلايا في صف. |
| [setAutoFitMergedCellsType(int value)](#setAutoFitMergedCellsType-int-) | يضبط نوع تعديل ارتفاع الصف تلقائيًا للخلايا المدمجة. |
| [setAutoFitWrappedTextType(int value)](#setAutoFitWrappedTextType-int-) | يضبط نوع تعديل النص الملتف تلقائيًا. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | يضبط لغة التحرير الافتراضية. |
| [setForRendering(boolean value)](#setForRendering-boolean-) | يشير إلى ما إذا كان الضبط لأغراض العرض. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | يضبط استراتيجية التنسيق. |
| [setIgnoreHidden(boolean value)](#setIgnoreHidden-boolean-) | يتجاهل الصفوف/الأعمدة المخفية. |
| [setMaxRowHeight(double value)](#setMaxRowHeight-double-) | يضبط الحد الأقصى لارتفاع الصف (بوحدة النقطة) عند تعديل ارتفاع الصفوف تلقائيًا. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | يشير إلى ما إذا كان يتم تعديل ارتفاع الصفوف فقط التي لم يتم تخصيص ارتفاعها. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AutoFitterOptions() {#AutoFitterOptions--}
```
public AutoFitterOptions()
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
### getAutoFitMergedCells() {#getAutoFitMergedCells--}
```
public boolean getAutoFitMergedCells()
```


يشير إلى ما إذا كان يتم تعديل ارتفاع الصف تلقائيًا عندما تكون الخلايا مدمجة في صف. القيمة الافتراضية هي false.

**Remarks**

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام الخاصية AutoFitterOptions.AutoFitMergedCellsType. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2018. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### getAutoFitMergedCellsType() {#getAutoFitMergedCellsType--}
```
public int getAutoFitMergedCellsType()
```


يحصل على نوع ضبط ارتفاع الصف تلقائيًا للخلايا المدمجة.

انظر [AutoFitMergedCellsType](../../com.aspose.cells/autofitmergedcellstype).

**Remarks**

يتم تجاهل الخلايا المدمجة افتراضيًا في Excel عند تعديل ارتفاع الصف، لذا يعمل Aspose.Cells وفقًا للإعداد الافتراضي لـ MS Excel. يرجى ضبط هذا النوع لتغيير طريقة تعديل ارتفاع الصف تلقائيًا للخلايا المدمجة.

**Returns:**
int
### getAutoFitWrappedTextType() {#getAutoFitWrappedTextType--}
```
public int getAutoFitWrappedTextType()
```


يحصل على نوع ضبط النص الملتف تلقائيًا.

انظر [AutoFitWrappedTextType](../../com.aspose.cells/autofitwrappedtexttype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


يحصل على لغة التحرير الافتراضية.

انظر [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

قد يعرض/يُصوّر تخطيطات مختلفة لفقرة النص عندما يتم تعيين لغات تحرير مختلفة. القيمة الافتراضية هي [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Returns:**
int
### getForRendering() {#getForRendering--}
```
public boolean getForRendering()
```


يشير إلى ما إذا كان الضبط لأغراض العرض.

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


يحصل على استراتيجية التنسيق.

انظر [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

القيمة الافتراضية هي CellStyle للأداء.

**Returns:**
int
### getIgnoreHidden() {#getIgnoreHidden--}
```
public boolean getIgnoreHidden()
```


يتجاهل الصفوف/الأعمدة المخفية.

**Returns:**
boolean
### getMaxRowHeight() {#getMaxRowHeight--}
```
public double getMaxRowHeight()
```


يحصل على الحد الأقصى لارتفاع الصف (بوحدة النقطة) عند ضبط الصفوف تلقائيًا.

**Returns:**
double
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


يشير إلى ما إذا كان يتم تعديل ارتفاع الصفوف فقط التي لم يتم تخصيص ارتفاعها.

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




### setAutoFitMergedCells(boolean value) {#setAutoFitMergedCells-boolean-}
```
public void setAutoFitMergedCells(boolean value)
```


يشير إلى ما إذا كان يتم تعديل ارتفاع الصف تلقائيًا عندما تكون الخلايا مدمجة في صف. القيمة الافتراضية هي false.

**Remarks**

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام الخاصية AutoFitterOptions.AutoFitMergedCellsType. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2018. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAutoFitMergedCellsType(int value) {#setAutoFitMergedCellsType-int-}
```
public void setAutoFitMergedCellsType(int value)
```


يضبط نوع تعديل ارتفاع الصف تلقائيًا للخلايا المدمجة.

انظر [AutoFitMergedCellsType](../../com.aspose.cells/autofitmergedcellstype).

**Remarks**

يتم تجاهل الخلايا المدمجة افتراضيًا في Excel عند تعديل ارتفاع الصف، لذا يعمل Aspose.Cells وفقًا للإعداد الافتراضي لـ MS Excel. يرجى ضبط هذا النوع لتغيير طريقة تعديل ارتفاع الصف تلقائيًا للخلايا المدمجة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setAutoFitWrappedTextType(int value) {#setAutoFitWrappedTextType-int-}
```
public void setAutoFitWrappedTextType(int value)
```


يضبط نوع تعديل النص الملتف تلقائيًا.

انظر [AutoFitWrappedTextType](../../com.aspose.cells/autofitwrappedtexttype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


يضبط لغة التحرير الافتراضية.

انظر [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

قد يعرض/يُصوّر تخطيطات مختلفة لفقرة النص عندما يتم تعيين لغات تحرير مختلفة. القيمة الافتراضية هي [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setForRendering(boolean value) {#setForRendering-boolean-}
```
public void setForRendering(boolean value)
```


يشير إلى ما إذا كان الضبط لأغراض العرض.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


يضبط استراتيجية التنسيق.

انظر [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

القيمة الافتراضية هي CellStyle للأداء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setIgnoreHidden(boolean value) {#setIgnoreHidden-boolean-}
```
public void setIgnoreHidden(boolean value)
```


يتجاهل الصفوف/الأعمدة المخفية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setMaxRowHeight(double value) {#setMaxRowHeight-double-}
```
public void setMaxRowHeight(double value)
```


يضبط الحد الأقصى لارتفاع الصف (بوحدة النقطة) عند تعديل ارتفاع الصفوف تلقائيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


يشير إلى ما إذا كان يتم تعديل ارتفاع الصفوف فقط التي لم يتم تخصيص ارتفاعها.

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

