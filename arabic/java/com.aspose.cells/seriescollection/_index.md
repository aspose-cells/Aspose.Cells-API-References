---
title: "SeriesCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على مجموعة من الكائنات."
type: docs
url: /ar/java/com.aspose.cells/seriescollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SeriesCollection extends CollectionBase
```

يحتوي على مجموعة من كائنات [Series](../../com.aspose.cells/series).

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Excel object
         int sheetIndex = workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(100);
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
         //Adding a sample value to "A4" cell
         worksheet.getCells().get("A4").putValue(200);
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(60);
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(32);
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
         //Adding a sample value to "B4" cell
         worksheet.getCells().get("B4").putValue(40);
         //Adding a sample value to "C1" cell as category data
         worksheet.getCells().get("C1").putValue("Q1");
         //Adding a sample value to "C2" cell as category data
         worksheet.getCells().get("C2").putValue("Q2");
         //Adding a sample value to "C3" cell as category data
         worksheet.getCells().get("C3").putValue("Y1");
         //Adding a sample value to "C4" cell as category data
         worksheet.getCells().get("C4").putValue("Y2");
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
         chart.getNSeries().add("A1:B4", true);
         //Setting the data source for the category data of NSeries
         chart.getNSeries().setCategoryData("C1:C4");
         //Saving the Excel file
         workbook.save("book1.xls");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [add(String dataArea, boolean isVertical)](#add-java.lang.String-boolean-) | يضيف مجموعة [Series](../../com.aspose.cells/series) إلى مخطط. |
| [add(String area, boolean isVertical, boolean checkLabels)](#add-java.lang.String-boolean-boolean-) | يضيف مجموعة [Series](../../com.aspose.cells/series) إلى مخطط. |
| [addR1C1(String area, boolean isVertical)](#addR1C1-java.lang.String-boolean-) | يضيف مجموعة [Series](../../com.aspose.cells/series) إلى مخطط. |
| [changeColors(int type)](#changeColors-int-) | تعيين لوحة ألوان أحادية اللون لسلسلة المخطط. |
| [changeSeriesOrder(int sourceIndex, int destIndex)](#changeSeriesOrder-int-int-) | يغيّر مباشرةً ترتيب السلسلتين. |
| [clear()](#clear--) | يمسح المجموعة. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على عنصر [Series](../../com.aspose.cells/series) في الفهرس المحدد. |
| [getCategoryData()](#getCategoryData--) | يحصل على نطاق قيم محور الفئة. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في مثيل CollectionBase. |
| [getSecondCategoryData()](#getSecondCategoryData--) | يحصل على نطاق قيم محور الفئة الثاني. |
| [getSeriesByOrder(int order)](#getSeriesByOrder-int-) | يحصل على عنصر [Series](../../com.aspose.cells/series) حسب الترتيب. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | يحدد فهرس عنصر محدد في مثيل CollectionBase. |
| [isColorVaried()](#isColorVaried--) | يمثل ما إذا كان لون النقاط متنوعًا. |
| [iterator()](#iterator--) | يرجع كائن تعداد يتنقل عبر مثيل CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | إزالة سلسلة في الفهرس المحدد. |
| [setCategoryData(String value)](#setCategoryData-java.lang.String-) | يضبط نطاق قيم محور الفئة. |
| [setColorVaried(boolean value)](#setColorVaried-boolean-) | يمثل ما إذا كان لون النقاط متنوعًا. |
| [setSecondCategoryData(String value)](#setSecondCategoryData-java.lang.String-) | يضبط نطاق قيم محور الفئة الثاني. |
| [setSeriesNames(int startIndex, String area, boolean isVertical)](#setSeriesNames-int-java.lang.String-boolean-) | يضبط أسماء جميع السلاسل في المخطط. |
| [swapSeries(int sourceIndex, int destIndex)](#swapSeries-int-int-) | يغيّر مباشرةً ترتيب السلسلتين. |
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
### add(String dataArea, boolean isVertical) {#add-java.lang.String-boolean-}
```
public int add(String dataArea, boolean isVertical)
```


يضيف مجموعة [Series](../../com.aspose.cells/series) إلى مخطط.

**Remarks**


إذا تم تعيين البيانات على خلايا متجاورة، استخدم النقطتين للفصل بينها.على سبيل المثال، $C$2:$C$5.

إذا تم تعيين البيانات على خلايا غير متجاورة، استخدم الفاصلة للفصل بينها.على سبيل المثال: ($C$2,$D$5).

هذه الطريقة تعالج ببساطة النطاق كبيانات فقط. إذا كنت ترغب في التحقق بذكاء من طريقة ChartCollection.Add().


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| dataArea | java.lang.String | يحدد القيم التي تُرسم منها سلسلة البيانات |
| isVertical | boolean | يحدد ما إذا كان سيتم رسم السلسلة من نطاق قيم الخلايا حسب الصف أو حسب العمود. إذا كان صحيحًا، سيتم إضافة [Series](../../com.aspose.cells/series) عمودًا بعمود. |

**Returns:**
int - إرجاع الفهرس الأول للسلسلة المضافة ASeries في NSeries.
### add(String area, boolean isVertical, boolean checkLabels) {#add-java.lang.String-boolean-boolean-}
```
public int add(String area, boolean isVertical, boolean checkLabels)
```


يضيف مجموعة [Series](../../com.aspose.cells/series) إلى مخطط.

**Remarks**


إذا تم تعيين البيانات على خلايا متجاورة، استخدم النقطتين للفصل بينها. على سبيل المثال، $C$2:$C$5.

إذا تم تعيين البيانات على خلايا غير متجاورة، استخدم الفاصلة للفصل بينها. على سبيل المثال، ($C$2,$D$5).


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| area | java.lang.String | يحدد القيم التي تُرسم منها سلسلة البيانات |
| isVertical | boolean | يحدد ما إذا كان سيتم رسم السلسلة من نطاق قيم الخلايا حسب الصف أو حسب العمود. |
| checkLabels | boolean | يشير إلى ما إذا كان النطاق يحتوي على اسم السلسلة |

**Returns:**
int - إرجاع الفهرس الأول للسلسلة المضافة ASeries في NSeries.
### addR1C1(String area, boolean isVertical) {#addR1C1-java.lang.String-boolean-}
```
public int addR1C1(String area, boolean isVertical)
```


يضيف مجموعة [Series](../../com.aspose.cells/series) إلى مخطط.

**Remarks**


إذا تم تعيين البيانات على خلايا متجاورة، استخدم النقطتين للفصل بينها. على سبيل المثال، R[1]C[1]:R[3]C[2].

إذا تم تعيين البيانات على خلايا متجاورة، استخدم الفاصلة للفصل بينها. على سبيل المثال،(R[1]C[1],R[3]C[2]).


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| area | java.lang.String | يحدد القيم التي تُرسم منها سلسلة البيانات |
| isVertical | boolean | يحدد ما إذا كان سيتم رسم السلسلة من نطاق قيم الخلايا حسب الصف أو حسب العمود. |

**Returns:**
int - إرجاع الفهرس الأول للسلسلة المضافة ASeries في NSeries.
### changeColors(int type) {#changeColors-int-}
```
public void changeColors(int type)
```


تعيين لوحة ألوان أحادية اللون لسلسلة المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [ChartColorPaletteType](../../com.aspose.cells/chartcolorpalettetype). النوع الأحادي اللون. |

### changeSeriesOrder(int sourceIndex, int destIndex) {#changeSeriesOrder-int-int-}
```
public void changeSeriesOrder(int sourceIndex, int destIndex)
```


يغيّر مباشرةً ترتيب السلسلتين.

**Remarks**

ملاحظة: هذه الطريقة أصبحت قديمة الآن. بدلاً من ذلك، يرجى استخدام طريقة SeriesCollection.SwapSeries. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ يونيو 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceIndex | int | الفهرس الحالي |
| destIndex | int | فهرس الوجهة |

### clear() {#clear--}
```
public void clear()
```


يمسح المجموعة.

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
public Series get(int index)
```


يحصل على عنصر [Series](../../com.aspose.cells/series) في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس الصفري للعنصر. |

**Returns:**
[Series](../../com.aspose.cells/series) - The element at the specified index.
### getCategoryData() {#getCategoryData--}
```
public String getCategoryData()
```


يحصل على نطاق قيم محور الفئة. يمكن أن يكون نطاق خلايا (مثل "d1:e10") أو تسلسل قيم (مثل "\{2,6,8,10\}").

**Returns:**
java.lang.String
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
### getSecondCategoryData() {#getSecondCategoryData--}
```
public String getSecondCategoryData()
```


يحصل على نطاق قيم محور الفئة الثاني. يمكن أن يكون نطاق خلايا (مثل "d1:e10"), أو تسلسل قيم (مثل "\{2,6,8,10\}"). يؤثر فقط عندما يتم رسم بعض السلاسل على المحور الثاني.

**Returns:**
java.lang.String
### getSeriesByOrder(int order) {#getSeriesByOrder-int-}
```
public Series getSeriesByOrder(int order)
```


يحصل على عنصر [Series](../../com.aspose.cells/series) حسب الترتيب.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| order | int | ترتيب السلاسل |

**Returns:**
[Series](../../com.aspose.cells/series) - The element series
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
### isColorVaried() {#isColorVaried--}
```
public boolean isColorVaried()
```


يمثل ما إذا كان لون النقاط متنوعًا.

**Remarks**

يعمل فقط مع مخطط دائري أو عندما تكون هناك سلسلة واحدة فقط.

**Returns:**
boolean
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


إزالة سلسلة في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس. |

### setCategoryData(String value) {#setCategoryData-java.lang.String-}
```
public void setCategoryData(String value)
```


يضبط نطاق قيم محور الفئة. يمكن أن يكون نطاق خلايا (مثل "d1:e10") أو تسلسل قيم (مثل "\{2,6,8,10\}").

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setColorVaried(boolean value) {#setColorVaried-boolean-}
```
public void setColorVaried(boolean value)
```


يمثل ما إذا كان لون النقاط متنوعًا.

**Remarks**

يعمل فقط مع مخطط دائري أو عندما تكون هناك سلسلة واحدة فقط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSecondCategoryData(String value) {#setSecondCategoryData-java.lang.String-}
```
public void setSecondCategoryData(String value)
```


يضبط نطاق قيم محور الفئة الثاني. يمكن أن يكون نطاق خلايا (مثل "d1:e10"), أو تسلسل قيم (مثل "\{2,6,8,10\}"). يؤثر فقط عندما يتم رسم بعض السلاسل على المحور الثاني.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setSeriesNames(int startIndex, String area, boolean isVertical) {#setSeriesNames-int-java.lang.String-boolean-}
```
public void setSeriesNames(int startIndex, String area, boolean isVertical)
```


يضبط أسماء جميع السلاسل في المخطط.

**Remarks**


إذا كان فهرس البداية أكبر من عدد السلاسل، فسيعود دون فعل شيء.

إذا تم تعيين البيانات على خلايا متجاورة، استخدم النقطتين للفصل بينها. على سبيل المثال، $C$2:$C$5.

إذا تم تعيين البيانات على خلايا متجاورة، استخدم الفاصلة لفصلها. على سبيل المثال، ($C$2,$D$5).


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startIndex | int | فهرس السلسلة الأولى التي تريد تعيين الاسم لها. |
| area | java.lang.String | يحدد المنطقة لاسم السلسلة. |
| isVertical | boolean | >يحدد ما إذا كان سيتم رسم السلسلة من نطاق قيم الخلايا حسب الصف أو حسب العمود. |

### swapSeries(int sourceIndex, int destIndex) {#swapSeries-int-int-}
```
public void swapSeries(int sourceIndex, int destIndex)
```


يغيّر مباشرةً ترتيب السلسلتين.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceIndex | int | الفهرس الحالي |
| destIndex | int | فهرس الوجهة |

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

