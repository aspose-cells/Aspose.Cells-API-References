---
title: "DataSorter"
second_title: "Aspose.Cells for Java API Reference"
description: "وصف موجز لـ DataSorter."
type: docs
url: /ar/java/com.aspose.cells/datasorter/
---

**Inheritance:**
java.lang.Object
```
public class DataSorter
```

وصف موجز لـ DataSorter.

**Example**

```
         //Instantiate a new Workbook object.
         Workbook workbook = new Workbook("Book1.xls");
         //Get the workbook datasorter object.
         DataSorter sorter = workbook.getDataSorter();
         //Set the first order for datasorter object.
         sorter.setOrder1(com.aspose.cells.SortOrder.DESCENDING);
         //Define the first key.
         sorter.setKey1(0);
         //Set the second order for datasorter object.
         sorter.setOrder2(com.aspose.cells.SortOrder.ASCENDING);
         //Define the second key.
         sorter.setKey2(1);
         //Create a cells area (range).
         CellArea ca = new CellArea();
         //Specify the start row index.
         ca.StartRow = 0;
         //Specify the start column index.
         ca.StartColumn = 0;
         //Specify the last row index.
         ca.EndRow = 13;
         //Specify the last column index.
         ca.EndColumn = 1;
         //Sort data in the specified data range (A1:B14)
         sorter.sort(workbook.getWorksheets().get(0).getCells(), ca);
         //Save the excel file.
         workbook.save("outBook.xls");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addColorKey(int key, int type, int order, Color color)](#addColorKey-int-int-int-com.aspose.cells.Color-) | يضيف مفتاح فرز اللون. |
| [addKey(int key, int order)](#addKey-int-int-) | يضيف فهرس العمود المرتب وترتيب الفرز. |
| [addKey(int key, int type, int order, Object customList)](#addKey-int-int-int-java.lang.Object-) | يضيف فهرس العمود المرتب وترتيب الفرز مع قائمة فرز مخصصة. |
| [addKey(int key, int order, String customList)](#addKey-int-int-java.lang.String-) | يضيف فهرس العمود المرتب وترتيب الفرز مع قائمة فرز مخصصة. |
| [addKey(int key, int order, String[] customList)](#addKey-int-int-java.lang.String---) | يضيف فهرس العمود المرتب وترتيب الفرز مع قائمة فرز مخصصة. |
| [clear()](#clear--) | امسح جميع الإعدادات. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaseSensitive()](#getCaseSensitive--) | يحصل على ما إذا كان حساسًا لحالة الأحرف عند مقارنة السلسلة. |
| [getClass()](#getClass--) |  |
| [getKey1()](#getKey1--) | يمثل فهرس العمود المرتب الأول (الموضع المطلق، العمود A هو 0، B هو 1، ...). |
| [getKey2()](#getKey2--) | يمثل فهرس العمود المرتب الثاني (الموضع المطلق، العمود A هو 0، B هو 1، ...). |
| [getKey3()](#getKey3--) | يمثل فهرس العمود المرتب الثالث (الموضع المطلق، العمود A هو 0، B هو 1، ...). |
| [getKeys()](#getKeys--) | يحصل على قائمة المفاتيح لــ DataSorter. |
| [getOrder1()](#getOrder1--) | يمثل ترتيب الفرز للمفتاح الأول. |
| [getOrder2()](#getOrder2--) | يمثل ترتيب الفرز للمفتاح الثاني. |
| [getOrder3()](#getOrder3--) | يمثل ترتيب الفرز للمفتاح الثالث. |
| [getSortAsNumber()](#getSortAsNumber--) | يشير إلى ما إذا كان يتم فرز أي شيء يبدو كرقم. |
| [getSortLeftToRight()](#getSortLeftToRight--) | صحيح يعني أن اتجاه الفرز من اليسار إلى اليمين. |
| [hasHeaders()](#hasHeaders--) | يمثل ما إذا كان النطاق يحتوي على رؤوس. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCaseSensitive(boolean value)](#setCaseSensitive-boolean-) | يضبط ما إذا كان حساسًا لحالة الأحرف عند مقارنة السلسلة. |
| [setHasHeaders(boolean value)](#setHasHeaders-boolean-) | يمثل ما إذا كان النطاق يحتوي على رؤوس. |
| [setKey1(int value)](#setKey1-int-) | يمثل فهرس العمود المرتب الأول (الموضع المطلق، العمود A هو 0، B هو 1، ...). |
| [setKey2(int value)](#setKey2-int-) | يمثل فهرس العمود المرتب الثاني (الموضع المطلق، العمود A هو 0، B هو 1، ...). |
| [setKey3(int value)](#setKey3-int-) | يمثل فهرس العمود المرتب الثالث (الموضع المطلق، العمود A هو 0، B هو 1، ...). |
| [setOrder1(int value)](#setOrder1-int-) | يمثل ترتيب الفرز للمفتاح الأول. |
| [setOrder2(int value)](#setOrder2-int-) | يمثل ترتيب الفرز للمفتاح الثاني. |
| [setOrder3(int value)](#setOrder3-int-) | يمثل ترتيب الفرز للمفتاح الثالث. |
| [setSortAsNumber(boolean value)](#setSortAsNumber-boolean-) | يشير إلى ما إذا كان يتم فرز أي شيء يبدو كرقم. |
| [setSortLeftToRight(boolean value)](#setSortLeftToRight-boolean-) | صحيح يعني أن اتجاه الفرز من اليسار إلى اليمين. |
| [sort()](#sort--) | فرز البيانات في النطاق. |
| [sort(Cells cells, CellArea area)](#sort-com.aspose.cells.Cells-com.aspose.cells.CellArea-) | رتب بيانات المنطقة. |
| [sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)](#sort-com.aspose.cells.Cells-int-int-int-int-) | يرتب بيانات المنطقة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addColorKey(int key, int type, int order, Color color) {#addColorKey-int-int-int-com.aspose.cells.Color-}
```
public void addColorKey(int key, int type, int order, Color color)
```


يضيف مفتاح فرز اللون.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| المفتاح | int | فهرس العمود المرتب (الموقع المطلق، العمود A هو 0، B هو 1، ...) |
| type | int | [SortOnType](../../com.aspose.cells/sortontype). نوع قيمة اللون المرتبة. |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). ترتيب الفرز. |
| color | [Color](../../com.aspose.cells/color) | لون الفرز المخصص. |

### addKey(int key, int order) {#addKey-int-int-}
```
public void addKey(int key, int order)
```


يضيف فهرس العمود المرتب وترتيب الفرز.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| المفتاح | int | فهرس العمود المرتب (الموقع المطلق، العمود A هو 0، B هو 1، ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). ترتيب الفرز |

### addKey(int key, int type, int order, Object customList) {#addKey-int-int-int-java.lang.Object-}
```
public void addKey(int key, int type, int order, Object customList)
```


يضيف فهرس العمود المرتب وترتيب الفرز مع قائمة فرز مخصصة.

**Remarks**

إذا كان النوع SortOnType.CellColor أو SortOnType.FontColor، فإن customList هو Color.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| المفتاح | int | فهرس العمود المرتب (الموقع المطلق، العمود A هو 0، B هو 1، ...) |
| type | int | [SortOnType](../../com.aspose.cells/sortontype). نوع القيمة المرتبة. |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). ترتيب الفرز. |
| customList | java.lang.Object | قائمة الفرز المخصصة. |

### addKey(int key, int order, String customList) {#addKey-int-int-java.lang.String-}
```
public void addKey(int key, int order, String customList)
```


يضيف فهرس العمود المرتب وترتيب الفرز مع قائمة فرز مخصصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| المفتاح | int | فهرس العمود المرتب (الموقع المطلق، العمود A هو 0، B هو 1، ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). ترتيب الفرز. |
| customList | java.lang.String | قائمة الفرز المخصصة. |

### addKey(int key, int order, String[] customList) {#addKey-int-int-java.lang.String---}
```
public void addKey(int key, int order, String[] customList)
```


يضيف فهرس العمود المرتب وترتيب الفرز مع قائمة فرز مخصصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| المفتاح | int | فهرس العمود المرتب (الموقع المطلق، العمود A هو 0، B هو 1، ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). ترتيب الفرز. |
| customList | java.lang.String[] | قائمة الفرز المخصصة. |

### clear() {#clear--}
```
public void clear()
```


امسح جميع الإعدادات.

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
### getCaseSensitive() {#getCaseSensitive--}
```
public boolean getCaseSensitive()
```


يحصل على ما إذا كان حساسًا لحالة الأحرف عند مقارنة السلسلة.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getKey1() {#getKey1--}
```
public int getKey1()
```


يمثل فهرس العمود المرتب الأول (الموضع المطلق، العمود A هو 0، B هو 1، ...).

**Returns:**
int
### getKey2() {#getKey2--}
```
public int getKey2()
```


يمثل فهرس العمود المرتب الثاني (الموضع المطلق، العمود A هو 0، B هو 1، ...).

**Returns:**
int
### getKey3() {#getKey3--}
```
public int getKey3()
```


يمثل فهرس العمود المرتب الثالث (الموضع المطلق، العمود A هو 0، B هو 1، ...).

**Returns:**
int
### getKeys() {#getKeys--}
```
public DataSorterKeyCollection getKeys()
```


يحصل على قائمة المفاتيح لــ DataSorter.

**Returns:**
[DataSorterKeyCollection](../../com.aspose.cells/datasorterkeycollection)
### getOrder1() {#getOrder1--}
```
public int getOrder1()
```


يمثل ترتيب الفرز للمفتاح الأول.

انظر إلى [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getOrder2() {#getOrder2--}
```
public int getOrder2()
```


يمثل ترتيب الفرز للمفتاح الثاني.

انظر إلى [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getOrder3() {#getOrder3--}
```
public int getOrder3()
```


يمثل ترتيب الفرز للمفتاح الثالث.

انظر إلى [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getSortAsNumber() {#getSortAsNumber--}
```
public boolean getSortAsNumber()
```


يشير إلى ما إذا كان يتم فرز أي شيء يبدو كرقم.

**Returns:**
boolean
### getSortLeftToRight() {#getSortLeftToRight--}
```
public boolean getSortLeftToRight()
```


True يعني أن اتجاه الفرز من اليسار إلى اليمين. False يعني أن اتجاه الفرز من الأعلى إلى الأسفل. القيمة الافتراضية هي false.

**Returns:**
boolean
### hasHeaders() {#hasHeaders--}
```
public boolean hasHeaders()
```


يمثل ما إذا كان النطاق يحتوي على رؤوس.

**Returns:**
boolean
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




### setCaseSensitive(boolean value) {#setCaseSensitive-boolean-}
```
public void setCaseSensitive(boolean value)
```


يضبط ما إذا كان حساسًا لحالة الأحرف عند مقارنة السلسلة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHasHeaders(boolean value) {#setHasHeaders-boolean-}
```
public void setHasHeaders(boolean value)
```


يمثل ما إذا كان النطاق يحتوي على رؤوس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setKey1(int value) {#setKey1-int-}
```
public void setKey1(int value)
```


يمثل فهرس العمود المرتب الأول (الموضع المطلق، العمود A هو 0، B هو 1، ...).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setKey2(int value) {#setKey2-int-}
```
public void setKey2(int value)
```


يمثل فهرس العمود المرتب الثاني (الموضع المطلق، العمود A هو 0، B هو 1، ...).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setKey3(int value) {#setKey3-int-}
```
public void setKey3(int value)
```


يمثل فهرس العمود المرتب الثالث (الموضع المطلق، العمود A هو 0، B هو 1، ...).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setOrder1(int value) {#setOrder1-int-}
```
public void setOrder1(int value)
```


يمثل ترتيب الفرز للمفتاح الأول.

انظر إلى [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setOrder2(int value) {#setOrder2-int-}
```
public void setOrder2(int value)
```


يمثل ترتيب الفرز للمفتاح الثاني.

انظر إلى [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setOrder3(int value) {#setOrder3-int-}
```
public void setOrder3(int value)
```


يمثل ترتيب الفرز للمفتاح الثالث.

انظر إلى [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setSortAsNumber(boolean value) {#setSortAsNumber-boolean-}
```
public void setSortAsNumber(boolean value)
```


يشير إلى ما إذا كان يتم فرز أي شيء يبدو كرقم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSortLeftToRight(boolean value) {#setSortLeftToRight-boolean-}
```
public void setSortLeftToRight(boolean value)
```


True يعني أن اتجاه الفرز من اليسار إلى اليمين. False يعني أن اتجاه الفرز من الأعلى إلى الأسفل. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### sort() {#sort--}
```
public int[] sort()
```


فرز البيانات في النطاق.

**Returns:**
int[] - الفهارس الأصلية (الموقع المطلق، على سبيل المثال، العمود A هو 0، B هو 1، ...) للصفوف/الأعمدة المرتبة. إذا لم تحتاج أي صفوف/أعمدة إلى النقل بواسطة عملية الفرز هذه، سيتم إرجاع null.
### sort(Cells cells, CellArea area) {#sort-com.aspose.cells.Cells-com.aspose.cells.CellArea-}
```
public int[] sort(Cells cells, CellArea area)
```


رتب بيانات المنطقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cells | [Cells](../../com.aspose.cells/cells) | الخلايا التي تحتوي على منطقة البيانات. |
| area | [CellArea](../../com.aspose.cells/cellarea) | المنطقة المطلوبة للفرز |

**Returns:**
int[] - الفهارس الأصلية (الموقع المطلق، على سبيل المثال، العمود A هو 0، B هو 1، ...) للصفوف/الأعمدة المرتبة. إذا لم تحتاج أي صفوف/أعمدة إلى النقل بواسطة عملية الفرز هذه، سيتم إرجاع null.
### sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn) {#sort-com.aspose.cells.Cells-int-int-int-int-}
```
public int[] sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)
```


يرتب بيانات المنطقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cells | [Cells](../../com.aspose.cells/cells) | الخلايا التي تحتوي على منطقة البيانات. |
| startRow | int | صف البداية للمنطقة. |
| startColumn | int | عمود البداية للمنطقة. |
| endRow | int | صف النهاية للمنطقة. |
| endColumn | int | عمود النهاية للمنطقة. |

**Returns:**
int[] - الفهارس الأصلية (الموقع المطلق، على سبيل المثال، العمود A هو 0، B هو 1، ...) للصفوف/الأعمدة المرتبة. إذا لم تحتاج أي صفوف/أعمدة إلى النقل بواسطة عملية الفرز هذه، سيتم إرجاع null.
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

