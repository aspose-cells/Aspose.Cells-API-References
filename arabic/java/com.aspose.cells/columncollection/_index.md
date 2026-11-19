---
title: "ColumnCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "مجموعة الكائنات التي تمثل إعدادات الأعمدة الفردية في ورقة العمل."
type: docs
url: /ar/java/com.aspose.cells/columncollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ColumnCollection extends CollectionBase
```

مجموعة من كائنات [Column](../../com.aspose.cells/column) التي تمثل الأعمدة (الإعدادات) الفردية في ورقة عمل. كائن Column يمثل فقط الإعدادات مثل عرض العمود، الأنماط، إلخ للعمود بأكمله، ولا علاقة له بوجود خلايا غير فارغة (بيانات) أو عدمها في العمود المقابل. و"Count" لهذه المجموعة يمثل فقط عدد كائنات Column التي تم إنشاءها في هذه المجموعة، ولا علاقة له بوجود خلايا غير فارغة (بيانات) أو عدمها في ورقة العمل.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Add new Style to Workbook
         Style style = workbook.createStyle();
 
         //Setting the background color to Blue
         style.setForegroundColor(Color.getBlue());
 
         //setting Background Pattern
         style.setPattern(BackgroundType.SOLID);
 
         //New Style Flag
         StyleFlag styleFlag = new StyleFlag();
 
         //Set All Styles
         styleFlag.setAll(true);
 
         //Change the default width of first ten columns
         for (int i = 0; i ? i++)
         {
             worksheet.getCells().getColumns().get(i).setWidth(20);
         }
 
         //Get the Column with non default formatting
         ColumnCollection columns = worksheet.getCells().getColumns();
 
         for (Column column : (Iterable<Column>) columns)
         {
             //Apply Style to first ten Columns
             column.applyStyle(style, styleFlag);
         }
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [clear()](#clear--) | يزيل جميع الكائنات من مثيل CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int columnIndex)](#get-int-) | يحصل على كائن [Column](../../com.aspose.cells/column) حسب فهرس العمود. |
| [getByIndex(int index)](#getByIndex-int-) | يحصل على كائن العمود حسب الفهرس. |
| [getClass()](#getClass--) |  |
| [getColumnByIndex(int index)](#getColumnByIndex-int-) | يحصل على كائن [Column](../../com.aspose.cells/column) حسب الموضع في القائمة. |
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
### get(int columnIndex) {#get-int-}
```
public Column get(int columnIndex)
```


يحصل على كائن [Column](../../com.aspose.cells/column) حسب فهرس العمود. سيتم إنشاء كائن Column للفهرس المحدد إذا لم يكن موجودًا مسبقًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int |  |

**Returns:**
[Column](../../com.aspose.cells/column)
### getByIndex(int index) {#getByIndex-int-}
```
public Column getByIndex(int index)
```


يحصل على كائن العمود حسب الفهرس.

**Remarks**

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام طريقة Columns.GetColumnByIndex(). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2010. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int |  |

**Returns:**
[Column](../../com.aspose.cells/column) - Returns the column object.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnByIndex(int index) {#getColumnByIndex-int-}
```
public Column getColumnByIndex(int index)
```


يحصل على كائن [Column](../../com.aspose.cells/column) حسب الموضع في القائمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الموضع في القائمة. |

**Returns:**
[Column](../../com.aspose.cells/column) - Returns the column object.
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

