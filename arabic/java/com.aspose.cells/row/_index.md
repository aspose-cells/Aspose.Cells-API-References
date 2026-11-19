---
title: "Row"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل صفًا واحدًا في ورقة العمل."
type: docs
url: /ar/java/com.aspose.cells/row/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Row implements Iterable
```

يمثل صفًا واحدًا في ورقة العمل.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Style style = workbook.createStyle();
 
         //Setting the background color to Blue
         style.setBackgroundColor(Color.getBlue());
 
         //Setting the foreground color to Red
         style.setForegroundColor(Color.getRed());
 
         //setting Background Pattern
         style.setPattern(BackgroundType.DIAGONAL_STRIPE);
 
         //New Style Flag
         StyleFlag styleFlag = new StyleFlag();
 
         //Set All Styles
         styleFlag.setAll(true);
 
          //Get first row
         Row row = worksheet.getCells().getRows().get(0);
          //Apply Style to first row
         row.applyStyle(style, styleFlag);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | يطبق التنسيقات على صف كامل. |
| [copySettings(Row source, boolean checkStyle)](#copySettings-com.aspose.cells.Row-boolean-) | نسخ إعدادات الصف، مثل النمط، الارتفاع، الإظهار، ... إلخ. |
| [equals(Row row)](#equals-com.aspose.cells.Row-) | يتحقق مما إذا كان هذا الكائن يشير إلى نفس الصف مع كائن صف آخر. |
| [equals(Object obj)](#equals-java.lang.Object-) | يتحقق مما إذا كان هذا الكائن يشير إلى نفس الصف مع آخر. |
| [get(int column)](#get-int-) | يحصل على الخلية. |
| [getCellByIndex(int index)](#getCellByIndex-int-) | احصل على الخلية بواسطة فهرس محدد في مجموعة الخلايا لهذا الصف. |
| [getCellOrNull(int column)](#getCellOrNull-int-) | يحصل على الخلية أو null في الفهرس المحدد. |
| [getClass()](#getClass--) |  |
| [getFirstCell()](#getFirstCell--) | يحصل على أول كائن خلية في الصف. |
| [getFirstDataCell()](#getFirstDataCell--) | يحصل على أول خلية غير فارغة في الصف. |
| [getGroupLevel()](#getGroupLevel--) | يحصل على مستوى المجموعة للصف. |
| [getHeight()](#getHeight--) | يحصل على ارتفاع الصف بوحدة النقاط. |
| [getIndex()](#getIndex--) | يحصل على فهرس هذا الصف. |
| [getLastCell()](#getLastCell--) | يحصل على آخر كائن خلية في الصف. |
| [getLastDataCell()](#getLastDataCell--) | يحصل على آخر خلية غير فارغة في الصف. |
| [getStyle()](#getStyle--) | يحصل على نمط هذا الصف. |
| [hasCustomStyle()](#hasCustomStyle--) | يشير إلى ما إذا كان هذا الصف يحتوي على إعدادات نمط مخصصة (مختلفة عن الإعداد الافتراضي الموروث من دفتر العمل). |
| [hashCode()](#hashCode--) |  |
| [isBlank()](#isBlank--) | يشير إلى ما إذا كان الصف يحتوي على أي بيانات |
| [isCollapsed()](#isCollapsed--) | ما إذا كان الصف مُطوى |
| [isHeightMatched()](#isHeightMatched--) | يشير إلى ما إذا كان ارتفاع الصف يتطابق مع إعداد الخط الافتراضي الحالي لدفتر العمل. |
| [isHidden()](#isHidden--) | يشير إلى ما إذا كان الصف مخفيًا. |
| [iterator()](#iterator--) | يحصل على مُعدِّد الخلايا |
| [iterator(boolean reversed, boolean sync)](#iterator-boolean-boolean-) | يحصل على مُعدِّد يتنقل عبر الخلايا في هذا الصف. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | ما إذا كان الصف مُطوى |
| [setGroupLevel(byte value)](#setGroupLevel-byte-) | يحصل على مستوى المجموعة للصف. |
| [setHeight(double value)](#setHeight-double-) | يضبط ارتفاع الصف بوحدة النقاط. |
| [setHeightMatched(boolean value)](#setHeightMatched-boolean-) | يشير إلى ما إذا كان ارتفاع الصف يتطابق مع إعداد الخط الافتراضي الحالي لدفتر العمل. |
| [setHidden(boolean value)](#setHidden-boolean-) | يشير إلى ما إذا كان الصف مخفيًا. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | يضبط نمط هذا الصف. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


يطبق التنسيقات على صف كامل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | كائن النمط الذي سيتم تطبيقه. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | علامات تشير إلى خصائص التنسيق المطبقة. |

### copySettings(Row source, boolean checkStyle) {#copySettings-com.aspose.cells.Row-boolean-}
```
public void copySettings(Row source, boolean checkStyle)
```


نسخ إعدادات الصف، مثل النمط، الارتفاع، الإظهار، ... إلخ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | [Row](../../com.aspose.cells/row) | صف المصدر الذي ستُنسخ إعداداته إلى هذا الصف |
| checkStyle | boolean | ما إذا كان يتم فحص وتجميع النمط. لا يُطبق إلا ويكون ضرورياً عندما ينتمي كائنان من الصف إلى دفتر عملين مختلفين وتكون أنماط دفترَي العمل مختلفتين. |

### equals(Row row) {#equals-com.aspose.cells.Row-}
```
public boolean equals(Row row)
```


يتحقق مما إذا كان هذا الكائن يشير إلى نفس الصف مع كائن صف آخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | كائن صف آخر |

**Returns:**
منطقي - true إذا كان كائنان من الصف يشيران إلى نفس الصف.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


يتحقق مما إذا كان هذا الكائن يشير إلى نفس الصف مع آخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | java.lang.Object | كائن آخر |

**Returns:**
منطقي - true إذا كان كائنان يشيران إلى نفس الصف.
### get(int column) {#get-int-}
```
public Cell get(int column)
```


يحصل على الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | مؤشر العمود |

**Returns:**
[Cell](../../com.aspose.cells/cell) - 
### getCellByIndex(int index) {#getCellByIndex-int-}
```
public Cell getCellByIndex(int index)
```


احصل على الخلية بواسطة فهرس محدد في مجموعة الخلايا لهذا الصف.

**Remarks**

للتنقل عبر جميع الخلايا بالتسلسل دون تعديل، سيؤدي استخدام [iterator()](../../com.aspose.cells/row\#iterator--) إلى أداء أفضل مقارنةً باستخدام هذه الطريقة للحصول على الخلية واحدة تلو الأخرى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس (الموقع) للخلية في مجموعة الخلايا لهذا الصف. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - The Cell object at given position.
### getCellOrNull(int column) {#getCellOrNull-int-}
```
public Cell getCellOrNull(int column)
```


يحصل على الخلية أو null في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | مؤشر العمود |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Returns the cell object if the cell exists. Or returns null if the cell object does not exist.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFirstCell() {#getFirstCell--}
```
public Cell getFirstCell()
```


يحصل على أول كائن خلية في الصف.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getFirstDataCell() {#getFirstDataCell--}
```
public Cell getFirstDataCell()
```


يحصل على أول خلية غير فارغة في الصف.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getGroupLevel() {#getGroupLevel--}
```
public byte getGroupLevel()
```


يحصل على مستوى المجموعة للصف.

**Returns:**
byte
### getHeight() {#getHeight--}
```
public double getHeight()
```


يحصل على ارتفاع الصف بوحدة النقاط.

**Returns:**
double
### getIndex() {#getIndex--}
```
public int getIndex()
```


يحصل على فهرس هذا الصف.

**Returns:**
int
### getLastCell() {#getLastCell--}
```
public Cell getLastCell()
```


يحصل على آخر كائن خلية في الصف.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getLastDataCell() {#getLastDataCell--}
```
public Cell getLastDataCell()
```


يحصل على آخر خلية غير فارغة في الصف.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getStyle() {#getStyle--}
```
public Style getStyle()
```


يحصل على نمط هذا الصف.

**Remarks**

تعديل كائن النمط المُرجَع مباشرة لا يؤثر على هذا الصف أو أي خلايا فيه. يجب عليك استدعاء طريقة [applyStyle(Style,StyleFlag)](../../com.aspose.cells/row\#applyStyle-Style-StyleFlag-) أو [setStyle(Style)](../../com.aspose.cells/row\#setStyle-Style-) لتطبيق التغيير على هذا الصف.

نمط الصف هو النمط الذي سيتم وراثته من قبل الخلايا في هذا الصف (تلك الخلايا التي لا تملك إعدادات نمط مخصصة، مثل الخلايا الموجودة التي لم يتم تعيين نمط لها صراحةً، أو تلك التي لم تُنشأ بعد).

**Returns:**
[Style](../../com.aspose.cells/style)
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


يشير إلى ما إذا كان هذا الصف يحتوي على إعدادات نمط مخصصة (مختلفة عن الإعداد الافتراضي الموروث من دفتر العمل).

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBlank() {#isBlank--}
```
public boolean isBlank()
```


يشير إلى ما إذا كان الصف يحتوي على أي بيانات

**Returns:**
boolean
### isCollapsed() {#isCollapsed--}
```
public boolean isCollapsed()
```


ما إذا كان الصف مُطوى

**Returns:**
boolean
### isHeightMatched() {#isHeightMatched--}
```
public boolean isHeightMatched()
```


يشير إلى ما إذا كان ارتفاع الصف يتطابق مع إعداد الخط الافتراضي الحالي لدفتر العمل. قيمة true لهذه الخاصية تعني أيضًا أن ارتفاع الصف "تلقائي" دون قيمة ارتفاع مخصصة يحددها المستخدم.

**Remarks**

عندما تكون هذه الخاصية true، إذا تغير محتوى هذا الصف، عادةً ما يحتاج ارتفاع الصف إلى إعادة حسابه (مثلًا باستخدام [Worksheet.autoFitRows()](../../com.aspose.cells/worksheet\#autoFitRows--)) للحصول على نفس النتيجة التي تُظهرها مايكروسوفت إكسل عند فتح دفتر العمل فيه.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


يشير إلى ما إذا كان الصف مخفيًا.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


يحصل على مُعدِّد الخلايا

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.getRows().get(1).iterator();
         	while (en.hasNext())
         	{
         	    Cell cell = (Cell)en.next();
         	    System.out.println(cell.getName() + ": " + cell.getValue());
         	}
```

**Returns:**
java.util.Iterator - مُعدِّد الخلايا الذي سيتنقل عبر جميع الخلايا الموجودة في هذا الصف.
### iterator(boolean reversed, boolean sync) {#iterator-boolean-boolean-}
```
public Iterator iterator(boolean reversed, boolean sync)
```


يحصل على مُعدِّد يتنقل عبر الخلايا في هذا الصف.

**Remarks**

إذا كان سيتم تعديل الصف (بعمليات قد تؤدي إلى إنشاء خلية جديدة أو إزالة خلية موجودة) أثناء التنقل باستخدام المُعدِّد، يجب استخدام مُعدِّد متزامن بدلاً من المُعدِّد العادي حتى يتمكن التنقل من الاستمرار من الموضع الذي يلي الأخير الذي تم التنقل عبره بواسطة MoveNext() الأخير. ومع ذلك، إلى جانب الميزة التي لا يتم فيها تخطي أو تكرار أي عنصر، فإن العيب في المُعدِّد المتزامن هو أن الأداء سيتدهور قليلًا مقارنةً بالمُعدِّد العادي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| معكوس | boolean | ما إذا كان يتم تعداد الخلايا بترتيب عكسي |
| مزامنة | boolean | ما إذا كان يجب على المُعدِّد المرجعي المعاد التحقق من تعديل الخلايا في هذا الصف والحفاظ على التزامن معه. |

**Returns:**
java.util.Iterator - مُعدِّد الخلايا الذي سيتنقل عبر جميع الخلايا الموجودة في هذا الصف.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public void setCollapsed(boolean value)
```


ما إذا كان الصف مُطوى

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setGroupLevel(byte value) {#setGroupLevel-byte-}
```
public void setGroupLevel(byte value)
```


يحصل على مستوى المجموعة للصف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | byte |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


يضبط ارتفاع الصف بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setHeightMatched(boolean value) {#setHeightMatched-boolean-}
```
public void setHeightMatched(boolean value)
```


يشير إلى ما إذا كان ارتفاع الصف يتطابق مع إعداد الخط الافتراضي الحالي لدفتر العمل. قيمة true لهذه الخاصية تعني أيضًا أن ارتفاع الصف "تلقائي" دون قيمة ارتفاع مخصصة يحددها المستخدم.

**Remarks**

عندما تكون هذه الخاصية true، إذا تغير محتوى هذا الصف، عادةً ما يحتاج ارتفاع الصف إلى إعادة حسابه (مثلًا باستخدام [Worksheet.autoFitRows()](../../com.aspose.cells/worksheet\#autoFitRows--)) للحصول على نفس النتيجة التي تُظهرها مايكروسوفت إكسل عند فتح دفتر العمل فيه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


يشير إلى ما إذا كان الصف مخفيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


يضبط نمط هذا الصف.

**Remarks**

هذه الطريقة تقوم فقط بتعيين النمط المحدد كنمط افتراضي لهذا الصف، دون تغيير إعدادات النمط للخلايا الموجودة في هذا الصف. لتحديث إعدادات النمط للخلايا الموجودة إلى النمط المحدد في نفس الوقت، يرجى استخدام [applyStyle(Style,StyleFlag)](../../com.aspose.cells/row\#applyStyle-Style-StyleFlag-)

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | النمط الذي سيُستخدم كنمط افتراضي للخلايا في هذا الصف. |

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

