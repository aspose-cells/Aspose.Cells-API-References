---
title: "SlicerCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يحدد مجموعة جميع كائنات Slicer في ورقة العمل المحددة."
type: docs
url: /ar/java/com.aspose.cells/slicercollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SlicerCollection extends CollectionBase
```

يحدد مجموعة جميع كائنات Slicer في ورقة العمل المحددة.

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
 
         pivot.calculateData();
 
         SlicerCollection slicers = sheet.getSlicers();
         int slicerIndex = slicers.add(pivot, "E12", "fruit");
         Slicer slicer = slicers.get(slicerIndex);
 
         //do your business
 
         book.save("out.xlsx");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(ListObject table, ListColumn listColumn, int row, int column)](#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-int-int-) | أضف مقطعًا جديدًا باستخدام ListObjet كمصدر بيانات |
| [add(ListObject table, ListColumn listColumn, String destCellName)](#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-java.lang.String-) | أضف مقطعًا جديدًا باستخدام ListObjet كمصدر بيانات |
| [add(ListObject table, int index, String destCellName)](#add-com.aspose.cells.ListObject-int-java.lang.String-) | أضف مقطعًا جديدًا باستخدام ListObjet كمصدر بيانات |
| [add(PivotTable pivot, int row, int column, PivotField baseField)](#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-) | أضف مقطعًا جديدًا باستخدام PivotTable كمصدر بيانات |
| [add(PivotTable pivot, int row, int column, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-int-int-int-) | أضف مقطعًا جديدًا باستخدام PivotTable كمصدر بيانات |
| [add(PivotTable pivot, int row, int column, String baseFieldName)](#add-com.aspose.cells.PivotTable-int-int-java.lang.String-) | أضف مقطعًا جديدًا باستخدام PivotTable كمصدر بيانات |
| [add(PivotTable pivot, String destCellName, PivotField baseField)](#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-) | أضف مقطعًا جديدًا باستخدام PivotTable كمصدر بيانات |
| [add(PivotTable pivot, String destCellName, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-java.lang.String-int-) | أضف مقطعًا جديدًا باستخدام PivotTable كمصدر بيانات |
| [add(PivotTable pivot, String destCellName, String baseFieldName)](#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-) | أضف مقطعًا جديدًا باستخدام PivotTable كمصدر بيانات |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [clear()](#clear--) | امسح جميع المقاطع. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على المقطع حسب الفهرس. |
| [get(String name)](#get-java.lang.String-) | يحصل على المقطع حسب اسم المقطع. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في مثيل CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | يحدد فهرس عنصر محدد في مثيل CollectionBase. |
| [iterator()](#iterator--) | يرجع كائن تعداد يتنقل عبر مثيل CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Slicer slicer)](#remove-com.aspose.cells.Slicer-) | إزالة المقطع المحدد |
| [removeAt(int index)](#removeAt-int-) | يحذف المقطع في الفهرس المحدد |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(ListObject table, ListColumn listColumn, int row, int column) {#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-int-int-}
```
public int add(ListObject table, ListColumn listColumn, int row, int column)
```


أضف مقطعًا جديدًا باستخدام ListObjet كمصدر بيانات

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | ListObject object |
| listColumn | [ListColumn](../../com.aspose.cells/listcolumn) | عمود القائمة في ListObject.ListColumns |
| صف | int | فهرس الصف للخلية في الزاوية العلوية اليسرى لنطاق المقطع. |
| عمود | int | فهرس العمود للخلية في الزاوية العلوية اليسرى لنطاق المقطع. |

**Returns:**
int - فهرس المقطع الجديد المضاف
### add(ListObject table, ListColumn listColumn, String destCellName) {#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-java.lang.String-}
```
public int add(ListObject table, ListColumn listColumn, String destCellName)
```


أضف مقطعًا جديدًا باستخدام ListObjet كمصدر بيانات

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | ListObject object |
| listColumn | [ListColumn](../../com.aspose.cells/listcolumn) | عمود القائمة في ListObject.ListColumns |
| destCellName | java.lang.String | الخلية في الزاوية العلوية اليسرى لنطاق المقطع. |

**Returns:**
int - فهرس المقطع الجديد المضاف
### add(ListObject table, int index, String destCellName) {#add-com.aspose.cells.ListObject-int-java.lang.String-}
```
public int add(ListObject table, int index, String destCellName)
```


أضف مقطعًا جديدًا باستخدام ListObjet كمصدر بيانات

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | ListObject object |
| الفهرس | int | فهرس ListColumn في ListObject.ListColumns |
| destCellName | java.lang.String | الخلية في الزاوية العلوية اليسرى لنطاق المقطع. |

**Returns:**
int - فهرس المقطع الجديد المضاف
### add(PivotTable pivot, int row, int column, PivotField baseField) {#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, int row, int column, PivotField baseField)
```


أضف مقطعًا جديدًا باستخدام PivotTable كمصدر بيانات

**Example**

```
         slicers.add(pivot, 3, 12, pivot.getBaseFields().get(0));
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |
| صف | int | فهرس الصف للخلية في الزاوية العلوية اليسرى لنطاق المقطع. |
| عمود | int | فهرس العمود للخلية في الزاوية العلوية اليسرى لنطاق المقطع. |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | حقل PivotField في PivotTable.BaseFields |

**Returns:**
int - فهرس المقطع الجديد المضاف
### add(PivotTable pivot, int row, int column, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-int-int-int-}
```
public int add(PivotTable pivot, int row, int column, int baseFieldIndex)
```


أضف مقطعًا جديدًا باستخدام PivotTable كمصدر بيانات

**Example**

```
         slicers.add(pivot, 20, 8, 0);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |
| صف | int | فهرس الصف للخلية في الزاوية العلوية اليسرى لنطاق المقطع. |
| عمود | int | فهرس العمود للخلية في الزاوية العلوية اليسرى لنطاق المقطع. |
| baseFieldIndex | int | المؤشر لـ PivotField في PivotTable.BaseFields |

**Returns:**
int - فهرس المقطع الجديد المضاف
### add(PivotTable pivot, int row, int column, String baseFieldName) {#add-com.aspose.cells.PivotTable-int-int-java.lang.String-}
```
public int add(PivotTable pivot, int row, int column, String baseFieldName)
```


أضف مقطعًا جديدًا باستخدام PivotTable كمصدر بيانات

**Example**

```
         slicers.add(pivot, 20, 12, "fruit");
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |
| صف | int | فهرس الصف للخلية في الزاوية العلوية اليسرى لنطاق المقطع. |
| عمود | int | فهرس العمود للخلية في الزاوية العلوية اليسرى لنطاق المقطع. |
| baseFieldName | java.lang.String | اسم PivotField في PivotTable.BaseFields |

**Returns:**
int - فهرس المقطع الجديد المضاف
### add(PivotTable pivot, String destCellName, PivotField baseField) {#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, String destCellName, PivotField baseField)
```


أضف مقطعًا جديدًا باستخدام PivotTable كمصدر بيانات

**Example**

```
         slicers.add(pivot, "I3", pivot.getBaseFields().get(0));
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |
| destCellName | java.lang.String | الخلية في الزاوية العلوية اليسرى لنطاق المقطع. |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | حقل PivotField في PivotTable.BaseFields |

**Returns:**
int - فهرس المقطع الجديد المضاف
### add(PivotTable pivot, String destCellName, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-java.lang.String-int-}
```
public int add(PivotTable pivot, String destCellName, int baseFieldIndex)
```


أضف مقطعًا جديدًا باستخدام PivotTable كمصدر بيانات

**Example**

```
         slicers.add(pivot, "E20", 0);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |
| destCellName | java.lang.String | الخلية في الزاوية العلوية اليسرى لنطاق المقطع. |
| baseFieldIndex | int | المؤشر لـ PivotField في PivotTable.BaseFields |

**Returns:**
int - فهرس المقطع الجديد المضاف
### add(PivotTable pivot, String destCellName, String baseFieldName) {#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-}
```
public int add(PivotTable pivot, String destCellName, String baseFieldName)
```


أضف مقطعًا جديدًا باستخدام PivotTable كمصدر بيانات

**Example**

```
         slicers.add(pivot, "E3", "fruit");
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable object |
| destCellName | java.lang.String | الخلية في الزاوية العلوية اليسرى لنطاق المقطع. |
| baseFieldName | java.lang.String | اسم PivotField في PivotTable.BaseFields |

**Returns:**
int - فهرس المقطع الجديد المضاف
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


امسح جميع المقاطع.

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
public Slicer get(int index)
```


يحصل على المقطع حسب الفهرس.

**Example**

```
         Slicer slicerByIndex = slicers.get(0);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int |  |

**Returns:**
[Slicer](../../com.aspose.cells/slicer)
### get(String name) {#get-java.lang.String-}
```
public Slicer get(String name)
```


يحصل على المقطع حسب اسم المقطع.

**Example**

```
         Slicer slicerByName = slicers.get("fruit");
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[Slicer](../../com.aspose.cells/slicer)
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




### remove(Slicer slicer) {#remove-com.aspose.cells.Slicer-}
```
public void remove(Slicer slicer)
```


إزالة المقطع المحدد

**Example**

```
         Slicer delSlicer = slicers.get(0);
         slicers.remove(delSlicer);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| slicer | [Slicer](../../com.aspose.cells/slicer) | كائن Slicer |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


يحذف المقطع في الفهرس المحدد

**Example**

```
         slicers.removeAt(1);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | مؤشر الموضع في مجموعة Slicer |

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

