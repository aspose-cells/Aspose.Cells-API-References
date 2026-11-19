---
title: "TimelineCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يحدد مجموعة جميع الكائنات على ورقة العمل."
type: docs
url: /ar/java/com.aspose.cells/timelinecollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class TimelineCollection extends CollectionBase
```

يحدد مجموعة جميع كائنات [Timeline](../../com.aspose.cells/timeline) على ورقة العمل. كان مدعومًا منذ Excel 2013.

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
 
         //Create date style
         Style dateStyle = new CellsFactory().createStyle();
         dateStyle.setCustom("m/d/yyyy");
         cells.get(0, 1).setValue("date");
         cells.get(1, 1).setValue(new DateTime(2021, 2, 5));
         cells.get(2, 1).setValue(new DateTime(2022, 3, 8));
         cells.get(3, 1).setValue(new DateTime(2023, 4, 10));
         cells.get(4, 1).setValue(new DateTime(2024, 5, 16));
         //Set date style
         cells.get(1, 1).setStyle(dateStyle);
         cells.get(2, 1).setStyle(dateStyle);
         cells.get(3, 1).setStyle(dateStyle);
         cells.get(4, 1).setStyle(dateStyle);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
 
         PivotTableCollection pivots = sheet.getPivotTables();
         //Add a PivotTable
         PivotTable pivot = pivots.add("=Sheet1!A1:C5", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "date");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(PivotTable pivot, int row, int column, PivotField baseField)](#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-) | إضافة مخطط زمني جديد باستخدام PivotTable كمصدر بيانات |
| [add(PivotTable pivot, int row, int column, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-int-int-int-) | إضافة مخطط زمني جديد باستخدام PivotTable كمصدر بيانات |
| [add(PivotTable pivot, int row, int column, String baseFieldName)](#add-com.aspose.cells.PivotTable-int-int-java.lang.String-) | إضافة مخطط زمني جديد باستخدام PivotTable كمصدر بيانات |
| [add(PivotTable pivot, String destCellName, PivotField baseField)](#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-) | إضافة مخطط زمني جديد باستخدام PivotTable كمصدر بيانات |
| [add(PivotTable pivot, String destCellName, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-java.lang.String-int-) | إضافة مخطط زمني جديد باستخدام PivotTable كمصدر بيانات |
| [add(PivotTable pivot, String destCellName, String baseFieldName)](#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-) | إضافة مخطط زمني جديد باستخدام PivotTable كمصدر بيانات |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [clear()](#clear--) | يزيل جميع الكائنات من مثيل CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على المخطط الزمني حسب الفهرس. |
| [get(String name)](#get-java.lang.String-) | يحصل على المخطط الزمني حسب اسم المخطط الزمني. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في مثيل CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | يحدد فهرس عنصر محدد في مثيل CollectionBase. |
| [iterator()](#iterator--) | يرجع كائن تعداد يتنقل عبر مثيل CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | يزيل العنصر في الفهرس المحدد. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(PivotTable pivot, int row, int column, PivotField baseField) {#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, int row, int column, PivotField baseField)
```


إضافة مخطط زمني جديد باستخدام PivotTable كمصدر بيانات

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, 20, 5, pivot.getBaseFields().get(1));
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |
| صف | int | فهرس الصف للخلية في الزاوية العلوية اليسرى لنطاق المخطط الزمني. |
| عمود | int | فهرس العمود للخلية في الزاوية العلوية اليسرى لنطاق المخطط الزمني. |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | حقل PivotField في PivotTable.BaseFields |

**Returns:**
int - فهرس المخطط الزمني الجديد المضاف
### add(PivotTable pivot, int row, int column, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-int-int-int-}
```
public int add(PivotTable pivot, int row, int column, int baseFieldIndex)
```


إضافة مخطط زمني جديد باستخدام PivotTable كمصدر بيانات

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, 15, 5, 1);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |
| صف | int | فهرس الصف للخلية في الزاوية العلوية اليسرى لنطاق المخطط الزمني. |
| عمود | int | فهرس العمود للخلية في الزاوية العلوية اليسرى لنطاق المخطط الزمني. |
| baseFieldIndex | int | المؤشر لـ PivotField في PivotTable.BaseFields |

**Returns:**
int - فهرس المخطط الزمني الجديد المضاف
### add(PivotTable pivot, int row, int column, String baseFieldName) {#add-com.aspose.cells.PivotTable-int-int-java.lang.String-}
```
public int add(PivotTable pivot, int row, int column, String baseFieldName)
```


إضافة مخطط زمني جديد باستخدام PivotTable كمصدر بيانات

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, 10, 5, "date");
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |
| صف | int | فهرس الصف للخلية في الزاوية العلوية اليسرى لنطاق المخطط الزمني. |
| عمود | int | فهرس العمود للخلية في الزاوية العلوية اليسرى لنطاق المخطط الزمني. |
| baseFieldName | java.lang.String | اسم PivotField في PivotTable.BaseFields |

**Returns:**
int - فهرس المخطط الزمني الجديد المضاف
### add(PivotTable pivot, String destCellName, PivotField baseField) {#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, String destCellName, PivotField baseField)
```


إضافة مخطط زمني جديد باستخدام PivotTable كمصدر بيانات

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, "i10", pivot.getBaseFields().get(1));
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |
| destCellName | java.lang.String | اسم الخلية في الزاوية العلوية اليسرى لنطاق المخطط الزمني. |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | حقل PivotField في PivotTable.BaseFields |

**Returns:**
int - فهرس المخطط الزمني الجديد المضاف
### add(PivotTable pivot, String destCellName, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-java.lang.String-int-}
```
public int add(PivotTable pivot, String destCellName, int baseFieldIndex)
```


إضافة مخطط زمني جديد باستخدام PivotTable كمصدر بيانات

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, "i5", 1);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |
| destCellName | java.lang.String | اسم الخلية في الزاوية العلوية اليسرى لنطاق المخطط الزمني. |
| baseFieldIndex | int | المؤشر لـ PivotField في PivotTable.BaseFields |

**Returns:**
int - فهرس المخطط الزمني الجديد المضاف
### add(PivotTable pivot, String destCellName, String baseFieldName) {#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-}
```
public int add(PivotTable pivot, String destCellName, String baseFieldName)
```


إضافة مخطط زمني جديد باستخدام PivotTable كمصدر بيانات

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, "i15", "date");
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |
| destCellName | java.lang.String | اسم الخلية في الزاوية العلوية اليسرى لنطاق المخطط الزمني. |
| baseFieldName | java.lang.String | اسم PivotField في PivotTable.BaseFields |

**Returns:**
int - فهرس المخطط الزمني الجديد المضاف
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
### clear() {#clear--}
```
public void clear()
```


يزيل جميع الكائنات من مثيل CollectionBase.

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
public Timeline get(int index)
```


يحصل على المخطط الزمني حسب الفهرس.

**Example**

```
         //Get the Timeline by index.
         Timeline objByIndex = sheet.getTimelines().get(0);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int |  |

**Returns:**
[Timeline](../../com.aspose.cells/timeline)
### get(String name) {#get-java.lang.String-}
```
public Timeline get(String name)
```


يحصل على المخطط الزمني حسب اسم المخطط الزمني.

**Example**

```
         //Get the Timeline by Timeline's name.
         Timeline objByName = sheet.getTimelines().get("date");
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[Timeline](../../com.aspose.cells/timeline)
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




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


يزيل العنصر في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس الصفري للعنصر المراد إزالته. |

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

