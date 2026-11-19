---
title: "SlicerCache"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل وصفًا ملخصًا لذاكرة التخزين المؤقت للمقسم"
type: docs
url: /ar/java/com.aspose.cells/slicercache/
---

**Inheritance:**
java.lang.Object
```
public class SlicerCache
```

يمثل وصفًا ملخصًا لذاكرة التخزين المؤقت للمقسم

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
 
         //Add a PivotTable
         PivotTable pivot = pivots.add("=Sheet1!A1:C5", "A12");
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         pivot.calculateData();
 
         SlicerCollection slicers = sheet.getSlicers();
         int slicerIndex = slicers.add(pivot, "E12", "fruit");
         Slicer slicer = slicers.get(slicerIndex);
         slicer.setStyleType(SlicerStyleType.SLICER_STYLE_LIGHT_2);
 
         //Get SlicerCache object of current slicer
         SlicerCache slicerCache = slicer.getSlicerCache();
 
         //do your business
 
         book.save("out.xlsx");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCrossFilterType()](#getCrossFilterType--) | يشير إلى كيفية إظهار العناصر التي لا تحتوي على بيانات من slicer. |
| [getList()](#getList--) | يشير إلى ما إذا كان slicer المرتبط بـ slicer cache المحدد يعتمد على مصدر بيانات غير OLAP. |
| [getName()](#getName--) | يرجع اسم slicer cache. |
| [getSlicerCacheItems()](#getSlicerCacheItems--) | يرجع مجموعة SlicerCacheItem التي تحتوي على مجموعة جميع العناصر في slicer cache. |
| [getSourceName()](#getSourceName--) | يرجع اسم هذا slicer cache. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCrossFilterType(int value)](#setCrossFilterType-int-) | يشير إلى كيفية إظهار العناصر التي لا تحتوي على بيانات من slicer. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getCrossFilterType() {#getCrossFilterType--}
```
public int getCrossFilterType()
```


يشير إلى كيفية إظهار العناصر التي لا تحتوي على بيانات من slicer.

انظر [SlicerCacheCrossFilterType](../../com.aspose.cells/slicercachecrossfiltertype).

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية [Slicer.getShowTypeOfItemsWithNoData()](../../com.aspose.cells/slicer\#getShowTypeOfItemsWithNoData--) . ستتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getList() {#getList--}
```
public boolean getList()
```


يشير إلى ما إذا كان slicer المرتبط بـ slicer cache المحدد يعتمد على مصدر بيانات غير OLAP.

**Example**

```
         System.out.println(slicerCache.getList());
```

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


يرجع اسم slicer cache.

**Example**

```
         //get the name of the slicer cache.
         System.out.println(slicerCache.getName());
```

**Returns:**
java.lang.String
### getSlicerCacheItems() {#getSlicerCacheItems--}
```
public SlicerCacheItemCollection getSlicerCacheItems()
```


يعيد مجموعة SlicerCacheItem التي تحتوي على مجموعة جميع العناصر في ذاكرة التخزين المؤقت للمقسم. للقراءة فقط

**Example**

```
         //get SlicerCacheItem collection that contains the collection of all items in the slicer cache.
         SlicerCacheItemCollection slicerCacheItems = slicerCache.getSlicerCacheItems();
         System.out.println(slicerCacheItems.getCount());
```

**Returns:**
[SlicerCacheItemCollection](../../com.aspose.cells/slicercacheitemcollection)
### getSourceName() {#getSourceName--}
```
public String getSourceName()
```


يرجع اسم هذا slicer cache.

**Example**

```
         //get the name of this slicer cache.
         System.out.println(slicerCache.getSourceName());
```

**Returns:**
java.lang.String
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




### setCrossFilterType(int value) {#setCrossFilterType-int-}
```
public void setCrossFilterType(int value)
```


يشير إلى كيفية إظهار العناصر التي لا تحتوي على بيانات من slicer.

انظر [SlicerCacheCrossFilterType](../../com.aspose.cells/slicercachecrossfiltertype).

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية [Slicer.getShowTypeOfItemsWithNoData()](../../com.aspose.cells/slicer\#getShowTypeOfItemsWithNoData--) . ستتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

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

