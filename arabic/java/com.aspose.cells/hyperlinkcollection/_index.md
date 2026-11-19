---
title: "HyperlinkCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على مجموعة من الكائنات."
type: docs
url: /ar/java/com.aspose.cells/hyperlinkcollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class HyperlinkCollection extends CollectionBase
```

يغلف مجموعة من كائنات [Hyperlink](../../com.aspose.cells/hyperlink).

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Get Hyperlinks Collection
         HyperlinkCollection hyperlinks = worksheet.getHyperlinks();
 
         //Adding a hyperlink to a URL at "A1" cell
         hyperlinks.add("A1", 1, 1, "http://www.aspose.com");
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)](#add-int-int-int-int-java.lang.String-) | يضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا. |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [add(String cellName, int totalRows, int totalColumns, String address)](#add-java.lang.String-int-int-java.lang.String-) | يضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا. |
| [add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)](#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | يضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا. |
| [clear()](#clear--) | يمسح جميع الارتباطات التشعبية. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على عنصر [Hyperlink](../../com.aspose.cells/hyperlink) في الفهرس المحدد. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في مثيل CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | يحدد فهرس عنصر محدد في مثيل CollectionBase. |
| [iterator()](#iterator--) | يرجع كائن تعداد يتنقل عبر مثيل CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | إزالة الارتباط التشعبي في الفهرس المحدد في هذه المجموعة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address) {#add-int-int-int-int-java.lang.String-}
```
public int add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)
```


يضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا.

**Example**

```
         //Instantiating a Workbook object
         Workbook excel = new Workbook();
         Worksheet worksheet = excel.getWorksheets().get(0);
         worksheet.getHyperlinks().add("A4", 1, 1, "http://www.aspose.com");
         worksheet.getHyperlinks().add("A5", 1, 1, "c:\\book1.xls");
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | int | الصف الأول لنطاق الارتباط التشعبي. |
| firstColumn | int | العمود الأول لنطاق الارتباط التشعبي. |
| totalRows | int | عدد الصفوف في نطاق الارتباط التشعبي هذا. |
| totalColumns | int | عدد الأعمدة في نطاق الارتباط التشعبي هذا. |
| العنوان | java.lang.String | عنوان الارتباط التشعبي. |

**Returns:**
int - فهرس كائن [Hyperlink](../../com.aspose.cells/hyperlink).
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
int - فهرس كائن [Hyperlink](../../com.aspose.cells/hyperlink).
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
int - فهرس كائن [Hyperlink](../../com.aspose.cells/hyperlink).
### clear() {#clear--}
```
public void clear()
```


يمسح جميع الارتباطات التشعبية.

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
public Hyperlink get(int index)
```


يحصل على عنصر [Hyperlink](../../com.aspose.cells/hyperlink) في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس الصفري للعنصر. |

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink) - The element at the specified index.
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


إزالة الارتباط التشعبي في الفهرس المحدد في هذه المجموعة.

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

