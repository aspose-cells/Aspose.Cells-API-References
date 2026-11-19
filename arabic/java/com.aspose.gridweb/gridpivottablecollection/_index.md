---
title: "GridPivotTableCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على مجموعة من الكائنات."
type: docs
url: /ar/java/com.aspose.gridweb/gridpivottablecollection/
---

**Inheritance:**
java.lang.Object
```
public class GridPivotTableCollection
```

يحتوي على مجموعة من كائنات [GridPivotTable](../../com.aspose.gridweb/gridpivottable).
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName)](#add-com.aspose.gridweb.GridWorksheet-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-) | يضيف ذاكرة تخزين مؤقت PivotTable جديدة إلى مجموعة PivotCaches. |
| [add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName)](#add-java.lang.String-com.aspose.gridweb.GridCellArea-int-int-java.lang.String-) | يضيف ذاكرة تخزين مؤقت PivotTable جديدة إلى مجموعة PivotCaches. |
| [add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName)](#add-java.lang.String-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-) | يضيف ذاكرة تخزين مؤقت PivotTable جديدة إلى مجموعة PivotCaches. |
| [add(String sourceData, String destCellName, String tableName)](#add-java.lang.String-java.lang.String-java.lang.String-) | يضيف ذاكرة تخزين مؤقت PivotTable جديدة إلى مجموعة PivotCaches. |
| [clear()](#clear--) | يمسح جميع PivotTables. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على عنصر [GridPivotTable](../../com.aspose.gridweb/gridpivottable) عند الفهرس المحدد. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على حجم المُعدد |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | إزالة PivotTable عند الفهرس المحدد. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName) {#add-com.aspose.gridweb.GridWorksheet-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-}
```
public int add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName)
```


يضيف ذاكرة تخزين مؤقت PivotTable جديدة إلى مجموعة PivotCaches.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceSheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | ورقة العمل المصدر. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | المنطقة في ورقة العمل المصدر. |
| destCellName | java.lang.String | الخلية في الزاوية العلوية اليسرى لنطاق وجهة تقرير PivotTable. |
| tableName | java.lang.String | اسم تقرير PivotTable الجديد. |

**Returns:**
int - فهرس الذاكرة المؤقتة المضاف حديثًا.
### add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName) {#add-java.lang.String-com.aspose.gridweb.GridCellArea-int-int-java.lang.String-}
```
public int add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName)
```


يضيف ذاكرة تخزين مؤقت PivotTable جديدة إلى مجموعة PivotCaches.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| worksheetname | java.lang.String | اسم ورقة العمل المصدر. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | المنطقة في ورقة العمل المصدر. |
| destRow | int | صف الخلية في الزاوية العلوية اليسرى لنطاق وجهة تقرير PivotTable. |
| destCol | int | عمود الخلية في الزاوية العلوية اليسرى لنطاق وجهة تقرير PivotTable. |
| tableName | java.lang.String | اسم تقرير PivotTable الجديد. |

**Returns:**
int - فهرس الذاكرة المؤقتة المضاف حديثًا.
### add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName) {#add-java.lang.String-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-}
```
public int add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName)
```


يضيف ذاكرة تخزين مؤقت PivotTable جديدة إلى مجموعة PivotCaches.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| worksheetname | java.lang.String | اسم ورقة العمل المصدر. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | المنطقة في ورقة العمل المصدر. |
| destCellName | java.lang.String | الخلية في الزاوية العلوية اليسرى لنطاق وجهة تقرير PivotTable. |
| tableName | java.lang.String | اسم تقرير PivotTable الجديد. |

**Returns:**
int - فهرس الذاكرة المؤقتة المضاف حديثًا.
### add(String sourceData, String destCellName, String tableName) {#add-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String sourceData, String destCellName, String tableName)
```


يضيف ذاكرة تخزين مؤقت PivotTable جديدة إلى مجموعة PivotCaches.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceData | java.lang.String | نطاق خلايا البيانات لـ PivotTable الجديد. مثال: Sheet1!A1:C8 |
| destCellName | java.lang.String | الخلية في الزاوية العلوية اليسرى لنطاق وجهة تقرير PivotTable. |
| tableName | java.lang.String | اسم تقرير PivotTable الجديد. |

**Returns:**
int - فهرس الذاكرة المؤقتة المضاف حديثًا.
### clear() {#clear--}
```
public void clear()
```


يمسح جميع PivotTables.

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
public GridPivotTable get(int index)
```


يحصل على عنصر [GridPivotTable](../../com.aspose.gridweb/gridpivottable) عند الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس الصفري للعنصر. |

**Returns:**
[GridPivotTable](../../com.aspose.gridweb/gridpivottable) - The element at the specified index.
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


يحصل على حجم المُعدد

**Returns:**
int
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




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


إزالة PivotTable عند الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس الصفري للعنصر. |

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

