---
title: "TrendlineCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل مجموعة من جميع الكائنات لسلسلة البيانات المحددة."
type: docs
url: /ar/java/com.aspose.cells/trendlinecollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class TrendlineCollection extends CollectionBase
```

يمثل مجموعة من جميع كائنات [Trendline](../../com.aspose.cells/trendline) لسلسلة البيانات المحددة.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Excel object
         int sheetIndex = workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
         worksheet.getCells().get("A1").putValue(50);
         worksheet.getCells().get("A2").putValue(100);
         worksheet.getCells().get("A3").putValue(150);
         worksheet.getCells().get("A4").putValue(200);
         worksheet.getCells().get("B1").putValue(60);
         worksheet.getCells().get("B2").putValue(32);
         worksheet.getCells().get("B3").putValue(50);
         worksheet.getCells().get("B4").putValue(40);
 
         //Adding a chart to the worksheet
         int chartIndex = workbook.getWorksheets().get(0).getCharts().add(ChartType.COLUMN, 3, 3, 15, 10);
         Chart chart = workbook.getWorksheets().get(0).getCharts().get(chartIndex);
         chart.getNSeries().add("A1:a3", true);
         chart.getNSeries().get(0).getTrendLines().add(TrendlineType.LINEAR, "MyTrendLine");
         Trendline line = chart.getNSeries().get(0).getTrendLines().get(0);
         line.setDisplayEquation(true);
         line.setDisplayRSquared(true);
         line.setColor(Color.getRed());
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(int type)](#add-int-) | يضيف كائن [Trendline](../../com.aspose.cells/trendline) إلى هذه المجموعة مع النوع المحدد. |
| [add(int type, String name)](#add-int-java.lang.String-) | يضيف كائن [Trendline](../../com.aspose.cells/trendline) إلى هذه المجموعة مع النوع والاسم المحددين. |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [clear()](#clear--) | يزيل جميع الكائنات من مثيل CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على كائن [Trendline](../../com.aspose.cells/trendline) بواسطة فهرسه. |
| [getClass()](#getClass--) |  |
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
### add(int type) {#add-int-}
```
public int add(int type)
```


يضيف كائن [Trendline](../../com.aspose.cells/trendline) إلى هذه المجموعة مع النوع المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [TrendlineType](../../com.aspose.cells/trendlinetype). نوع خط الاتجاه. |

**Returns:**
int - فهرس كائن [Trendline](../../com.aspose.cells/trendline).
### add(int type, String name) {#add-int-java.lang.String-}
```
public int add(int type, String name)
```


يضيف كائن [Trendline](../../com.aspose.cells/trendline) إلى هذه المجموعة مع النوع والاسم المحددين.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [TrendlineType](../../com.aspose.cells/trendlinetype). نوع خط الاتجاه. |
| name | java.lang.String | اسم خط الاتجاه. |

**Returns:**
int - فهرس كائن [Trendline](../../com.aspose.cells/trendline).
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
### get(int index) {#get-int-}
```
public Trendline get(int index)
```


يحصل على كائن [Trendline](../../com.aspose.cells/trendline) بواسطة فهرسه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int |  |

**Returns:**
[Trendline](../../com.aspose.cells/trendline)
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

