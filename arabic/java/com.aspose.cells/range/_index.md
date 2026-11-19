---
title: "Range"
second_title: "Aspose.Cells for Java API Reference"
description: "يغلف الكائن الذي يمثل نطاقًا من الخلايا داخل جدول البيانات."
type: docs
url: /ar/java/com.aspose.cells/range/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Range implements Iterable
```

يغلف الكائن الذي يمثل نطاقًا من الخلايا داخل جدول البيانات.

**Remarks**

تشير فئة Range إلى منطقة في جدول بيانات Excel. باستخدامها، يمكنك تنسيق وتعيين قيمة النطاق. ويمكنك أيضًا نسخ نطاق Excel بسهولة.

**Example**

يوضح المثال التالي كيفية إنشاء نطاق وتعيين قيمة النطاق في Excel.

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         // Create a range (A1:D3).
         Range range = cells.createRange("A1", "D3");
         // Set value to the range.
         range.setValue("Hello");
         //Save the Excel file
         workbook.save("book1.xlsm");
```
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [Range(CellArea ca, Cells cells)](#Range-com.aspose.cells.CellArea-com.aspose.cells.Cells-) | منشئ الفئة. |
| [Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells)](#Range-int-int-int-int-com.aspose.cells.Cells-) | منشئ الفئة. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addHyperlink(String address, String textToDisplay, String screenTip)](#addHyperlink-java.lang.String-java.lang.String-java.lang.String-) | يضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا. |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | يطبق التنسيقات على نطاق كامل. |
| [autoFill(Range target)](#autoFill-com.aspose.cells.Range-) | يملأ النطاق المستهدف تلقائيًا. |
| [autoFill(Range target, int autoFillType)](#autoFill-com.aspose.cells.Range-int-) | يملأ النطاق المستهدف تلقائيًا. |
| [clear()](#clear--) | يمسح هذا النطاق. |
| [clearComments()](#clearComments--) | يمسح تعليقات هذا النطاق. |
| [clearContents()](#clearContents--) | يمسح محتويات هذا النطاق. |
| [clearFormats()](#clearFormats--) | يمسح تنسيقات هذا النطاق. |
| [clearHyperlinks(boolean clearFormat)](#clearHyperlinks-boolean-) | يزيل الروابط التشعبية فقط. |
| [copy(Range range)](#copy-com.aspose.cells.Range-) | ينسخ البيانات (بما في ذلك الصيغ)، التنسيق، كائنات الرسم وغيرها من نطاق المصدر. |
| [copy(Range range, PasteOptions options)](#copy-com.aspose.cells.Range-com.aspose.cells.PasteOptions-) | نسخ النطاق باستخدام خيارات اللصق الخاصة. |
| [copyData(Range range)](#copyData-com.aspose.cells.Range-) | ينسخ بيانات الخلية (بما في ذلك الصيغ) من نطاق المصدر. |
| [copyStyle(Range range)](#copyStyle-com.aspose.cells.Range-) | ينسخ إعدادات النمط من نطاق المصدر. |
| [copyValue(Range range)](#copyValue-com.aspose.cells.Range-) | ينسخ قيمة الخلية من نطاق المصدر. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int rowOffset, int columnOffset)](#get-int-int-) | يحصل على كائن [Cell](../../com.aspose.cells/cell) في هذا النطاق. |
| [getAddress()](#getAddress--) | يحصل على عنوان النطاق. |
| [getCellOrNull(int rowOffset, int columnOffset)](#getCellOrNull-int-int-) | يحصل على كائن [Cell](../../com.aspose.cells/cell) أو null في هذا النطاق. |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | يحصل على عدد الأعمدة في النطاق. |
| [getColumnWidth()](#getColumnWidth--) | يضبط أو يحصل على عرض العمود لهذا النطاق |
| [getCurrentRegion()](#getCurrentRegion--) | يرجع كائن Range يمثل المنطقة الحالية. |
| [getEntireColumn()](#getEntireColumn--) | يحصل على كائن Range يمثل العمود (أو الأعمدة) بالكامل الذي يحتوي على النطاق المحدد. |
| [getEntireRow()](#getEntireRow--) | يحصل على كائن Range يمثل الصف (أو الصفوف) بالكامل الذي يحتوي على النطاق المحدد. |
| [getFirstColumn()](#getFirstColumn--) | يحصل على فهرس العمود الأول في النطاق. |
| [getFirstRow()](#getFirstRow--) | يحصل على فهرس الصف الأول في النطاق. |
| [getHeight()](#getHeight--) | يحصل على عرض النطاق بالنقاط. |
| [getHyperlinks()](#getHyperlinks--) | يحصل على جميع الروابط التشعبية في النطاق. |
| [getLeft()](#getLeft--) | يحصل على المسافة، بالنقاط، من الحافة اليسرى للعمود A إلى الحافة اليسرى للنطاق. |
| [getName()](#getName--) | يحصل على اسم النطاق. |
| [getOffset(int rowOffset, int columnOffset)](#getOffset-int-int-) | يحصل على نطاق [Range](../../com.aspose.cells/range) عن طريق الإزاحة. |
| [getRefersTo()](#getRefersTo--) | يحصل على ما يشير إليه النطاق. |
| [getRowCount()](#getRowCount--) | يحصل على عدد الصفوف في النطاق. |
| [getRowHeight()](#getRowHeight--) | يضبط أو يحصل على ارتفاع الصفوف في هذا النطاق |
| [getTop()](#getTop--) | يحصل على المسافة، بالنقاط، من الحافة العلوية للصف 1 إلى الحافة العلوية للنطاق. |
| [getValue()](#getValue--) | يحصل على قيمة النطاق. |
| [getWidth()](#getWidth--) | يحصل على عرض النطاق بالنقاط. |
| [getWorksheet()](#getWorksheet--) | يحصل على كائن [getWorksheet()](../../com.aspose.cells/range\#getWorksheet--) الذي يحتوي على هذا النطاق. |
| [hashCode()](#hashCode--) |  |
| [intersect(Range range)](#intersect-com.aspose.cells.Range-) | يرجع كائن [Range](../../com.aspose.cells/range) يمثل تقاطع مستطيل لنطاقين. |
| [isBlank()](#isBlank--) | يشير إلى ما إذا كان النطاق يحتوي على قيم. |
| [isIntersect(Range range)](#isIntersect-com.aspose.cells.Range-) | يشير إلى ما إذا كان النطاق يتقاطع. |
| [iterator()](#iterator--) | يحصل على المُعدِّد للخلايا في هذا النطاق. |
| [merge()](#merge--) | يجمع مجموعة من الخلايا في خلية واحدة. |
| [moveTo(int destRow, int destColumn)](#moveTo-int-int-) | نقل النطاق الحالي إلى النطاق الهدف. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | يضع قيمة في النطاق، إذا كان مناسبًا سيتم تحويل القيمة إلى نوع بيانات آخر وسيتم إعادة ضبط تنسيق الأرقام للخلية. |
| [setColumnWidth(double value)](#setColumnWidth-double-) | يضبط أو يحصل على عرض العمود لهذا النطاق |
| [setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor)](#setInsideBorders-int-int-com.aspose.cells.CellsColor-) | تعيين الحدود الداخلية للنطاق. |
| [setName(String value)](#setName-java.lang.String-) | يحدد اسم النطاق. |
| [setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor)](#setOutlineBorder-int-int-com.aspose.cells.CellsColor-) | يحدد حدًا خارجيًا حول مجموعة من الخلايا. |
| [setOutlineBorder(int borderEdge, int borderStyle, Color borderColor)](#setOutlineBorder-int-int-com.aspose.cells.Color-) | يحدد حدًا خارجيًا حول مجموعة من الخلايا. |
| [setOutlineBorders(int borderStyle, CellsColor borderColor)](#setOutlineBorders-int-com.aspose.cells.CellsColor-) | يحدد الحدود الخارجية حول مجموعة من الخلايا بنفس نمط الحد واللون. |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | يحدد الحدود الخارجية حول مجموعة من الخلايا بنفس نمط الحد واللون. |
| [setOutlineBorders(int[] borderStyles, Color[] borderColors)](#setOutlineBorders-int---com.aspose.cells.Color---) | يحدد حدودًا خارجية حول مجموعة من الخلايا. |
| [setRowHeight(double value)](#setRowHeight-double-) | يضبط أو يحصل على ارتفاع الصفوف في هذا النطاق |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | يحدد نمط النطاق. |
| [setStyle(Style style, boolean explicitFlag)](#setStyle-com.aspose.cells.Style-boolean-) | تطبيق نمط الخلية. |
| [setValue(Object value)](#setValue-java.lang.Object-) | يحدد قيمة النطاق. |
| [toHtml(HtmlSaveOptions saveOptions)](#toHtml-com.aspose.cells.HtmlSaveOptions-) | تحويل النطاق إلى HTML. |
| [toImage(ImageOrPrintOptions options)](#toImage-com.aspose.cells.ImageOrPrintOptions-) | يحول النطاق إلى صورة. |
| [toJson(JsonSaveOptions options)](#toJson-com.aspose.cells.JsonSaveOptions-) | تحويل النطاق إلى قيمة JSON. |
| [toString()](#toString--) | يرجع سلسلة تمثل كائن النطاق الحالي. |
| [transpose()](#transpose--) | تحويل (تدوير) البيانات من الصفوف إلى الأعمدة أو العكس. |
| [unMerge()](#unMerge--) | يفك دمج الخلايا المدمجة في هذا النطاق. |
| [union(Range range)](#union-com.aspose.cells.Range-) | يعيد اتحاد نطاقين. |
| [unionRang(Range range)](#unionRang-com.aspose.cells.Range-) | يعيد نتيجة اتحاد نطاقين. |
| [unionRanges(Range[] ranges)](#unionRanges-com.aspose.cells.Range---) | يعيد نتيجة اتحاد نطاقين. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Range(CellArea ca, Cells cells) {#Range-com.aspose.cells.CellArea-com.aspose.cells.Cells-}
```
public Range(CellArea ca, Cells cells)
```


منشئ الفئة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | النطاق. |
| cells | [Cells](../../com.aspose.cells/cells) |  |

### Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells) {#Range-int-int-int-int-com.aspose.cells.Cells-}
```
public Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells)
```


منشئ الفئة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | int | الصف الأول في هذا النطاق (مؤشر صفر) |
| firstColumn | int | العمود الأول من هذا النطاق (صفر أساس). |
| rowNumber | int | عدد الصفوف (مؤشر واحد) |
| columnNumber | int | عدد الأعمدة (مستند إلى الواحد) |
| cells | [Cells](../../com.aspose.cells/cells) | كائن النطاق ينتمي إلى كائن الخلايا هذا. |

### addHyperlink(String address, String textToDisplay, String screenTip) {#addHyperlink-java.lang.String-java.lang.String-java.lang.String-}
```
public Hyperlink addHyperlink(String address, String textToDisplay, String screenTip)
```


يضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| العنوان | java.lang.String | عنوان الارتباط التشعبي. |
| textToDisplay | java.lang.String | النص الذي سيُعرض للرابط المحدد. |
| screenTip | java.lang.String | نص تلميح الشاشة للرابط المحدد. |

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink) - [Hyperlink](../../com.aspose.cells/hyperlink) object.
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


يطبق التنسيقات على نطاق كامل.

**Remarks**

كل خلية في هذا النطاق ستحتوي على كائن [Style](../../com.aspose.cells/style). لذا فإن هذه طريقة مستهلكة للذاكرة. يرجى استخدامها بحذر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | كائن النمط الذي سيتم تطبيقه. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | علامات تشير إلى خصائص التنسيق المطبقة. |

### autoFill(Range target) {#autoFill-com.aspose.cells.Range-}
```
public void autoFill(Range target)
```


يملأ النطاق المستهدف تلقائيًا.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").putValue(1);
         cells.get("A2").putValue(2);
         Range source = cells.createRange("A1:A2");
         Range target = cells.createRange("A3:A10");
         //fill 3,4,5....10 to the range A3:A10
         source.autoFill(target);
         //Save the Excel file
         workbook.save("book1.xlsm");
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| target | [Range](../../com.aspose.cells/range) | النطاق الهدف. |

### autoFill(Range target, int autoFillType) {#autoFill-com.aspose.cells.Range-int-}
```
public void autoFill(Range target, int autoFillType)
```


يملأ النطاق المستهدف تلقائيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| target | [Range](../../com.aspose.cells/range) | النطاق المستهدف. |
| autoFillType | int | [AutoFillType](../../com.aspose.cells/autofilltype). نوع التعبئة التلقائي. |

### clear() {#clear--}
```
public void clear()
```


يمسح هذا النطاق.

### clearComments() {#clearComments--}
```
public void clearComments()
```


يمسح تعليقات هذا النطاق.

### clearContents() {#clearContents--}
```
public void clearContents()
```


يمسح محتويات هذا النطاق.

### clearFormats() {#clearFormats--}
```
public void clearFormats()
```


يمسح تنسيقات هذا النطاق.

### clearHyperlinks(boolean clearFormat) {#clearHyperlinks-boolean-}
```
public void clearHyperlinks(boolean clearFormat)
```


يزيل الروابط التشعبية فقط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| clearFormat | boolean | يشير إلى ما إذا كان يجب مسح تنسيق الروابط. |

### copy(Range range) {#copy-com.aspose.cells.Range-}
```
public void copy(Range range)
```


ينسخ البيانات (بما في ذلك الصيغ)، التنسيق، كائنات الرسم وغيرها من نطاق المصدر.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         Range range1 = cells.createRange("A1:A5");
         Range range2 = cells.createRange("A6:A10");
         //Copy the range.
         range1.copy(range2);
         //Save the Excel file
         workbook.save("book1.xlsm");
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | كائن [Range](../../com.aspose.cells/range) المصدر. |

### copy(Range range, PasteOptions options) {#copy-com.aspose.cells.Range-com.aspose.cells.PasteOptions-}
```
public void copy(Range range, PasteOptions options)
```


نسخ النطاق باستخدام خيارات اللصق الخاصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | النطاق المصدر. |
| options | [PasteOptions](../../com.aspose.cells/pasteoptions) | خيارات اللصق الخاصة. |

### copyData(Range range) {#copyData-com.aspose.cells.Range-}
```
public void copyData(Range range)
```


ينسخ بيانات الخلية (بما في ذلك الصيغ) من نطاق المصدر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | كائن [Range](../../com.aspose.cells/range) المصدر. |

### copyStyle(Range range) {#copyStyle-com.aspose.cells.Range-}
```
public void copyStyle(Range range)
```


ينسخ إعدادات النمط من نطاق المصدر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | كائن [Range](../../com.aspose.cells/range) المصدر. |

### copyValue(Range range) {#copyValue-com.aspose.cells.Range-}
```
public void copyValue(Range range)
```


ينسخ قيمة الخلية من نطاق المصدر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | كائن [Range](../../com.aspose.cells/range) المصدر. |

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
### get(int rowOffset, int columnOffset) {#get-int-int-}
```
public Cell get(int rowOffset, int columnOffset)
```


يحصل على كائن [Cell](../../com.aspose.cells/cell) في هذا النطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowOffset | int | إزاحة الصف في هذا النطاق، بدءًا من الصفر. |
| columnOffset | int | إزاحة العمود في هذا النطاق، بدءًا من الصفر. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - [Cell](../../com.aspose.cells/cell) object.
### getAddress() {#getAddress--}
```
public String getAddress()
```


يحصل على عنوان النطاق.

**Returns:**
java.lang.String
### getCellOrNull(int rowOffset, int columnOffset) {#getCellOrNull-int-int-}
```
public Cell getCellOrNull(int rowOffset, int columnOffset)
```


يحصل على كائن [Cell](../../com.aspose.cells/cell) أو null في هذا النطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowOffset | int | إزاحة الصف في هذا النطاق، بدءًا من الصفر. |
| columnOffset | int | إزاحة العمود في هذا النطاق، بدءًا من الصفر. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - [Cell](../../com.aspose.cells/cell) object.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


يحصل على عدد الأعمدة في النطاق.

**Returns:**
int
### getColumnWidth() {#getColumnWidth--}
```
public double getColumnWidth()
```


يضبط أو يحصل على عرض العمود لهذا النطاق

**Returns:**
double
### getCurrentRegion() {#getCurrentRegion--}
```
public Range getCurrentRegion()
```


يعيد كائن Range يمثل المنطقة الحالية. المنطقة الحالية هي نطاق محاط بأي تركيبة من الصفوف الفارغة والأعمدة الفارغة.

**Returns:**
[Range](../../com.aspose.cells/range)
### getEntireColumn() {#getEntireColumn--}
```
public Range getEntireColumn()
```


يحصل على كائن Range يمثل العمود (أو الأعمدة) بالكامل الذي يحتوي على النطاق المحدد.

**Returns:**
[Range](../../com.aspose.cells/range)
### getEntireRow() {#getEntireRow--}
```
public Range getEntireRow()
```


يحصل على كائن Range يمثل الصف (أو الصفوف) بالكامل الذي يحتوي على النطاق المحدد.

**Returns:**
[Range](../../com.aspose.cells/range)
### getFirstColumn() {#getFirstColumn--}
```
public int getFirstColumn()
```


يحصل على فهرس العمود الأول في النطاق.

**Returns:**
int
### getFirstRow() {#getFirstRow--}
```
public int getFirstRow()
```


يحصل على فهرس الصف الأول في النطاق.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


يحصل على عرض النطاق بالنقاط.

**Returns:**
double
### getHyperlinks() {#getHyperlinks--}
```
public Hyperlink[] getHyperlinks()
```


يحصل على جميع الروابط التشعبية في النطاق.

**Returns:**
com.aspose.cells.Hyperlink[]
### getLeft() {#getLeft--}
```
public double getLeft()
```


يحصل على المسافة، بالنقاط، من الحافة اليسرى للعمود A إلى الحافة اليسرى للنطاق.

**Returns:**
double
### getName() {#getName--}
```
public String getName()
```


يحصل على اسم النطاق.

**Remarks**

النطاق المسمى مدعوم. على سبيل المثال،

range.Name = "Sheet1!MyRange";

**Returns:**
java.lang.String
### getOffset(int rowOffset, int columnOffset) {#getOffset-int-int-}
```
public Range getOffset(int rowOffset, int columnOffset)
```


يحصل على نطاق [Range](../../com.aspose.cells/range) عن طريق الإزاحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowOffset | int | إزاحة الصف في هذا النطاق، بدءًا من الصفر. |
| columnOffset | int | إزاحة العمود في هذا النطاق، بدءًا من الصفر. |

**Returns:**
[Range](../../com.aspose.cells/range) - 
### getRefersTo() {#getRefersTo--}
```
public String getRefersTo()
```


يحصل على ما يشير إليه النطاق.

**Returns:**
java.lang.String
### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


يحصل على عدد الصفوف في النطاق.

**Returns:**
int
### getRowHeight() {#getRowHeight--}
```
public double getRowHeight()
```


يضبط أو يحصل على ارتفاع الصفوف في هذا النطاق

**Returns:**
double
### getTop() {#getTop--}
```
public double getTop()
```


يحصل على المسافة، بالنقاط، من الحافة العلوية للصف 1 إلى الحافة العلوية للنطاق.

**Returns:**
double
### getValue() {#getValue--}
```
public Object getValue()
```


يحصل على قيمة النطاق.

**Remarks**

إذا كان النطاق يحتوي على خلايا متعددة، يجب أن يكون الكائن المرتجع/المطبق هو Object[][].

**Returns:**
java.lang.Object
### getWidth() {#getWidth--}
```
public double getWidth()
```


يحصل على عرض النطاق بالنقاط.

**Returns:**
double
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


يحصل على كائن [getWorksheet()](../../com.aspose.cells/range\#getWorksheet--) الذي يحتوي على هذا النطاق.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### intersect(Range range) {#intersect-com.aspose.cells.Range-}
```
public Range intersect(Range range)
```


يرجع كائن [Range](../../com.aspose.cells/range) يمثل تقاطع مستطيل لنطاقين.

**Remarks**

إذا لم تتقاطع النطاقان، يعيد null.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         Range range1 = cells.createRange("A1:A5");
         Range range2 = cells.createRange("A3:A10");
         //Get intersected range of the two ranges.
         Range intersectRange = range1.intersect(range2);
         //Save the Excel file
         workbook.save("book1.xlsm");
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | النطاق المتقاطع. |

**Returns:**
[Range](../../com.aspose.cells/range) - Returns a [Range](../../com.aspose.cells/range) object
### isBlank() {#isBlank--}
```
public boolean isBlank()
```


يشير إلى ما إذا كان النطاق يحتوي على قيم.

**Returns:**
boolean -
### isIntersect(Range range) {#isIntersect-com.aspose.cells.Range-}
```
public boolean isIntersect(Range range)
```


يشير إلى ما إذا كان النطاق يتقاطع.

**Remarks**

إذا لم تكن النطاقان في نفس ورقة العمل، إرجاع false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | النطاق. |

**Returns:**
boolean - ما إذا كان النطاق متقاطعًا.
### iterator() {#iterator--}
```
public Iterator iterator()
```


يحصل على المُعدِّد للخلايا في هذا النطاق.

**Remarks**

عند تجوال العناصر باستخدام الـ Enumerator المُرجَع، يجب عدم تعديل مجموعة الخلايا (مثل العمليات التي قد تُنشئ خلية/صف جديد أو تحذف خلية/صف موجود). وإلا قد لا يتمكن الـ enumerator من تجوال جميع الخلايا بشكل صحيح (قد يتم تجوال بعض العناصر أكثر من مرة أو يتم تخطيها).

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.createRange("B2:C3").iterator();
         	while (en.hasNext())
         	{
         	    Cell cell = (Cell)en.next();
         	    System.out.println(cell.getName() + ": " + cell.getValue());
         	}
```

**Returns:**
java.util.Iterator - مُعدِّد الخلايا
### merge() {#merge--}
```
public void merge()
```


يجمع مجموعة من الخلايا في خلية واحدة.

**Remarks**

الإشارة إلى الخلية المدمجة عبر عنوان الخلية العليا اليسرى في النطاق.

### moveTo(int destRow, int destColumn) {#moveTo-int-int-}
```
public void moveTo(int destRow, int destColumn)
```


نقل النطاق الحالي إلى النطاق الهدف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| destRow | int | صف البداية للنطاق الوجهة. |
| destColumn | int | عمود البداية للنطاق الوجهة. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


يضع قيمة في النطاق، إذا كان مناسبًا سيتم تحويل القيمة إلى نوع بيانات آخر وسيتم إعادة ضبط تنسيق الأرقام للخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stringValue | java.lang.String | قيمة الإدخال |
| isConverted | boolean | True: تم التحويل إلى نوع بيانات آخر إذا كان مناسبًا. |
| setStyle | boolean | True: ضبط تنسيق الرقم على نمط الخلية عند التحويل إلى نوع بيانات آخر |

### setColumnWidth(double value) {#setColumnWidth-double-}
```
public void setColumnWidth(double value)
```


يضبط أو يحصل على عرض العمود لهذا النطاق

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor) {#setInsideBorders-int-int-com.aspose.cells.CellsColor-}
```
public void setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor)
```


تعيين الحدود الداخلية للنطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). داخل نوع الحدود، يمكن أن يكون فقط [BorderType.VERTICAL](../../com.aspose.cells/bordertype\#VERTICAL) و [BorderType.HORIZONTAL](../../com.aspose.cells/bordertype\#HORIZONTAL). |
| lineStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). نمط الحد. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | لون الحد. |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


يحدد اسم النطاق.

**Remarks**

النطاق المسمى مدعوم. على سبيل المثال،

range.Name = "Sheet1!MyRange";

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor) {#setOutlineBorder-int-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor)
```


يحدد حدًا خارجيًا حول مجموعة من الخلايا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). حافة الحد. |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). نمط الحد. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | لون الحد. |

### setOutlineBorder(int borderEdge, int borderStyle, Color borderColor) {#setOutlineBorder-int-int-com.aspose.cells.Color-}
```
public void setOutlineBorder(int borderEdge, int borderStyle, Color borderColor)
```


يحدد حدًا خارجيًا حول مجموعة من الخلايا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). حافة الحد. |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). نمط الحد. |
| borderColor | [Color](../../com.aspose.cells/color) | لون الحد. |

### setOutlineBorders(int borderStyle, CellsColor borderColor) {#setOutlineBorders-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorders(int borderStyle, CellsColor borderColor)
```


يحدد الحدود الخارجية حول مجموعة من الخلايا بنفس نمط الحد واللون.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). نمط الحد. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | لون الحد. |

### setOutlineBorders(int borderStyle, Color borderColor) {#setOutlineBorders-int-com.aspose.cells.Color-}
```
public void setOutlineBorders(int borderStyle, Color borderColor)
```


يحدد الحدود الخارجية حول مجموعة من الخلايا بنفس نمط الحد واللون.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). نمط الحد. |
| borderColor | [Color](../../com.aspose.cells/color) | لون الحد. |

### setOutlineBorders(int[] borderStyles, Color[] borderColors) {#setOutlineBorders-int---com.aspose.cells.Color---}
```
public void setOutlineBorders(int[] borderStyles, Color[] borderColors)
```


يحدد حدودًا خارجية حول مجموعة من الخلايا.

**Remarks**

يجب أن يكون طول كل من borderStyles و borderStyles هو 4. يجب أن يكون ترتيب borderStyles و borderStyles هو الأعلى، الأسفل، اليسار، اليمين.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| borderStyles | int[] | [CellBorderType](../../com.aspose.cells/cellbordertype). أنماط الحد. |
| borderColors | [Color\[\]](../../com.aspose.cells/color) | ألوان الحدود. |

### setRowHeight(double value) {#setRowHeight-double-}
```
public void setRowHeight(double value)
```


يضبط أو يحصل على ارتفاع الصفوف في هذا النطاق

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


يحدد نمط النطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | كائن Style. |

### setStyle(Style style, boolean explicitFlag) {#setStyle-com.aspose.cells.Style-boolean-}
```
public void setStyle(Style style, boolean explicitFlag)
```


تطبيق نمط الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | نمط الخلية. |
| explicitFlag | boolean | صحيح، يتم الكتابة فوق التنسيق فقط إذا تم تعيينه صراحةً. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


يحدد قيمة النطاق.

**Remarks**

إذا كان النطاق يحتوي على خلايا متعددة، يجب أن يكون الكائن المرتجع/المطبق هو Object[][].

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object |  |

### toHtml(HtmlSaveOptions saveOptions) {#toHtml-com.aspose.cells.HtmlSaveOptions-}
```
public byte[] toHtml(HtmlSaveOptions saveOptions)
```


تحويل النطاق إلى HTML.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| saveOptions | [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) | خيارات تحويل النطاق إلى html. |

**Returns:**
byte[] -
### toImage(ImageOrPrintOptions options) {#toImage-com.aspose.cells.ImageOrPrintOptions-}
```
public byte[] toImage(ImageOrPrintOptions options)
```


يحول النطاق إلى صورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | الخيارات لتحويل هذا النطاق إلى صورة |

**Returns:**
byte[] -
### toJson(JsonSaveOptions options) {#toJson-com.aspose.cells.JsonSaveOptions-}
```
public String toJson(JsonSaveOptions options)
```


تحويل النطاق إلى قيمة JSON.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| options | [JsonSaveOptions](../../com.aspose.cells/jsonsaveoptions) | خيارات التحويل |

**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```


يرجع سلسلة تمثل كائن النطاق الحالي.

**Returns:**
java.lang.String -
### transpose() {#transpose--}
```
public void transpose()
```


تحويل (تدوير) البيانات من الصفوف إلى الأعمدة أو العكس.

### unMerge() {#unMerge--}
```
public void unMerge()
```


يفك دمج الخلايا المدمجة في هذا النطاق.

### union(Range range) {#union-com.aspose.cells.Range-}
```
public ArrayList union(Range range)
```


يعيد اتحاد نطاقين.

**Remarks**

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة Range.UnionRanges(). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ نوفمبر 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | النطاق |

**Returns:**
java.util.ArrayList - اتحاد نطاقين.
### unionRang(Range range) {#unionRang-com.aspose.cells.Range-}
```
public Range[] unionRang(Range range)
```


يعيد نتيجة اتحاد نطاقين.

**Remarks**

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة Range.UnionRanges(). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ مايو 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | النطاق |

**Returns:**
com.aspose.cells.Range[] - اتحاد نطاقين.
### unionRanges(Range[] ranges) {#unionRanges-com.aspose.cells.Range---}
```
public UnionRange unionRanges(Range[] ranges)
```


يعيد نتيجة اتحاد نطاقين.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | النطاق |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - The union of two ranges.
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

