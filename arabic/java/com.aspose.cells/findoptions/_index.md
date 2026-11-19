---
title: "FindOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل خيارات البحث."
type: docs
url: /ar/java/com.aspose.cells/findoptions/
---

**Inheritance:**
java.lang.Object
```
public class FindOptions
```

يمثل خيارات البحث.

**Example**

```
         //Instantiate the workbook object
         Workbook workbook = new Workbook("book1.xls");
 
         //Get Cells collection 
         Cells cells = workbook.getWorksheets().get(0).getCells();
 
         //Instantiate FindOptions Object
         FindOptions findOptions = new FindOptions();
 
         //Create a Cells Area
         CellArea ca = new CellArea();
         ca.StartRow = 8;
         ca.StartColumn = 2;
         ca.EndRow = 17;
         ca.EndColumn = 13;
 
         //Set cells area for find options
         findOptions.setRange(ca);
 
         //Set searching properties
         findOptions.setSearchBackward(false);
 
         findOptions.setSearchOrderByRows(true);
 
         findOptions.setLookInType(LookInType.VALUES);
 
         //Find the cell with 0 value
         Cell cell = cells.find(0, null, findOptions);
```
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [FindOptions()](#FindOptions--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaseSensitive()](#getCaseSensitive--) | يشير إلى ما إذا كانت السلسلة التي تم البحث عنها حساسة لحالة الأحرف. |
| [getClass()](#getClass--) |  |
| [getConvertNumericData()](#getConvertNumericData--) | يحصل على قيمة تشير إلى ما إذا كان سيتم تحويل قيمة السلسلة التي تم البحث عنها إلى بيانات رقمية. |
| [getLookAtType()](#getLookAtType--) | نوع LookAt. |
| [getLookInType()](#getLookInType--) | نوع LookIn. |
| [getRange()](#getRange--) | يحصل على النطاق الذي تم البحث فيه ويضبطه. |
| [getRegexKey()](#getRegexKey--) | يشير إلى ما إذا كان المفتاح الذي تم البحث عنه تعبيرًا نمطيًا. |
| [getSearchBackward()](#getSearchBackward--) | ما إذا كان البحث عكسيًا للخلايا. |
| [getSearchNext()](#getSearchNext--) | ترتيب البحث. |
| [getSearchOrderByRows()](#getSearchOrderByRows--) | يشير إلى ما إذا كان ترتيب البحث حسب الصفوف أو الأعمدة. |
| [getStyle()](#getStyle--) | الصيغة للبحث عنها. |
| [getValueTypeSensitive()](#getValueTypeSensitive--) | يشير إلى ما إذا كان نوع قيمة الخلية التي تم البحث عنها يجب أن يكون نفس المفتاح الذي تم البحث عنه. |
| [hashCode()](#hashCode--) |  |
| [isRangeSet()](#isRangeSet--) | يشير إلى ما إذا كان النطاق الذي تم البحث فيه محددًا. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCaseSensitive(boolean value)](#setCaseSensitive-boolean-) | يشير إلى ما إذا كانت السلسلة التي تم البحث عنها حساسة لحالة الأحرف. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | يضبط قيمة تشير إلى ما إذا كان تحويل قيمة السلسلة التي تم البحث عنها إلى بيانات رقمية. |
| [setLookAtType(int value)](#setLookAtType-int-) | نوع LookAt. |
| [setLookInType(int value)](#setLookInType-int-) | نوع LookIn. |
| [setRange(CellArea ca)](#setRange-com.aspose.cells.CellArea-) | يضبط النطاق الذي تم البحث فيه. |
| [setRegexKey(boolean value)](#setRegexKey-boolean-) | يشير إلى ما إذا كان المفتاح الذي تم البحث عنه تعبيرًا نمطيًا. |
| [setSearchBackward(boolean value)](#setSearchBackward-boolean-) | ما إذا كان البحث عكسيًا للخلايا. |
| [setSearchNext(boolean value)](#setSearchNext-boolean-) | ترتيب البحث. |
| [setSearchOrderByRows(boolean value)](#setSearchOrderByRows-boolean-) | يشير إلى ما إذا كان ترتيب البحث حسب الصفوف أو الأعمدة. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | الصيغة للبحث عنها. |
| [setValueTypeSensitive(boolean value)](#setValueTypeSensitive-boolean-) | يشير إلى ما إذا كان نوع قيمة الخلية التي تم البحث عنها يجب أن يكون نفس المفتاح الذي تم البحث عنه. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FindOptions() {#FindOptions--}
```
public FindOptions()
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
### getCaseSensitive() {#getCaseSensitive--}
```
public boolean getCaseSensitive()
```


يشير إلى ما إذا كانت السلسلة التي تم البحث عنها حساسة لحالة الأحرف.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


يحصل على قيمة تشير إلى ما إذا كان سيتم تحويل قيمة السلسلة التي تم البحث عنها إلى بيانات رقمية.

**Returns:**
boolean
### getLookAtType() {#getLookAtType--}
```
public int getLookAtType()
```


نوع LookAt.

انظر [LookAtType](../../com.aspose.cells/lookattype).

**Remarks**

عند كون [getRegexKey()](../../com.aspose.cells/findoptions\#getRegexKey--) صحيحًا وقد حدد المستخدم القاعدة الدقيقة للتعبير النمطي، من منظور الأداء يجب ضبط هذه الخاصية كـ [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT). وإلا سنعيد تشكيل مفتاح البحث لضمان أنه يمكن مطابقته وفق النوع المحدد. على سبيل المثال، عندما يكون النوع هو [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (وهذا هو القيمة الافتراضية لهذه الخاصية)، سنضيف أحرف البدل في بداية ونهاية مفتاح البحث تلقائيًا. في هذه الحالة، ستصبح التعبيرات النمطية أكثر تعقيدًا وسيقل الأداء أيضًا.

**Returns:**
int
### getLookInType() {#getLookInType--}
```
public int getLookInType()
```


نوع LookIn.

انظر [LookInType](../../com.aspose.cells/lookintype).

**Returns:**
int
### getRange() {#getRange--}
```
public CellArea getRange()
```


يحصل على النطاق الذي تم البحث فيه ويضبطه.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Returns the searched range.
### getRegexKey() {#getRegexKey--}
```
public boolean getRegexKey()
```


يشير إلى ما إذا كان المفتاح الذي تم البحث عنه تعبيرًا نمطيًا. إذا كان صحيحًا سيتم اعتبار المفتاح تعبيرًا نمطيًا وتحليله. وإلا سيتم تحليل المفتاح وفقًا للقواعد في MS Excel.

**Remarks**

على الرغم من تحديد مفتاح البحث كتعريف نمطي، قد يتم إعادة تشكيله وفقًا للـ [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--). على سبيل المثال، عندما يكون النوع هو [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (وهذا هو القيمة الافتراضية لهذه الخيارات)، ستُضاف أحرف البدل في بداية ونهاية مفتاح البحث تلقائيًا لضمان فحص المطابقة كـ \"contains\". في هذه الحالة، ستصبح التعبيرات النمطية أكثر تعقيدًا وسيقل الأداء أيضًا. لذلك، من منظور الأداء، إذا كان المستخدم قد حدد القاعدة الدقيقة للتعبير النمطي، فلا حاجة لاستخدام [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--) كقيد إضافي ويمكن للمستخدم ضبطه كـ [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT) للحصول على أداء أفضل.

**Returns:**
boolean
### getSearchBackward() {#getSearchBackward--}
```
public boolean getSearchBackward()
```


ما إذا كان البحث عكسيًا للخلايا.

**Returns:**
boolean
### getSearchNext() {#getSearchNext--}
```
public boolean getSearchNext()
```


ترتيب البحث. صحيح: البحث التالي. خطأ: البحث السابق.

**Remarks**

ملاحظة: هذا العضو أصبح الآن غير صالح. بدلاً من ذلك، يرجى استخدام الخاصية FindOptions.SearchBackward. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ نوفمبر 2018. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### getSearchOrderByRows() {#getSearchOrderByRows--}
```
public boolean getSearchOrderByRows()
```


يشير إلى ما إذا كان ترتيب البحث حسب الصفوف أو الأعمدة.

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public Style getStyle()
```


الصيغة للبحث عنها.

**Returns:**
[Style](../../com.aspose.cells/style)
### getValueTypeSensitive() {#getValueTypeSensitive--}
```
public boolean getValueTypeSensitive()
```


يشير إلى ما إذا كان نوع قيمة الخلية التي تم البحث عنها يجب أن يكون نفس المفتاح الذي تم البحث عنه.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isRangeSet() {#isRangeSet--}
```
public boolean isRangeSet()
```


يشير إلى ما إذا كان النطاق الذي تم البحث فيه محددًا.

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




### setCaseSensitive(boolean value) {#setCaseSensitive-boolean-}
```
public void setCaseSensitive(boolean value)
```


يشير إلى ما إذا كانت السلسلة التي تم البحث عنها حساسة لحالة الأحرف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان تحويل قيمة السلسلة التي تم البحث عنها إلى بيانات رقمية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setLookAtType(int value) {#setLookAtType-int-}
```
public void setLookAtType(int value)
```


نوع LookAt.

انظر [LookAtType](../../com.aspose.cells/lookattype).

**Remarks**

عند كون [getRegexKey()](../../com.aspose.cells/findoptions\#getRegexKey--) صحيحًا وقد حدد المستخدم القاعدة الدقيقة للتعبير النمطي، من منظور الأداء يجب ضبط هذه الخاصية كـ [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT). وإلا سنعيد تشكيل مفتاح البحث لضمان أنه يمكن مطابقته وفق النوع المحدد. على سبيل المثال، عندما يكون النوع هو [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (وهذا هو القيمة الافتراضية لهذه الخاصية)، سنضيف أحرف البدل في بداية ونهاية مفتاح البحث تلقائيًا. في هذه الحالة، ستصبح التعبيرات النمطية أكثر تعقيدًا وسيقل الأداء أيضًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setLookInType(int value) {#setLookInType-int-}
```
public void setLookInType(int value)
```


نوع LookIn.

انظر [LookInType](../../com.aspose.cells/lookintype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setRange(CellArea ca) {#setRange-com.aspose.cells.CellArea-}
```
public void setRange(CellArea ca)
```


يضبط النطاق الذي تم البحث فيه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | النطاق الذي تم البحث فيه. |

### setRegexKey(boolean value) {#setRegexKey-boolean-}
```
public void setRegexKey(boolean value)
```


يشير إلى ما إذا كان المفتاح الذي تم البحث عنه تعبيرًا نمطيًا. إذا كان صحيحًا سيتم اعتبار المفتاح تعبيرًا نمطيًا وتحليله. وإلا سيتم تحليل المفتاح وفقًا للقواعد في MS Excel.

**Remarks**

على الرغم من تحديد مفتاح البحث كتعريف نمطي، قد يتم إعادة تشكيله وفقًا للـ [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--). على سبيل المثال، عندما يكون النوع هو [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (وهذا هو القيمة الافتراضية لهذه الخيارات)، ستُضاف أحرف البدل في بداية ونهاية مفتاح البحث تلقائيًا لضمان فحص المطابقة كـ \"contains\". في هذه الحالة، ستصبح التعبيرات النمطية أكثر تعقيدًا وسيقل الأداء أيضًا. لذلك، من منظور الأداء، إذا كان المستخدم قد حدد القاعدة الدقيقة للتعبير النمطي، فلا حاجة لاستخدام [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--) كقيد إضافي ويمكن للمستخدم ضبطه كـ [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT) للحصول على أداء أفضل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSearchBackward(boolean value) {#setSearchBackward-boolean-}
```
public void setSearchBackward(boolean value)
```


ما إذا كان البحث عكسيًا للخلايا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSearchNext(boolean value) {#setSearchNext-boolean-}
```
public void setSearchNext(boolean value)
```


ترتيب البحث. صحيح: البحث التالي. خطأ: البحث السابق.

**Remarks**

ملاحظة: هذا العضو أصبح الآن غير صالح. بدلاً من ذلك، يرجى استخدام الخاصية FindOptions.SearchBackward. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ نوفمبر 2018. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSearchOrderByRows(boolean value) {#setSearchOrderByRows-boolean-}
```
public void setSearchOrderByRows(boolean value)
```


يشير إلى ما إذا كان ترتيب البحث حسب الصفوف أو الأعمدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


الصيغة للبحث عنها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setValueTypeSensitive(boolean value) {#setValueTypeSensitive-boolean-}
```
public void setValueTypeSensitive(boolean value)
```


يشير إلى ما إذا كان نوع قيمة الخلية التي تم البحث عنها يجب أن يكون نفس المفتاح الذي تم البحث عنه.

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

