---
title: "PictureCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على مجموعة من الكائنات."
type: docs
url: /ar/java/com.aspose.cells/picturecollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PictureCollection extends CollectionBase
```

يحتوي على مجموعة من كائنات [Picture](../../com.aspose.cells/picture).

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //get PictureCollection
         PictureCollection pictures = workbook.getWorksheets().get(0).getPictures();
 
         //do your business
 
         //Save the excel file.
         workbook.save("result.xlsx");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)](#add-int-int-int-int-java.io.InputStream-) | يضيف صورة إلى المجموعة. |
| [add(int topRow, int leftColumn, int bottomRow, int rightColumn, String fileName)](#add-int-int-int-int-java.lang.String-) | يضيف صورة إلى المجموعة. |
| [add(int topRow, int leftColumn, InputStream stream)](#add-int-int-java.io.InputStream-) | يضيف صورة إلى المجموعة. |
| [add(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)](#add-int-int-java.io.InputStream-int-int-) | يضيف صورة إلى المجموعة. |
| [add(int topRow, int leftColumn, String fileName)](#add-int-int-java.lang.String-) | يضيف صورة إلى المجموعة. |
| [add(int topRow, int leftColumn, String fileName, int widthScale, int heightScale)](#add-int-int-java.lang.String-int-int-) | يضيف صورة إلى المجموعة. |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [camera(int row, int column, String range)](#camera-int-int-java.lang.String-) | يأخذ صورة للنطاق. |
| [clear()](#clear--) | مسح جميع الصور. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على عنصر [Picture](../../com.aspose.cells/picture) في الفهرس المحدد. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في مثيل CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | يحدد فهرس عنصر محدد في مثيل CollectionBase. |
| [iterator()](#iterator--) | يرجع كائن تعداد يتنقل عبر مثيل CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | إزالة الأشكال في الفهرس المحدد |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream) {#add-int-int-int-int-java.io.InputStream-}
```
public int add(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)
```


يضيف صورة إلى المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| bottomRow | int | فهرس الصف السفلي الأيمن. |
| rightColumn | int | فهرس العمود السفلي الأيمن. |
| stream | java.io.InputStream | كائن الدفق الذي يحتوي على بيانات الصورة. |

**Returns:**
int - فهرس كائن [Picture](../../com.aspose.cells/picture).
### add(int topRow, int leftColumn, int bottomRow, int rightColumn, String fileName) {#add-int-int-int-int-java.lang.String-}
```
public int add(int topRow, int leftColumn, int bottomRow, int rightColumn, String fileName)
```


يضيف صورة إلى المجموعة.

**Example**

```
         //add a picture
         pictures.add(1, 1, 5, 5, "image.jpg");
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| bottomRow | int | فهرس الصف السفلي الأيمن. |
| rightColumn | int | فهرس العمود السفلي الأيمن. |
| fileName | java.lang.String | اسم ملف الصورة. |

**Returns:**
int - فهرس كائن [Picture](../../com.aspose.cells/picture).
### add(int topRow, int leftColumn, InputStream stream) {#add-int-int-java.io.InputStream-}
```
public int add(int topRow, int leftColumn, InputStream stream)
```


يضيف صورة إلى المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| stream | java.io.InputStream | كائن الدفق الذي يحتوي على بيانات الصورة. |

**Returns:**
int - فهرس كائن [Picture](../../com.aspose.cells/picture).
### add(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale) {#add-int-int-java.io.InputStream-int-int-}
```
public int add(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)
```


يضيف صورة إلى المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| stream | java.io.InputStream | كائن الدفق الذي يحتوي على بيانات الصورة. |
| widthScale | int | مقياس عرض الصورة، كنسبة مئوية. |
| heightScale | int | مقياس ارتفاع الصورة، كنسبة مئوية. |

**Returns:**
int - فهرس كائن [Picture](../../com.aspose.cells/picture).
### add(int topRow, int leftColumn, String fileName) {#add-int-int-java.lang.String-}
```
public int add(int topRow, int leftColumn, String fileName)
```


يضيف صورة إلى المجموعة.

**Example**

```
         //add a picture
         pictures.add(1, 1, "image.jpg");
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| fileName | java.lang.String | اسم ملف الصورة. |

**Returns:**
int - فهرس كائن [Picture](../../com.aspose.cells/picture).
### add(int topRow, int leftColumn, String fileName, int widthScale, int heightScale) {#add-int-int-java.lang.String-int-int-}
```
public int add(int topRow, int leftColumn, String fileName, int widthScale, int heightScale)
```


يضيف صورة إلى المجموعة.

**Example**

```
         //add a picture
         pictures.add(1, 1, "image.jpg", 50, 50);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| fileName | java.lang.String | اسم ملف الصورة. |
| widthScale | int | مقياس عرض الصورة، كنسبة مئوية. |
| heightScale | int | مقياس ارتفاع الصورة، كنسبة مئوية. |

**Returns:**
int - فهرس كائن [Picture](../../com.aspose.cells/picture).
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
### camera(int row, int column, String range) {#camera-int-int-java.lang.String-}
```
public int camera(int row, int column, String range)
```


يأخذ صورة للنطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف لهذه الصورة. |
| عمود | int | فهرس العمود لهذه الصورة. |
| نطاق | java.lang.String | المنطقة التي تتطلب التصوير |

**Returns:**
int -
### clear() {#clear--}
```
public void clear()
```


مسح جميع الصور.

**Example**

```
         //clear
         pictures.clear();
```

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
public Picture get(int index)
```


يحصل على عنصر [Picture](../../com.aspose.cells/picture) في الفهرس المحدد.

**Example**

```
         //get picture collection
         //PictureCollection pictures = workbook.Worksheets[0].Pictures;
         //add a picture
         int index = pictures.add(1, 1, "image.png");
         //get the picture
         Picture pic = pictures.get(index);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس الصفري للعنصر. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - The element at the specified index.
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


إزالة الأشكال في الفهرس المحدد

**Example**

```
         //add a picture
         int index2 = pictures.add(1, 1, "image.png");
         //delete
         pictures.removeAt(index2);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int |  |

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

