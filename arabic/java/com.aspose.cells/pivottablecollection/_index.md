---
title: "PivotTableCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل مجموعة جميع كائنات PivotTable في ورقة العمل المحددة."
type: docs
url: /ar/java/com.aspose.cells/pivottablecollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotTableCollection extends CollectionBase
```

يمثل مجموعة جميع كائنات PivotTable في ورقة العمل المحددة.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         //Add PivotFilter
         PivotFilter filter = pivot.getRowFields().get(0).filterTop10(0, PivotFilterType.PERCENT, false, 2);
 
 
         //Add PivotFormatCondition
         int formatIndex = pivot.getConditionalFormats().add();
         PivotConditionalFormat pfc = pivot.getConditionalFormats().get(formatIndex);
         pfc.addCellArea(pivot.getDataBodyRange());
         FormatConditionCollection fcc = pfc.getFormatConditions();
         int ii = fcc.addCondition(FormatConditionType.CELL_VALUE, OperatorType.GREATER_OR_EQUAL, "100", null);
 
         FormatCondition fc = fcc.get(ii);
 
         fc.getStyle().setBackgroundColor(Color.getRed());
 
         pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(PivotTable pivotTable, int row, int column, String tableName)](#add-com.aspose.cells.PivotTable-int-int-java.lang.String-) | يضيف PivotTable جديدًا بناءً على PivotTable آخر. |
| [add(PivotTable pivotTable, String destCellName, String tableName)](#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-) | يضيف PivotTable جديدًا بناءً على PivotTable آخر. |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [add(String sourceData, int row, int column)](#add-java.lang.String-int-int-) | يضيف PivotTable حديثًا جديدًا (منذ Excel 2007) في الصف والعمود المحددين في ورقة العمل مع الخيارات الافتراضية. |
| [add(String sourceData, int row, int column, PivotTableCreateOptions options)](#add-java.lang.String-int-int-com.aspose.cells.PivotTableCreateOptions-) | يضيف PivotTable جديدًا في الصف والعمود المحددين في ورقة العمل. |
| [add(String sourceData, int row, int column, String tableName)](#add-java.lang.String-int-int-java.lang.String-) | يضيف PivotTable جديدًا بتنسيق ونمط Excel القديم (97-2003). |
| [add(String sourceData, int row, int column, String tableName, boolean useSameSource)](#add-java.lang.String-int-int-java.lang.String-boolean-) | يضيف PivotTable جديدًا بتنسيق ونمط Excel القديم (97-2003). |
| [add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic)](#add-java.lang.String-int-int-java.lang.String-boolean-boolean-) | يضيف PivotTable جديدًا بتنسيق ونمط Excel القديم (97-2003). |
| [add(String sourceData, String cellName)](#add-java.lang.String-java.lang.String-) | يضيف PivotTable حديثًا جديدًا (منذ Excel 2007) في الصف والعمود المحددين في ورقة العمل مع الخيارات الافتراضية. |
| [add(String sourceData, String cellName, PivotTableCreateOptions options)](#add-java.lang.String-java.lang.String-com.aspose.cells.PivotTableCreateOptions-) | يضيف PivotTable حديثًا جديدًا (منذ Excel 2007) في الصف والعمود المحددين في ورقة العمل مع الخيارات الافتراضية. |
| [add(String sourceData, String destCellName, String tableName)](#add-java.lang.String-java.lang.String-java.lang.String-) | يضيف PivotTable جديدًا بتنسيق ونمط Excel القديم (97-2003). |
| [add(String sourceData, String destCellName, String tableName, boolean useSameSource)](#add-java.lang.String-java.lang.String-java.lang.String-boolean-) | يضيف PivotTable جديدًا بتنسيق ونمط Excel القديم (97-2003). |
| [add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic)](#add-java.lang.String-java.lang.String-java.lang.String-boolean-boolean-) | يضيف PivotTable جديدًا. |
| [add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName)](#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-int-int-java.lang.String-) | يضيف كائن PivotTable جديد إلى المجموعة مع نطاقات دمج متعددة كمصدر للبيانات. |
| [add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName)](#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-java.lang.String-java.lang.String-) | يضيف كائن PivotTable جديد إلى المجموعة مع نطاقات دمج متعددة كمصدر للبيانات. |
| [clear()](#clear--) | يمسح جميع جداول PivotTable. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [dispose()](#dispose--) | ينفذ مهام محددة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة ضبط الموارد غير المُدارة. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على تقرير PivotTable حسب الفهرس. |
| [get(int row, int column)](#get-int-int-) | يحصل على [PivotTable](../../com.aspose.cells/pivottable) الموجود في الخلية. |
| [get(String name)](#get-java.lang.String-) | يحصل على تقرير PivotTable حسب اسم PivotTable. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في مثيل CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | يحدد فهرس عنصر محدد في مثيل CollectionBase. |
| [iterator()](#iterator--) | يرجع كائن تعداد يتنقل عبر مثيل CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(PivotTable pivotTable)](#remove-com.aspose.cells.PivotTable-) | يحذف PivotTable المحدد ويحذف بيانات PivotTable. |
| [remove(PivotTable pivotTable, boolean keepData)](#remove-com.aspose.cells.PivotTable-boolean-) | يحذف PivotTable المحدد. |
| [removeAt(int index)](#removeAt-int-) | يحذف PivotTable في الفهرس المحدد ويحذف بيانات PivotTable. |
| [removeAt(int index, boolean keepData)](#removeAt-int-boolean-) | يحذف PivotTable في الفهرس المحدد. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(PivotTable pivotTable, int row, int column, String tableName) {#add-com.aspose.cells.PivotTable-int-int-java.lang.String-}
```
public int add(PivotTable pivotTable, int row, int column, String tableName)
```


يضيف PivotTable جديدًا بناءً على PivotTable آخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable المصدر. |
| صف | int | فهرس الصف للخلية في الزاوية العلوية اليسرى لنطاق وجهة تقرير PivotTable. |
| عمود | int | فهرس العمود للخلية في الزاوية العلوية اليسرى لنطاق وجهة تقرير PivotTable. |
| tableName | java.lang.String | اسم تقرير PivotTable الجديد. |

**Returns:**
int - فهرس PivotTable المضاف حديثًا.
### add(PivotTable pivotTable, String destCellName, String tableName) {#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-}
```
public int add(PivotTable pivotTable, String destCellName, String tableName)
```


يضيف PivotTable جديدًا بناءً على PivotTable آخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable المصدر. |
| destCellName | java.lang.String | الخلية في الزاوية العلوية اليسرى لنطاق وجهة تقرير PivotTable. |
| tableName | java.lang.String | اسم تقرير PivotTable الجديد. |

**Returns:**
int - فهرس PivotTable المضاف حديثًا.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


يضيف عنصرًا إلى مثيل CollectionBase.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | الكائن لإضافته إلى مثيل CollectionBase. |

**Returns:**
int - الموضع الذي تم إدراج العنصر الجديد فيه.
### add(String sourceData, int row, int column) {#add-java.lang.String-int-int-}
```
public PivotTable add(String sourceData, int row, int column)
```


يضيف PivotTable حديثًا جديدًا (منذ Excel 2007) في الصف والعمود المحددين في ورقة العمل مع الخيارات الافتراضية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceData | java.lang.String | نطاق خلايا البيانات لـ PivotTable الجديد. مثال: Sheet1!A1:C8 |
| صف | int | فهرس الصف الصفري للزاوية العلوية اليسرى لوجهة PivotTable. |
| عمود | int | فهرس العمود الصفري للزاوية العلوية اليسرى لوجهة PivotTable. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, int row, int column, PivotTableCreateOptions options) {#add-java.lang.String-int-int-com.aspose.cells.PivotTableCreateOptions-}
```
public PivotTable add(String sourceData, int row, int column, PivotTableCreateOptions options)
```


يضيف PivotTable جديدًا في الصف والعمود المحددين في ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceData | java.lang.String | نطاق خلايا البيانات لـ PivotTable الجديد. مثال: Sheet1!A1:C8 |
| صف | int | فهرس الصف الصفري للزاوية العلوية اليسرى لوجهة PivotTable. |
| عمود | int | فهرس العمود الصفري للزاوية العلوية اليسرى لوجهة PivotTable. |
| options | [PivotTableCreateOptions](../../com.aspose.cells/pivottablecreateoptions) | خيارات إنشاء PivotTable. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, int row, int column, String tableName) {#add-java.lang.String-int-int-java.lang.String-}
```
public int add(String sourceData, int row, int column, String tableName)
```


يضيف PivotTable جديدًا بتنسيق ونمط Excel القديم (97-2003).

**Remarks**

ملاحظة: هذه الطريقة مهجورة. إنها تعادل استدعاء PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) مع `NewPivotTableOptions.IsXlsClassic = true`. يرجى استخدام نسخة PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا من سبتمبر 2026. نعتذر عن أي إزعاج.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceData | java.lang.String | نطاق خلايا البيانات لـ PivotTable الجديد. مثال: Sheet1!A1:C8 |
| صف | int | فهرس الصف للخلية في الزاوية العلوية اليسرى لنطاق وجهة تقرير PivotTable. |
| عمود | int | فهرس العمود للخلية في الزاوية العلوية اليسرى لنطاق وجهة تقرير PivotTable. |
| tableName | java.lang.String | اسم تقرير PivotTable الجديد. |

**Returns:**
int - الفهرس في قائمة جداول PivotTable هذه.
### add(String sourceData, int row, int column, String tableName, boolean useSameSource) {#add-java.lang.String-int-int-java.lang.String-boolean-}
```
public int add(String sourceData, int row, int column, String tableName, boolean useSameSource)
```


يضيف PivotTable جديدًا بتنسيق ونمط Excel القديم (97-2003).

**Remarks**

ملاحظة: هذه الطريقة مهجورة. إنها تعادل استدعاء PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) مع `NewPivotTableOptions.IsXlsClassic = true`. يرجى استخدام نسخة PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا من سبتمبر 2026. نعتذر عن أي إزعاج.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceData | java.lang.String | نطاق خلايا البيانات لـ PivotTable الجديد. مثال: Sheet1!A1:C8 |
| صف | int | فهرس الصف للخلية في الزاوية العلوية اليسرى لنطاق وجهة تقرير PivotTable. |
| عمود | int | فهرس العمود للخلية في الزاوية العلوية اليسرى لنطاق وجهة تقرير PivotTable. |
| tableName | java.lang.String | اسم تقرير PivotTable الجديد. |
| useSameSource | boolean | يشير إلى ما إذا كان يتم استخدام نفس مصدر البيانات عندما يكون جدول PivotTable آخر موجود قد استخدم هذا المصدر. إذا كانت الخاصية true، فستوفر الذاكرة. |

**Returns:**
int - فهرس الذاكرة المؤقتة المضاف حديثًا.
### add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic) {#add-java.lang.String-int-int-java.lang.String-boolean-boolean-}
```
public int add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic)
```


يضيف PivotTable جديدًا بتنسيق ونمط Excel القديم (97-2003).

**Remarks**

ملاحظة: هذه الطريقة قديمة. إنها تعادل استدعاء PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) مع `NewPivotTableOptions.IsXlsClassic = true`. يرجى استخدام overload PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا من أكتوبر 2026. نعتذر عن أي إزعاج.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceData | java.lang.String | نطاق خلايا البيانات لـ PivotTable الجديد. مثال: Sheet1!A1:C8 |
| صف | int | فهرس الصف للخلية في الزاوية العلوية اليسرى لنطاق وجهة تقرير PivotTable. |
| عمود | int | فهرس العمود للخلية في الزاوية العلوية اليسرى لنطاق وجهة تقرير PivotTable. |
| tableName | java.lang.String | اسم تقرير PivotTable الجديد. |
| useSameSource | boolean | يشير إلى ما إذا كان يتم استخدام نفس مصدر البيانات عندما يكون جدول PivotTable آخر موجود قد استخدم هذا المصدر. إذا كانت الخاصية true، فستوفر الذاكرة. |
| isXlsClassic | boolean | يشير إلى ما إذا كان يتم إضافة جدول محوري كلاسيكي لإصدار Excel 97-2003. |

**Returns:**
int - فهرس الذاكرة المؤقتة المضاف حديثًا.
### add(String sourceData, String cellName) {#add-java.lang.String-java.lang.String-}
```
public PivotTable add(String sourceData, String cellName)
```


يضيف PivotTable حديثًا جديدًا (منذ Excel 2007) في الصف والعمود المحددين في ورقة العمل مع الخيارات الافتراضية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceData | java.lang.String | نطاق خلايا البيانات لـ PivotTable الجديد. مثال: Sheet1!A1:C8 |
| cellName | java.lang.String | اسم الخلية الموجودة في الزاوية العلوية اليسرى لوجهة جدول PivotTable. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, String cellName, PivotTableCreateOptions options) {#add-java.lang.String-java.lang.String-com.aspose.cells.PivotTableCreateOptions-}
```
public PivotTable add(String sourceData, String cellName, PivotTableCreateOptions options)
```


يضيف PivotTable حديثًا جديدًا (منذ Excel 2007) في الصف والعمود المحددين في ورقة العمل مع الخيارات الافتراضية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceData | java.lang.String | نطاق خلايا البيانات لـ PivotTable الجديد. مثال: Sheet1!A1:C8 |
| cellName | java.lang.String | اسم الخلية الموجودة في الزاوية العلوية اليسرى لوجهة جدول PivotTable. |
| options | [PivotTableCreateOptions](../../com.aspose.cells/pivottablecreateoptions) | خيارات إنشاء جدول محوري. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, String destCellName, String tableName) {#add-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String sourceData, String destCellName, String tableName)
```


يضيف PivotTable جديدًا بتنسيق ونمط Excel القديم (97-2003).

**Remarks**

ملاحظة: هذه الطريقة مهجورة. إنها تعادل استدعاء PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) مع `NewPivotTableOptions.IsXlsClassic = true`. يرجى استخدام نسخة PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا من سبتمبر 2026. نعتذر عن أي إزعاج.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceData | java.lang.String | البيانات الخاصة بذاكرة التخزين المؤقت لجدول PivotTable الجديد. |
| destCellName | java.lang.String | الخلية في الزاوية العلوية اليسرى لنطاق وجهة تقرير PivotTable. |
| tableName | java.lang.String | اسم تقرير PivotTable الجديد. |

**Returns:**
int - الفهرس في قائمة جداول PivotTable هذه.
### add(String sourceData, String destCellName, String tableName, boolean useSameSource) {#add-java.lang.String-java.lang.String-java.lang.String-boolean-}
```
public int add(String sourceData, String destCellName, String tableName, boolean useSameSource)
```


يضيف PivotTable جديدًا بتنسيق ونمط Excel القديم (97-2003).

**Remarks**

ملاحظة: هذه الطريقة مهجورة. إنها تعادل استدعاء PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) مع `NewPivotTableOptions.IsXlsClassic = true`. يرجى استخدام نسخة PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا من سبتمبر 2026. نعتذر عن أي إزعاج.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceData | java.lang.String | البيانات الخاصة بذاكرة التخزين المؤقت لجدول PivotTable الجديد. |
| destCellName | java.lang.String | الخلية في الزاوية العلوية اليسرى لنطاق وجهة تقرير PivotTable. |
| tableName | java.lang.String | اسم تقرير PivotTable الجديد. |
| useSameSource | boolean | يشير إلى ما إذا كان يتم استخدام نفس مصدر البيانات عندما يكون جدول PivotTable آخر موجود قد استخدم هذا المصدر. إذا كانت الخاصية true، فستوفر الذاكرة. |

**Returns:**
int - فهرس الذاكرة المؤقتة المضاف حديثًا.
### add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic) {#add-java.lang.String-java.lang.String-java.lang.String-boolean-boolean-}
```
public int add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic)
```


يضيف PivotTable جديدًا.

**Remarks**

ملاحظة: هذه الطريقة قديمة. إنها تعادل استدعاء PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) مع `NewPivotTableOptions.IsXlsClassic = true`. يرجى استخدام overload PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا من أكتوبر 2026. نعتذر عن أي إزعاج.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceData | java.lang.String | نطاق خلايا البيانات لـ PivotTable الجديد. مثال: Sheet1!A1:C8 |
| خلية | java.lang.String | الخلية في الزاوية العلوية اليسرى لنطاق وجهة تقرير PivotTable. |
| tableName | java.lang.String | اسم تقرير PivotTable الجديد. |
| useSameSource | boolean | يشير إلى ما إذا كان يتم استخدام مصدر البيانات نفسه عندما يكون جدول محوري آخر قد استخدم هذا المصدر. إذا كانت الخاصية true، سيوفر ذلك الذاكرة عندما يتم تجميع مصدر البيانات نفسه في ذاكرة تخزين مؤقت واحدة للجدول المحوري. |
| isXlsClassic | boolean | يشير إلى ما إذا كان يتم إضافة جدول محوري كلاسيكي لإصدار Excel 97-2003. |

**Returns:**
int - فهرس الذاكرة المؤقتة المضاف حديثًا.
### add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName) {#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-int-int-java.lang.String-}
```
public int add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName)
```


يضيف كائن PivotTable جديد إلى المجموعة مع نطاقات دمج متعددة كمصدر للبيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceData | java.lang.String[] | نطاقات التجميع المتعددة، مثل \{"Sheet1!A1:C8","Sheet2!A1:B8"\} |
| isAutoPage | boolean | ما إذا كان يتم إنشاء حقل صفحة واحد تلقائيًا. إذا كان true، سيتم تجاهل المعامل التالي pageFields. |
| pageFields | [PivotPageFields](../../com.aspose.cells/pivotpagefields) | عناصر حقل صفحة الجدول المحوري. |
| صف | int | فهرس الصف للخلية في الزاوية العلوية اليسرى لنطاق وجهة تقرير PivotTable. |
| عمود | int | فهرس العمود للخلية في الزاوية العلوية اليسرى لنطاق وجهة تقرير PivotTable. |
| tableName | java.lang.String | اسم تقرير PivotTable الجديد. |

**Returns:**
int - فهرس PivotTable المضاف حديثًا.
### add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName) {#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-java.lang.String-java.lang.String-}
```
public int add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName)
```


يضيف كائن PivotTable جديد إلى المجموعة مع نطاقات دمج متعددة كمصدر للبيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceData | java.lang.String[] | نطاقات التجميع المتعددة، مثل \{"Sheet1!A1:C8","Sheet2!A1:B8"\} |
| isAutoPage | boolean | ما إذا كان يتم إنشاء حقل صفحة واحد تلقائيًا. إذا كان true، سيتم تجاهل المعامل التالي pageFields. |
| pageFields | [PivotPageFields](../../com.aspose.cells/pivotpagefields) | عناصر حقل صفحة الجدول المحوري. |
| destCellName | java.lang.String | destCellName اسم التقرير الجديد لجدول PivotTable. |
| tableName | java.lang.String | اسم التقرير الجديد لجدول PivotTable. |

**Returns:**
int - فهرس PivotTable المضاف حديثًا.
### clear() {#clear--}
```
public void clear()
```


يمسح جميع جداول PivotTable.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


إرجاع ما إذا كان المثيل يحتوي على هذا الكائن

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | كائن اختبار |

**Returns:**
boolean - ما إذا كان المثيل يحتوي على هذا الكائن
### dispose() {#dispose--}
```
public void dispose()
```


ينفذ مهام محددة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة ضبط الموارد غير المُدارة.

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
### get(int index) {#get-int-}
```
public PivotTable get(int index)
```


يحصل على تقرير PivotTable حسب الفهرس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
### get(int row, int column) {#get-int-int-}
```
public PivotTable get(int row, int column)
```


يحصل على [PivotTable](../../com.aspose.cells/pivottable) الموجود في الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int |  |
| عمود | int |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
### get(String name) {#get-java.lang.String-}
```
public PivotTable get(String name)
```


يحصل على تقرير PivotTable حسب اسم PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


يحصل على عدد العناصر الموجودة في مثيل CollectionBase.

**Returns:**
int - عدد العناصر الموجودة في مثيل CollectionBase.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


يحدد فهرس عنصر محدد في مثيل CollectionBase.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | يحدد فهرس عنصر محدد في مثيل CollectionBase. |

**Returns:**
int - فهرس القيمة إذا وجد في القائمة؛ وإلا -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


يرجع كائن تعداد يتنقل عبر مثيل CollectionBase.

**Returns:**
java.util.Iterator - كائن تكرار لمثيل CollectionBase.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(PivotTable pivotTable) {#remove-com.aspose.cells.PivotTable-}
```
public void remove(PivotTable pivotTable)
```


يحذف PivotTable المحدد ويحذف بيانات PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |

### remove(PivotTable pivotTable, boolean keepData) {#remove-com.aspose.cells.PivotTable-boolean-}
```
public void remove(PivotTable pivotTable, boolean keepData)
```


يحذف PivotTable المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |
| keepData | boolean | ما إذا كان يجب الاحتفاظ ببيانات جدول PivotTable |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


يحذف PivotTable في الفهرس المحدد ويحذف بيانات PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس الموضع في مجموعة PivotTable |

### removeAt(int index, boolean keepData) {#removeAt-int-boolean-}
```
public void removeAt(int index, boolean keepData)
```


يحذف PivotTable في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس الموضع في مجموعة PivotTable |
| keepData | boolean | ما إذا كان يجب الاحتفاظ ببيانات جدول PivotTable |

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

