---
title: "ListObject"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل جدولًا في ورقة عمل."
type: docs
url: /ar/java/com.aspose.cells/listobject/
---

**Inheritance:**
java.lang.Object
```
public class ListObject
```

يمثل جدولًا في ورقة عمل.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         for (int i = 0; i  ? i++)
         {
         cells.get(0,i).putValue(CellsHelper.columnIndexToName(i));
          }
         for (int row = 1; row  ? row++)
         {
          for (int column = 0; column  ? column++)
         {
         cells.get(row, column).putValue(row * column);
          }
          }
         ListObjectCollection tables = workbook.getWorksheets().get(0).getListObjects();
         int index = tables.add(0, 0, 9, 4, true);
         ListObject table = tables.get(0);
         table.setShowTotals(true);
         table.getListColumns().get(4).setTotalsCalculation(com.aspose.cells.TotalsCalculation.SUM);
         workbook.save("Book1.xlsx");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [applyStyleToRange()](#applyStyleToRange--) | تطبيق نمط الجدول على النطاق. |
| [convertToRange()](#convertToRange--) | تحويل الجدول إلى نطاق. |
| [convertToRange(TableToRangeOptions options)](#convertToRange-com.aspose.cells.TableToRangeOptions-) | تحويل الجدول إلى نطاق. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter()](#filter--) | تصفية الجدول. |
| [getAlternativeDescription()](#getAlternativeDescription--) | يحصل على الوصف البديل. |
| [getAlternativeText()](#getAlternativeText--) | يحصل على النص البديل. |
| [getAutoFilter()](#getAutoFilter--) | يحصل على الفلتر التلقائي لهذا الجدول. |
| [getClass()](#getClass--) |  |
| [getComment()](#getComment--) | يحصل على تعليق الجدول. |
| [getDataRange()](#getDataRange--) | يحصل على نطاق البيانات للجدول. |
| [getDataSourceType()](#getDataSourceType--) | يحصل على نوع مصدر البيانات للجدول. |
| [getDisplayName()](#getDisplayName--) | يحصل على الاسم المعروض للجدول. |
| [getEndColumn()](#getEndColumn--) | يحصل على العمود النهائي للنطاق. |
| [getEndRow()](#getEndRow--) | يحصل على الصف النهائي للنطاق. |
| [getListColumns()](#getListColumns--) | يحصل على قائمة [ListColumn](../../com.aspose.cells/listcolumn) لهذا الجدول. |
| [getQueryTable()](#getQueryTable--) | يحصل على جدول الاستعلام المرتبط. |
| [getShowHeaderRow()](#getShowHeaderRow--) | يحصل على ما إذا كان هذا الجدول يعرض صف الرأس. |
| [getShowTableStyleColumnStripes()](#getShowTableStyleColumnStripes--) | يشير إلى ما إذا تم تطبيق تنسيق الشرائط العمودية. |
| [getShowTableStyleFirstColumn()](#getShowTableStyleFirstColumn--) | يشير إلى ما إذا كان العمود الأول في الجدول هو النمط المطبق. |
| [getShowTableStyleLastColumn()](#getShowTableStyleLastColumn--) | يشير إلى ما إذا كان العمود الأخير في الجدول هو النمط المطبق. |
| [getShowTableStyleRowStripes()](#getShowTableStyleRowStripes--) | يشير إلى ما إذا تم تطبيق تنسيق الشرائط الصفية. |
| [getShowTotals()](#getShowTotals--) | يحصل على ما إذا كان هذا TAble يعرض صف الإجمال. |
| [getStartColumn()](#getStartColumn--) | يحصل على العمود الابتدائي للنطاق. |
| [getStartRow()](#getStartRow--) | يحصل على الصف الابتدائي للنطاق. |
| [getTableStyleName()](#getTableStyleName--) | يحصل على اسم نمط الجدول. |
| [getTableStyleType()](#getTableStyleType--) | يحصل على النمط المدمج للجدول. |
| [getXmlMap()](#getXmlMap--) | يحصل على [getXmlMap()](../../com.aspose.cells/listobject\#getXmlMap--) المستخدم لهذه القائمة. |
| [hasAutoFilter()](#hasAutoFilter--) | يشير إلى ما إذا تم تطبيق الفلتر التلقائي على هذا الجدول. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putCellFormula(int rowOffset, int columnOffset, String formula)](#putCellFormula-int-int-java.lang.String-) | ضع الصيغة في الخلية داخل الجدول. |
| [putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula)](#putCellFormula-int-int-java.lang.String-boolean-) | ضع الصيغة في الخلية داخل الجدول. |
| [putCellValue(int rowOffset, int columnOffset, Object value)](#putCellValue-int-int-java.lang.Object-) | ضع القيمة في الخلية. |
| [putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel)](#putCellValue-int-int-java.lang.Object-boolean-) | ضع القيمة في الخلية. |
| [removeAutoFilter()](#removeAutoFilter--) | يزيل الفلتر التلقائي المطبق على هذا الجدول. |
| [resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)](#resize-int-int-int-int-boolean-) | غيّر حجم نطاق كائن القائمة. |
| [setAlternativeDescription(String value)](#setAlternativeDescription-java.lang.String-) | يضبط الوصف البديل. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | يضبط النص البديل. |
| [setComment(String value)](#setComment-java.lang.String-) | يضبط تعليق الجدول. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | يضبط الاسم المعروض للجدول. |
| [setHasAutoFilter(boolean value)](#setHasAutoFilter-boolean-) | يشير إلى ما إذا تم تطبيق الفلتر التلقائي على هذا الجدول. |
| [setShowHeaderRow(boolean value)](#setShowHeaderRow-boolean-) | يضبط ما إذا كان هذا الجدول يعرض صف الرأس. |
| [setShowTableStyleColumnStripes(boolean value)](#setShowTableStyleColumnStripes-boolean-) | يشير إلى ما إذا تم تطبيق تنسيق الشرائط العمودية. |
| [setShowTableStyleFirstColumn(boolean value)](#setShowTableStyleFirstColumn-boolean-) | يشير إلى ما إذا كان العمود الأول في الجدول هو النمط المطبق. |
| [setShowTableStyleLastColumn(boolean value)](#setShowTableStyleLastColumn-boolean-) | يشير إلى ما إذا كان العمود الأخير في الجدول هو النمط المطبق. |
| [setShowTableStyleRowStripes(boolean value)](#setShowTableStyleRowStripes-boolean-) | يشير إلى ما إذا تم تطبيق تنسيق الشرائط الصفية. |
| [setShowTotals(boolean value)](#setShowTotals-boolean-) | يضبط ما إذا كان هذا TAble يعرض صف الإجمال. |
| [setTableStyleName(String value)](#setTableStyleName-java.lang.String-) | يضبط اسم نمط الجدول. |
| [setTableStyleType(int value)](#setTableStyleType-int-) | يحصل على النمط المدمج للجدول. |
| [toString()](#toString--) |  |
| [updateColumnName()](#updateColumnName--) | يقوم بتحديث أسماء جميع أعمدة القائمة إلى الخلايا في الجدول. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyleToRange() {#applyStyleToRange--}
```
public void applyStyleToRange()
```


تطبيق نمط الجدول على النطاق.

### convertToRange() {#convertToRange--}
```
public void convertToRange()
```


تحويل الجدول إلى نطاق.

### convertToRange(TableToRangeOptions options) {#convertToRange-com.aspose.cells.TableToRangeOptions-}
```
public void convertToRange(TableToRangeOptions options)
```


تحويل الجدول إلى نطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| options | [TableToRangeOptions](../../com.aspose.cells/tabletorangeoptions) | الخيارات عند تحويل الجدول إلى نطاق. |

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
### filter() {#filter--}
```
public AutoFilter filter()
```


تصفية الجدول.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى ضبط خاصية ListObject.HasAutoFilter./// سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أكتوبر 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getAlternativeDescription() {#getAlternativeDescription--}
```
public String getAlternativeDescription()
```


يحصل على الوصف البديل.

**Returns:**
java.lang.String
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


يحصل على النص البديل.

**Returns:**
java.lang.String
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


يحصل على الفلتر التلقائي لهذا الجدول.

**Remarks**

يعمل فقط عندما يكون [hasAutoFilter()](../../com.aspose.cells/listobject\#hasAutoFilter--) غير صحيح.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
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


يحصل على تعليق الجدول.

**Returns:**
java.lang.String
### getDataRange() {#getDataRange--}
```
public Range getDataRange()
```


يحصل على نطاق البيانات للجدول.

**Returns:**
[Range](../../com.aspose.cells/range)
### getDataSourceType() {#getDataSourceType--}
```
public int getDataSourceType()
```


يحصل على نوع مصدر البيانات للجدول.

انظر [TableDataSourceType](../../com.aspose.cells/tabledatasourcetype).

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


يحصل على الاسم المعروض للجدول.

**Returns:**
java.lang.String
### getEndColumn() {#getEndColumn--}
```
public int getEndColumn()
```


يحصل على العمود النهائي للنطاق.

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


يحصل على الصف النهائي للنطاق.

**Returns:**
int
### getListColumns() {#getListColumns--}
```
public ListColumnCollection getListColumns()
```


يحصل على قائمة [ListColumn](../../com.aspose.cells/listcolumn) لهذا الجدول.

**Returns:**
[ListColumnCollection](../../com.aspose.cells/listcolumncollection)
### getQueryTable() {#getQueryTable--}
```
public QueryTable getQueryTable()
```


يحصل على جدول الاستعلام المرتبط.

**Returns:**
[QueryTable](../../com.aspose.cells/querytable)
### getShowHeaderRow() {#getShowHeaderRow--}
```
public boolean getShowHeaderRow()
```


يحصل على ما إذا كان هذا الجدول يعرض صف الرأس.

**Returns:**
boolean
### getShowTableStyleColumnStripes() {#getShowTableStyleColumnStripes--}
```
public boolean getShowTableStyleColumnStripes()
```


يشير إلى ما إذا تم تطبيق تنسيق الشرائط العمودية.

**Returns:**
boolean
### getShowTableStyleFirstColumn() {#getShowTableStyleFirstColumn--}
```
public boolean getShowTableStyleFirstColumn()
```


يشير إلى ما إذا كان العمود الأول في الجدول هو النمط المطبق.

**Returns:**
boolean
### getShowTableStyleLastColumn() {#getShowTableStyleLastColumn--}
```
public boolean getShowTableStyleLastColumn()
```


يشير إلى ما إذا كان العمود الأخير في الجدول هو النمط المطبق.

**Returns:**
boolean
### getShowTableStyleRowStripes() {#getShowTableStyleRowStripes--}
```
public boolean getShowTableStyleRowStripes()
```


يشير إلى ما إذا تم تطبيق تنسيق الشرائط الصفية.

**Returns:**
boolean
### getShowTotals() {#getShowTotals--}
```
public boolean getShowTotals()
```


يحصل على ما إذا كان هذا TAble يعرض صف الإجمال.

**Returns:**
boolean
### getStartColumn() {#getStartColumn--}
```
public int getStartColumn()
```


يحصل على العمود الابتدائي للنطاق.

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


يحصل على الصف الابتدائي للنطاق.

**Returns:**
int
### getTableStyleName() {#getTableStyleName--}
```
public String getTableStyleName()
```


يحصل على اسم نمط الجدول.

**Returns:**
java.lang.String
### getTableStyleType() {#getTableStyleType--}
```
public int getTableStyleType()
```


يحصل على النمط المدمج للجدول.

انظر [TableStyleType](../../com.aspose.cells/tablestyletype).

**Example**

```
         Workbook workbook = new Workbook("Book1.xlsx");
         ListObjectCollection tables = workbook.getWorksheets().get(0).getListObjects();
         int index = tables.add(0, 0, 9, 4, true);
         ListObject table = tables.get(0);
         table.setTableStyleType(TableStyleType.TABLE_STYLE_DARK_2);
          workbook.save("TableStyle.xlsx");
```

**Returns:**
int
### getXmlMap() {#getXmlMap--}
```
public XmlMap getXmlMap()
```


يحصل على [getXmlMap()](../../com.aspose.cells/listobject\#getXmlMap--) المستخدم لهذه القائمة.

**Returns:**
[XmlMap](../../com.aspose.cells/xmlmap)
### hasAutoFilter() {#hasAutoFilter--}
```
public boolean hasAutoFilter()
```


يشير إلى ما إذا تم تطبيق الفلتر التلقائي على هذا الجدول.

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




### putCellFormula(int rowOffset, int columnOffset, String formula) {#putCellFormula-int-int-java.lang.String-}
```
public void putCellFormula(int rowOffset, int columnOffset, String formula)
```


ضع الصيغة في الخلية داخل الجدول.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowOffset | int | إزاحة الصف في الجدول. |
| columnOffset | int | إزاحة العمود في الجدول. |
| formula | java.lang.String | صيغة الخلية. |

### putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula) {#putCellFormula-int-int-java.lang.String-boolean-}
```
public void putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula)
```


ضع الصيغة في الخلية داخل الجدول.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowOffset | int | إزاحة الصف في الجدول. |
| columnOffset | int | إزاحة العمود في الجدول. |
| formula | java.lang.String | صيغة الخلية. |
| isTotalsRowFormula | boolean |  |

### putCellValue(int rowOffset, int columnOffset, Object value) {#putCellValue-int-int-java.lang.Object-}
```
public void putCellValue(int rowOffset, int columnOffset, Object value)
```


ضع القيمة في الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowOffset | int | إزاحة الصف في الجدول. |
| columnOffset | int | إزاحة العمود في الجدول. |
| القيمة | java.lang.Object | قيمة الخلية. |

### putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel) {#putCellValue-int-int-java.lang.Object-boolean-}
```
public void putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel)
```


ضع القيمة في الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowOffset | int | إزاحة الصف في الجدول. |
| columnOffset | int | إزاحة العمود في الجدول. |
| القيمة | java.lang.Object | قيمة الخلية. |
| isTotalsRowLabel | boolean | يشير إلى ما إذا كان تسمية لصف الإجمال، يعمل فقط لصف الإجمال. إذا كان غير صحيح وكان هذا الصف هو صف الإجمال، سيتم إدراج صف جديد. |

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


يزيل الفلتر التلقائي المطبق على هذا الجدول.

### resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders) {#resize-int-int-int-int-boolean-}
```
public void resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)
```


غيّر حجم نطاق كائن القائمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | فهرس صف البداية للنطاق الجديد. |
| startColumn | int | فهرس عمود البداية للنطاق الجديد. |
| endRow | int | فهرس صف النهاية للنطاق الجديد. |
| endColumn | int | فهرس عمود النهاية للنطاق الجديد. |
| hasHeaders | boolean | ما إذا كان هذا الجدول يحتوي على رؤوس. |

### setAlternativeDescription(String value) {#setAlternativeDescription-java.lang.String-}
```
public void setAlternativeDescription(String value)
```


يضبط الوصف البديل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


يضبط النص البديل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setComment(String value) {#setComment-java.lang.String-}
```
public void setComment(String value)
```


يضبط تعليق الجدول.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


يضبط الاسم المعروض للجدول.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setHasAutoFilter(boolean value) {#setHasAutoFilter-boolean-}
```
public void setHasAutoFilter(boolean value)
```


يشير إلى ما إذا تم تطبيق الفلتر التلقائي على هذا الجدول.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowHeaderRow(boolean value) {#setShowHeaderRow-boolean-}
```
public void setShowHeaderRow(boolean value)
```


يضبط ما إذا كان هذا الجدول يعرض صف الرأس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowTableStyleColumnStripes(boolean value) {#setShowTableStyleColumnStripes-boolean-}
```
public void setShowTableStyleColumnStripes(boolean value)
```


يشير إلى ما إذا تم تطبيق تنسيق الشرائط العمودية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowTableStyleFirstColumn(boolean value) {#setShowTableStyleFirstColumn-boolean-}
```
public void setShowTableStyleFirstColumn(boolean value)
```


يشير إلى ما إذا كان العمود الأول في الجدول هو النمط المطبق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowTableStyleLastColumn(boolean value) {#setShowTableStyleLastColumn-boolean-}
```
public void setShowTableStyleLastColumn(boolean value)
```


يشير إلى ما إذا كان العمود الأخير في الجدول هو النمط المطبق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowTableStyleRowStripes(boolean value) {#setShowTableStyleRowStripes-boolean-}
```
public void setShowTableStyleRowStripes(boolean value)
```


يشير إلى ما إذا تم تطبيق تنسيق الشرائط الصفية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowTotals(boolean value) {#setShowTotals-boolean-}
```
public void setShowTotals(boolean value)
```


يضبط ما إذا كان هذا TAble يعرض صف الإجمال.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setTableStyleName(String value) {#setTableStyleName-java.lang.String-}
```
public void setTableStyleName(String value)
```


يضبط اسم نمط الجدول.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setTableStyleType(int value) {#setTableStyleType-int-}
```
public void setTableStyleType(int value)
```


يحصل على النمط المدمج للجدول.

انظر [TableStyleType](../../com.aspose.cells/tablestyletype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### updateColumnName() {#updateColumnName--}
```
public void updateColumnName()
```


يقوم بتحديث أسماء جميع أعمدة القائمة إلى الخلايا في الجدول.

**Remarks**

يجب أن تكون قيمة الخلايا في صف الرأس للجدول مطابقة لاسم ListColumn؛ لا تقوم Cell.PutValue بتعديل اسم ListColumn تلقائيًا لأداء أفضل.

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

