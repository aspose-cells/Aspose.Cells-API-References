---
title: "RowCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يجمع الكائنات التي تمثل الصفوف الفردية في ورقة العمل."
type: docs
url: /ar/java/com.aspose.cells/rowcollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class RowCollection implements Iterable
```

يجمع كائنات [Row](../../com.aspose.cells/row) التي تمثل الصفوف الفردية في ورقة العمل.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
          //Get first row
         Row row = worksheet.getCells().getRows().get(0);
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [clear()](#clear--) | امسح جميع الصفوف والخلايا. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int rowIndex)](#get-int-) | يحصل على كائن [Row](../../com.aspose.cells/row) وفقًا لمؤشر الصف المعطى. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد الصفوف في هذه المجموعة. |
| [getRowByIndex(int index)](#getRowByIndex-int-) | يحصل على كائن الصف حسب الموقع في القائمة. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | يحصل على مُعدد يمر عبر الصفوف في هذه المجموعة |
| [iterator(boolean reversed, boolean sync)](#iterator-boolean-boolean-) | يحصل على مُعدد يمر عبر الصفوف في هذه المجموعة |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | إزالة عنصر الصف عند الفهرس (الموقع) المحدد في هذه المجموعة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### clear() {#clear--}
```
public void clear()
```


امسح جميع الصفوف والخلايا.

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
### get(int rowIndex) {#get-int-}
```
public Row get(int rowIndex)
```


يحصل على كائن [Row](../../com.aspose.cells/row) وفقًا لمؤشر الصف المعطى. سيتم إنشاء كائن Row لمؤشر الصف المعطى إذا لم يكن موجودًا مسبقًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int |  |

**Returns:**
[Row](../../com.aspose.cells/row)
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


يحصل على عدد الصفوف في هذه المجموعة.

**Returns:**
int
### getRowByIndex(int index) {#getRowByIndex-int-}
```
public Row getRowByIndex(int index)
```


يحصل على كائن الصف حسب الموقع في القائمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الموضع. |

**Returns:**
[Row](../../com.aspose.cells/row) - The Row object at given position.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### iterator() {#iterator--}
```
public Iterator iterator()
```


يحصل على مُعدد يمر عبر الصفوف في هذه المجموعة

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.getRows().iterator();
         	while (en.hasNext())
         	{
         	    Row row = (Row)en.next();
         	    System.out.println(row.getIndex() + ": " + row.getHeight());
         	}
```

**Returns:**
java.util.Iterator - عداد الصفوف الذي سيستعرض جميع الصفوف الموجودة في هذه المجموعة.
### iterator(boolean reversed, boolean sync) {#iterator-boolean-boolean-}
```
public Iterator iterator(boolean reversed, boolean sync)
```


يحصل على مُعدد يمر عبر الصفوف في هذه المجموعة

**Remarks**

إذا تم تعديل مجموعة الصفوف (بعمليات قد تؤدي إلى إنشاء صف جديد أو إزالة صف موجود) أثناء الاستعراض باستخدام العداد، يجب استخدام العداد المتزامن بدلاً من العداد العادي حتى يتمكن الاستعراض من المتابعة من الموضع الذي يلي الأخير الذي تم استعراضه بواسطة آخر MoveNext(). ومع ذلك، إلى جانب الميزة التي لا يتم فيها تخطي أي عنصر أو استعراضه مرارًا، فإن العيب في العداد المتزامن هو أن الأداء سيتدهور قليلاً مقارنةً بالعداد العادي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| معكوس | boolean | ما إذا كان سيتم تعداد الصفوف بترتيب معكوس |
| مزامنة | boolean | ما إذا كان العداد المرتجع يجب أن يتحقق من تعديل مجموعة الصفوف ويحافظ على التزامن معها. |

**Returns:**
java.util.Iterator - عداد الصفوف الذي سيستعرض جميع الصفوف الموجودة في هذه المجموعة.
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


إزالة عنصر الصف عند الفهرس (الموقع) المحدد في هذه المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| index | int | فهرس يبدأ من الصفر (الموضع، ليس [Row.getIndex()](../../com.aspose.cells/row\#getIndex--)) لعنصر الصف الموجود في هذه المجموعة. |

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

