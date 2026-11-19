---
title: "GridHyperlinkCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على مجموعة من الكائنات."
type: docs
url: /ar/java/com.aspose.gridweb/gridhyperlinkcollection/
---

**Inheritance:**
java.lang.Object
```
public class GridHyperlinkCollection
```

يحتوي على مجموعة من كائنات [GridHyperlink](../../com.aspose.gridweb/gridhyperlink).
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)](#add-int-int-int-int-java.lang.String-) | يضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا. |
| [add(String cellName, int totalRows, int totalColumns, String address)](#add-java.lang.String-int-int-java.lang.String-) | يضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا. |
| [add(String cellName, String address)](#add-java.lang.String-java.lang.String-) | يضيف ارتباطًا تشعبيًا إلى خلية محددة. |
| [add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)](#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | يضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا. |
| [clear()](#clear--) | يمسح جميع الارتباطات التشعبية. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على عنصر [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) في الفهرس المحدد. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على حجم المُعدد |
| [getHyperlink(GridCell cell)](#getHyperlink-com.aspose.gridweb.GridCell-) | يحصل على كائن الارتباط التشعبي للخلية. |
| [getHyperlink(int row, int column)](#getHyperlink-int-int-) | يحصل على كائن الارتباط التشعبي للخلية. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(GridCellArea area)](#remove-com.aspose.gridweb.GridCellArea-) | إزالة الارتباط التشعبي في المنطقة المحددة. |
| [removeAt(int index)](#removeAt-int-) | إزالة الارتباط التشعبي في الفهرس المحدد. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address) {#add-int-int-int-int-java.lang.String-}
```
public int add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)
```


يضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | int | الصف الأول لنطاق الارتباط التشعبي. |
| firstColumn | int | العمود الأول لنطاق الارتباط التشعبي. |
| totalRows | int | عدد الصفوف في نطاق الارتباط التشعبي هذا. |
| totalColumns | int | عدد الأعمدة في نطاق الارتباط التشعبي هذا. |
| العنوان | java.lang.String | عنوان الارتباط التشعبي. |

**Returns:**
int - فهرس كائن [GridHyperlink](../../com.aspose.gridweb/gridhyperlink).
### add(String cellName, int totalRows, int totalColumns, String address) {#add-java.lang.String-int-int-java.lang.String-}
```
public int add(String cellName, int totalRows, int totalColumns, String address)
```


يضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | java.lang.String | اسم الخلية. |
| totalRows | int | عدد الصفوف في نطاق الارتباط التشعبي هذا. |
| totalColumns | int | عدد الأعمدة في نطاق الارتباط التشعبي هذا. |
| العنوان | java.lang.String | عنوان الارتباط التشعبي. |

**Returns:**
int - فهرس كائن [GridHyperlink](../../com.aspose.gridweb/gridhyperlink).
### add(String cellName, String address) {#add-java.lang.String-java.lang.String-}
```
public int add(String cellName, String address)
```


يضيف ارتباطًا تشعبيًا إلى خلية محددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | java.lang.String | اسم الخلية. |
| العنوان | java.lang.String | عنوان الارتباط التشعبي. |

**Returns:**
int - فهرس كائن [GridHyperlink](../../com.aspose.gridweb/gridhyperlink).
### add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip) {#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)
```


يضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startCellName | java.lang.String | الخلية العلوية اليسرى للنطاق. |
| endCellName | java.lang.String | الخلية السفلية اليمنى للنطاق. |
| العنوان | java.lang.String | عنوان الارتباط التشعبي. |
| textToDisplay | java.lang.String | النص الذي سيُعرض للرابط المحدد. |
| screenTip | java.lang.String | نص تلميح الشاشة للرابط المحدد. |

**Returns:**
int - فهرس كائن [GridHyperlink](../../com.aspose.gridweb/gridhyperlink).
### clear() {#clear--}
```
public void clear()
```


يمسح جميع الارتباطات التشعبية.

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
public GridHyperlink get(int index)
```


يحصل على عنصر [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس الصفري للعنصر. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - The element at the specified index.
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
### getHyperlink(GridCell cell) {#getHyperlink-com.aspose.gridweb.GridCell-}
```
public GridHyperlink getHyperlink(GridCell cell)
```


يحصل على كائن الارتباط التشعبي للخلية. إذا لم يكن هناك ارتباط تشعبي للخلية، يرجع null.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cell | [GridCell](../../com.aspose.gridweb/gridcell) | كائن GridCell. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) the GridHyperlink object.
### getHyperlink(int row, int column) {#getHyperlink-int-int-}
```
public GridHyperlink getHyperlink(int row, int column)
```


يحصل على كائن الارتباط التشعبي للخلية. إذا لم يكن هناك ارتباط تشعبي للخلية، يرجع null.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | صف الخلية. |
| عمود | int | عمود الخلية. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) the GridHyperlink object.
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




### remove(GridCellArea area) {#remove-com.aspose.gridweb.GridCellArea-}
```
public void remove(GridCellArea area)
```


إزالة الارتباط التشعبي في المنطقة المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | المنطقة التي تحتوي على الارتباط التشعبي. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


إزالة الارتباط التشعبي في الفهرس المحدد.

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

