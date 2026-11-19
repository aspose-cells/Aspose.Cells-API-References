---
title: "CopyOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل خيارات النسخ."
type: docs
url: /ar/java/com.aspose.cells/copyoptions/
---

**Inheritance:**
java.lang.Object
```
public class CopyOptions
```

يمثل خيارات النسخ.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [CopyOptions()](#CopyOptions--) | CopyOptions منشئ. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColumnCharacterWidth()](#getColumnCharacterWidth--) | يشير إلى ما إذا كان يتم نسخ عرض العمود بوحدة الأحرف. |
| [getCopyInvalidFormulasAsValues()](#getCopyInvalidFormulasAsValues--) | إذا لم تكن الصيغة صالحة للوجهة الهدف، يتم نسخ القيم فقط. |
| [getCopyNames()](#getCopyNames--) | يشير إلى ما إذا كان يتم نسخ الأسماء. |
| [getExtendToAdjacentRange()](#getExtendToAdjacentRange--) | يشير إلى ما إذا كان يتم توسيع النطاقات عند نسخ النطاق إلى النطاق المجاور. |
| [getKeepMacros()](#getKeepMacros--) | يشير إلى ما إذا كان يتم الاحتفاظ بالماكرو؛ |
| [getReferToDestinationSheet()](#getReferToDestinationSheet--) | عند نسخ النطاق في نفس الملف وإشارة المخطط إلى ورقة المصدر، يعني False أن مصدر بيانات المخطط المنسوخ لن يتغير. |
| [getReferToSheetWithSameName()](#getReferToSheetWithSameName--) | في مايكروسوفت إكسل، عند نسخ الصيغ التي تشير إلى أوراق عمل أخرى أثناء نسخ ورقة عمل إلى أخرى، يجب أن تشير الصيغ المنسوخة إلى مصنف المصدر. |
| [getUpdateInvalidReferencesToTargetSheet()](#getUpdateInvalidReferencesToTargetSheet--) | يشير إلى ما إذا كان يجب الإشارة إلى ورقة العمل الهدف إذا لم يتم نسخ ورقة العمل المشار إليها. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColumnCharacterWidth(boolean value)](#setColumnCharacterWidth-boolean-) | يشير إلى ما إذا كان يتم نسخ عرض العمود بوحدة الأحرف. |
| [setCopyInvalidFormulasAsValues(boolean value)](#setCopyInvalidFormulasAsValues-boolean-) | إذا لم تكن الصيغة صالحة للوجهة الهدف، يتم نسخ القيم فقط. |
| [setCopyNames(boolean value)](#setCopyNames-boolean-) | يشير إلى ما إذا كان يتم نسخ الأسماء. |
| [setExtendToAdjacentRange(boolean value)](#setExtendToAdjacentRange-boolean-) | يشير إلى ما إذا كان يتم توسيع النطاقات عند نسخ النطاق إلى النطاق المجاور. |
| [setKeepMacros(boolean value)](#setKeepMacros-boolean-) | يشير إلى ما إذا كان يتم الاحتفاظ بالماكرو؛ |
| [setReferToDestinationSheet(boolean value)](#setReferToDestinationSheet-boolean-) | عند نسخ النطاق في نفس الملف وإشارة المخطط إلى ورقة المصدر، يعني False أن مصدر بيانات المخطط المنسوخ لن يتغير. |
| [setReferToSheetWithSameName(boolean value)](#setReferToSheetWithSameName-boolean-) | في مايكروسوفت إكسل، عند نسخ الصيغ التي تشير إلى أوراق عمل أخرى أثناء نسخ ورقة عمل إلى أخرى، يجب أن تشير الصيغ المنسوخة إلى مصنف المصدر. |
| [setUpdateInvalidReferencesToTargetSheet(boolean value)](#setUpdateInvalidReferencesToTargetSheet-boolean-) | يشير إلى ما إذا كان يجب الإشارة إلى ورقة العمل الهدف إذا لم يتم نسخ ورقة العمل المشار إليها. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CopyOptions() {#CopyOptions--}
```
public CopyOptions()
```


CopyOptions منشئ.

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
### getColumnCharacterWidth() {#getColumnCharacterWidth--}
```
public boolean getColumnCharacterWidth()
```


يشير إلى ما إذا كان يتم نسخ عرض العمود بوحدة الأحرف.

**Returns:**
boolean
### getCopyInvalidFormulasAsValues() {#getCopyInvalidFormulasAsValues--}
```
public boolean getCopyInvalidFormulasAsValues()
```


إذا لم تكن الصيغة صالحة للوجهة الهدف، يتم نسخ القيم فقط.

**Returns:**
boolean
### getCopyNames() {#getCopyNames--}
```
public boolean getCopyNames()
```


يشير إلى ما إذا كان يتم نسخ الأسماء.

**Returns:**
boolean
### getExtendToAdjacentRange() {#getExtendToAdjacentRange--}
```
public boolean getExtendToAdjacentRange()
```


يشير إلى ما إذا كان يتم توسيع النطاقات عند نسخ النطاق إلى النطاق المجاور.

**Remarks**

إذا كان True، يتم فقط توسيع نطاق الارتباط التشعبي دون إضافة ارتباط تشعبي جديد عند نسخ الارتباطات التشعبية إلى الصفوف المجاورة.

**Returns:**
boolean
### getKeepMacros() {#getKeepMacros--}
```
public boolean getKeepMacros()
```


يشير إلى ما إذا كان يتم الاحتفاظ بالماكرو؛

**Remarks**

فقط لنسخ المصنف.

**Returns:**
boolean
### getReferToDestinationSheet() {#getReferToDestinationSheet--}
```
public boolean getReferToDestinationSheet()
```


عند نسخ النطاق في نفس الملف وإشارة المخطط إلى ورقة المصدر، يعني False أن مصدر بيانات المخطط المنسوخ لن يتغير. يعني True أن مصدر بيانات المخطط المنسوخ يشير إلى ورقة الوجهة.

**Remarks**

القيمة الافتراضية هي false، وتعمل كما في مايكروسوفت إكسل. على سبيل المثال: إذا تم نسخ مخطط بمصدر البيانات \"sheet1!A1:B10\" من ورقة العمل \"sheet1 إلى ورقة عمل أخرى \"sheet2\"، سيتغير مصدر البيانات إلى \"sheet2!A1:B10\".

**Returns:**
boolean
### getReferToSheetWithSameName() {#getReferToSheetWithSameName--}
```
public boolean getReferToSheetWithSameName()
```


في مايكروسوفت إكسل، عند نسخ الصيغ التي تشير إلى أوراق عمل أخرى أثناء نسخ ورقة عمل إلى أخرى، يجب أن تشير الصيغ المنسوخة إلى مصنف المصدر. ومع ذلك، في بعض الحالات قد يحتاج المستخدم إلى أن تشير الصيغ المنسوخة إلى أوراق عمل بنفس الاسم في نفس المصنف، مثل عندما تكون تلك الأوراق قد تم نسخها قبل عملية النسخ هذه، عندها يجب إبقاء هذه الخاصية على true.

**Remarks**

القيمة الافتراضية هي true.

**Returns:**
boolean
### getUpdateInvalidReferencesToTargetSheet() {#getUpdateInvalidReferencesToTargetSheet--}
```
public boolean getUpdateInvalidReferencesToTargetSheet()
```


يشير إلى ما إذا كان يجب الإشارة إلى ورقة العمل الهدف إذا لم يتم نسخ ورقة العمل المشار إليها.

**Remarks**

يعمل فقط عند نسخ نطاق أو ورقة عمل من مصنف آخر.

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




### setColumnCharacterWidth(boolean value) {#setColumnCharacterWidth-boolean-}
```
public void setColumnCharacterWidth(boolean value)
```


يشير إلى ما إذا كان يتم نسخ عرض العمود بوحدة الأحرف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCopyInvalidFormulasAsValues(boolean value) {#setCopyInvalidFormulasAsValues-boolean-}
```
public void setCopyInvalidFormulasAsValues(boolean value)
```


إذا لم تكن الصيغة صالحة للوجهة الهدف، يتم نسخ القيم فقط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCopyNames(boolean value) {#setCopyNames-boolean-}
```
public void setCopyNames(boolean value)
```


يشير إلى ما إذا كان يتم نسخ الأسماء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExtendToAdjacentRange(boolean value) {#setExtendToAdjacentRange-boolean-}
```
public void setExtendToAdjacentRange(boolean value)
```


يشير إلى ما إذا كان يتم توسيع النطاقات عند نسخ النطاق إلى النطاق المجاور.

**Remarks**

إذا كان True، يتم فقط توسيع نطاق الارتباط التشعبي دون إضافة ارتباط تشعبي جديد عند نسخ الارتباطات التشعبية إلى الصفوف المجاورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setKeepMacros(boolean value) {#setKeepMacros-boolean-}
```
public void setKeepMacros(boolean value)
```


يشير إلى ما إذا كان يتم الاحتفاظ بالماكرو؛

**Remarks**

فقط لنسخ المصنف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setReferToDestinationSheet(boolean value) {#setReferToDestinationSheet-boolean-}
```
public void setReferToDestinationSheet(boolean value)
```


عند نسخ النطاق في نفس الملف وإشارة المخطط إلى ورقة المصدر، يعني False أن مصدر بيانات المخطط المنسوخ لن يتغير. يعني True أن مصدر بيانات المخطط المنسوخ يشير إلى ورقة الوجهة.

**Remarks**

القيمة الافتراضية هي false، وتعمل كما في مايكروسوفت إكسل. على سبيل المثال: إذا تم نسخ مخطط بمصدر البيانات \"sheet1!A1:B10\" من ورقة العمل \"sheet1 إلى ورقة عمل أخرى \"sheet2\"، سيتغير مصدر البيانات إلى \"sheet2!A1:B10\".

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setReferToSheetWithSameName(boolean value) {#setReferToSheetWithSameName-boolean-}
```
public void setReferToSheetWithSameName(boolean value)
```


في مايكروسوفت إكسل، عند نسخ الصيغ التي تشير إلى أوراق عمل أخرى أثناء نسخ ورقة عمل إلى أخرى، يجب أن تشير الصيغ المنسوخة إلى مصنف المصدر. ومع ذلك، في بعض الحالات قد يحتاج المستخدم إلى أن تشير الصيغ المنسوخة إلى أوراق عمل بنفس الاسم في نفس المصنف، مثل عندما تكون تلك الأوراق قد تم نسخها قبل عملية النسخ هذه، عندها يجب إبقاء هذه الخاصية على true.

**Remarks**

القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setUpdateInvalidReferencesToTargetSheet(boolean value) {#setUpdateInvalidReferencesToTargetSheet-boolean-}
```
public void setUpdateInvalidReferencesToTargetSheet(boolean value)
```


يشير إلى ما إذا كان يجب الإشارة إلى ورقة العمل الهدف إذا لم يتم نسخ ورقة العمل المشار إليها.

**Remarks**

يعمل فقط عند نسخ نطاق أو ورقة عمل من مصنف آخر.

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

