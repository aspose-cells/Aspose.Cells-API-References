---
title: "TextBoxCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على مجموعة من الكائنات."
type: docs
url: /ar/java/com.aspose.cells/textboxcollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class TextBoxCollection extends CollectionBase
```

يغلف مجموعة من كائنات [TextBox](../../com.aspose.cells/textbox).

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //get collection object
         TextBoxCollection textBoxCollection = workbook.getWorksheets().get(0).getTextBoxes();
         //add a textbox
         textBoxCollection.add(1, 1, 50, 100);
         for(TextBox tbox : (Iterable<TextBox>) textBoxCollection)
         {
             //do what you want
         }
 
         //do your business
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(int topRow, int leftColumn, int height, int width)](#add-int-int-int-int-) | يضيف مربع نص إلى المجموعة. |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [clear()](#clear--) | امسح جميع مربعات النص. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على العنصر [TextBox](../../com.aspose.cells/textbox) عند الفهرس المحدد. |
| [get(String name)](#get-java.lang.String-) | يحصل على عنصر [TextBox](../../com.aspose.cells/textbox) بالاسم. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في مثيل CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | يحدد فهرس عنصر محدد في مثيل CollectionBase. |
| [iterator()](#iterator--) | يرجع كائن تعداد يتنقل عبر مثيل CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | إزالة مربع نص من الملف. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int topRow, int leftColumn, int height, int width) {#add-int-int-int-int-}
```
public int add(int topRow, int leftColumn, int height, int width)
```


يضيف مربع نص إلى المجموعة.

**Example**

```
         //add a TextBox
         int index2 = textBoxCollection.add(1, 1, 50, 100);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | int | فهرس الصف العلوي الأيسر. |
| leftColumn | int | فهرس العمود العلوي الأيسر. |
| الارتفاع | int | ارتفاع الـtextbox، بوحدة البكسل. |
| العرض | int | عرض الـtextbox، بوحدة البكسل. |

**Returns:**
int - فهرس كائن [TextBox](../../com.aspose.cells/textbox).
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


امسح جميع مربعات النص.

**Example**

```
         //clear all textbox
         textBoxCollection.clear();
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
public TextBox get(int index)
```


يحصل على العنصر [TextBox](../../com.aspose.cells/textbox) عند الفهرس المحدد.

**Example**

```
         int index = textBoxCollection.getCount() - 1;
         TextBox txb = textBoxCollection.get(index);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس الصفري للعنصر. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - The element at the specified index.
### get(String name) {#get-java.lang.String-}
```
public TextBox get(String name)
```


يحصل على عنصر [TextBox](../../com.aspose.cells/textbox) بالاسم.

**Example**

```
         String txtboxName = "textbox 1"; 
         TextBox txb2 = textBoxCollection.get(txtboxName);
         if(txb2 != null)
         {
             //do what you want
         }
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم مربع النص. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - 
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


إزالة مربع نص من الملف.

**Example**

```
         int index3 = textBoxCollection.getCount() - 1;
         textBoxCollection.removeAt(index3);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس مربع النص. |

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

