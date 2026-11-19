---
title: "Timeline"
second_title: "Aspose.Cells for Java API Reference"
description: "وصف ملخص لعرض المخطط الزمني بسبب عدم دعم MS Excel 2003 للمخطط الزمني."
type: docs
url: /ar/java/com.aspose.cells/timeline/
---

**Inheritance:**
java.lang.Object
```
public class Timeline
```

وصف موجز لعرض الخط الزمني بسبب برنامج MS Excel، لا يدعم Excel 2003 الخط الزمني.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
 
         //Create date style
         Style dateStyle = new CellsFactory().createStyle();
         dateStyle.setCustom("m/d/yyyy");
         cells.get(0, 1).setValue("date");
         cells.get(1, 1).setValue(new DateTime(2021, 2, 5));
         cells.get(2, 1).setValue(new DateTime(2022, 3, 8));
         cells.get(3, 1).setValue(new DateTime(2023, 4, 10));
         cells.get(4, 1).setValue(new DateTime(2024, 5, 16));
         //Set date style
         cells.get(1, 1).setStyle(dateStyle);
         cells.get(2, 1).setStyle(dateStyle);
         cells.get(3, 1).setStyle(dateStyle);
         cells.get(4, 1).setStyle(dateStyle);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
 
         PivotTableCollection pivots = sheet.getPivotTables();
         //Add a PivotTable
         PivotTable pivot = pivots.add("=Sheet1!A1:C5", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "date");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         pivot.calculateData();
         //Add time line based on date field.
         int index = sheet.getTimelines().add(pivot, "E1","date");
         Timeline timeline = sheet.getTimelines().get(index);
 
         //do your business
         book.save("out.xlsx");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaption()](#getCaption--) | يحصل على التسمية التوضيحية لهذا المخطط الزمني. |
| [getClass()](#getClass--) |  |
| [getCurrentLevel()](#getCurrentLevel--) | المستوى الزمني الحالي للمخطط الزمني. |
| [getHeightPixel()](#getHeightPixel--) | إرجاع أو تعيين ارتفاع المخطط الزمني المحدد، بوحدات البكسل. |
| [getLeftPixel()](#getLeftPixel--) | إرجاع أو تعيين الإزاحة الأفقية لشكل المخطط الزمني من عموده الأيسر، بوحدات البكسل. |
| [getName()](#getName--) | إرجاع أو تعيين اسم المخطط الزمني المحدد |
| [getSelectedDateTimeRange()](#getSelectedDateTimeRange--) | يحصل على النطاق المحدد للتاريخ والوقت. |
| [getSelectionLevel()](#getSelectionLevel--) | يحصل على المستوى الزمني الذي تم فيه اختيار الحالي للمخطط الزمني. |
| [getShape()](#getShape--) | إرجاع كائن [TimelineShape](../../com.aspose.cells/timelineshape) المرتبط بهذا المخطط الزمني. |
| [getShowHeader()](#getShowHeader--) | يشير إلى ما إذا كان يجب عرض رأس هذا المخطط الزمني. |
| [getShowHorizontalScrollbar()](#getShowHorizontalScrollbar--) | يشير إلى ما إذا كان يجب عرض شريط التمرير الأفقي. |
| [getShowSelectionLabel()](#getShowSelectionLabel--) | يشير إلى ما إذا كان يجب عرض تسمية الاختيار. |
| [getShowTimeLevel()](#getShowTimeLevel--) | يشير إلى ما إذا كان يجب عرض صندوق الاختيار المنسدل للمستوى الزمني. |
| [getStartDate()](#getStartDate--) | يحصل على تاريخ البدء لموضع التمرير للفترة الزمنية لهذا [Timeline](../../com.aspose.cells/timeline). |
| [getTopPixel()](#getTopPixel--) | إرجاع أو تعيين الإزاحة العمودية لشكل المخطط الزمني من صفه العلوي، بوحدات البكسل. |
| [getWidthPixel()](#getWidthPixel--) | إرجاع أو تعيين عرض المخطط الزمني المحدد، بوحدات البكسل. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [select(DateTime start, DateTime end, boolean calculate)](#select-com.aspose.cells.DateTime-com.aspose.cells.DateTime-boolean-) | اختر عنصرًا بين التاريخ والوقت. |
| [setCaption(String value)](#setCaption-java.lang.String-) | يضبط التسمية التوضيحية لهذا المخطط الزمني. |
| [setCurrentLevel(int value)](#setCurrentLevel-int-) | المستوى الزمني الحالي للمخطط الزمني. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | إرجاع أو تعيين ارتفاع المخطط الزمني المحدد، بوحدات البكسل. |
| [setLeftPixel(int value)](#setLeftPixel-int-) | إرجاع أو تعيين الإزاحة الأفقية لشكل المخطط الزمني من عموده الأيسر، بوحدات البكسل. |
| [setName(String value)](#setName-java.lang.String-) | إرجاع أو تعيين اسم المخطط الزمني المحدد |
| [setSelectionLevel(int value)](#setSelectionLevel-int-) | يضبط المستوى الزمني الذي تم فيه اختيار الحالي للمخطط الزمني. |
| [setShowHeader(boolean value)](#setShowHeader-boolean-) | يشير إلى ما إذا كان يجب عرض رأس هذا المخطط الزمني. |
| [setShowHorizontalScrollbar(boolean value)](#setShowHorizontalScrollbar-boolean-) | يشير إلى ما إذا كان يجب عرض شريط التمرير الأفقي. |
| [setShowSelectionLabel(boolean value)](#setShowSelectionLabel-boolean-) | يشير إلى ما إذا كان يجب عرض تسمية الاختيار. |
| [setShowTimeLevel(boolean value)](#setShowTimeLevel-boolean-) | يشير إلى ما إذا كان يجب عرض صندوق الاختيار المنسدل للمستوى الزمني. |
| [setStartDate(DateTime value)](#setStartDate-com.aspose.cells.DateTime-) | يضبط تاريخ البدء لموضع التمرير للفترة الزمنية لهذا [Timeline](../../com.aspose.cells/timeline). |
| [setTopPixel(int value)](#setTopPixel-int-) | إرجاع أو تعيين الإزاحة العمودية لشكل المخطط الزمني من صفه العلوي، بوحدات البكسل. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | إرجاع أو تعيين عرض المخطط الزمني المحدد، بوحدات البكسل. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getCaption() {#getCaption--}
```
public String getCaption()
```


يحصل على التسمية التوضيحية لهذا المخطط الزمني.

**Example**

```
         //Set the caption of this Timeline.
         timeline.setCaption("timeline caption test");
```

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentLevel() {#getCurrentLevel--}
```
public int getCurrentLevel()
```


المستوى الزمني الحالي للمخطط الزمني.

انظر [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Returns:**
int
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


إرجاع أو تعيين ارتفاع المخطط الزمني المحدد، بوحدات البكسل.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية Shape.Height. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getLeftPixel() {#getLeftPixel--}
```
public int getLeftPixel()
```


إرجاع أو تعيين الإزاحة الأفقية لشكل المخطط الزمني من عموده الأيسر، بوحدات البكسل.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية Shape.Left. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


إرجاع أو تعيين اسم المخطط الزمني المحدد

**Example**

```
         //Set the name of the specified Timeline.
         timeline.setName("timeline name test");
```

**Returns:**
java.lang.String
### getSelectedDateTimeRange() {#getSelectedDateTimeRange--}
```
public DateTime[] getSelectedDateTimeRange()
```


يحصل على النطاق المحدد للتاريخ والوقت.

**Returns:**
com.aspose.cells.DateTime[] -
### getSelectionLevel() {#getSelectionLevel--}
```
public int getSelectionLevel()
```


يحصل على المستوى الزمني الذي تم فيه اختيار الحالي للمخطط الزمني.

انظر [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Returns:**
int
### getShape() {#getShape--}
```
public TimelineShape getShape()
```


إرجاع كائن [TimelineShape](../../com.aspose.cells/timelineshape) المرتبط بهذا المخطط الزمني.

**Returns:**
[TimelineShape](../../com.aspose.cells/timelineshape)
### getShowHeader() {#getShowHeader--}
```
public boolean getShowHeader()
```


يشير إلى ما إذا كان يجب عرض رأس هذا المخطط الزمني.

**Returns:**
boolean
### getShowHorizontalScrollbar() {#getShowHorizontalScrollbar--}
```
public boolean getShowHorizontalScrollbar()
```


يشير إلى ما إذا كان يجب عرض شريط التمرير الأفقي.

**Returns:**
boolean
### getShowSelectionLabel() {#getShowSelectionLabel--}
```
public boolean getShowSelectionLabel()
```


يشير إلى ما إذا كان يجب عرض تسمية الاختيار.

**Returns:**
boolean
### getShowTimeLevel() {#getShowTimeLevel--}
```
public boolean getShowTimeLevel()
```


يشير إلى ما إذا كان يجب عرض صندوق الاختيار المنسدل للمستوى الزمني.

**Returns:**
boolean
### getStartDate() {#getStartDate--}
```
public DateTime getStartDate()
```


يحصل على تاريخ البدء لموضع التمرير للفترة الزمنية لهذا [Timeline](../../com.aspose.cells/timeline).

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getTopPixel() {#getTopPixel--}
```
public int getTopPixel()
```


إرجاع أو تعيين الإزاحة العمودية لشكل المخطط الزمني من صفه العلوي، بوحدات البكسل.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية Shape.Top. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


إرجاع أو تعيين عرض المخطط الزمني المحدد، بوحدات البكسل.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية Shape.Width. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

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




### select(DateTime start, DateTime end, boolean calculate) {#select-com.aspose.cells.DateTime-com.aspose.cells.DateTime-boolean-}
```
public void select(DateTime start, DateTime end, boolean calculate)
```


اختر عنصرًا بين التاريخ والوقت.

**Remarks**

[getCurrentLevel()](../../com.aspose.cells/timeline\#getCurrentLevel--) must be set before calling this method. If this method is called, [getSelectionLevel()](../../com.aspose.cells/timeline\#getSelectionLevel--) will be [getCurrentLevel()](../../com.aspose.cells/timeline\#getCurrentLevel--).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| start | [DateTime](../../com.aspose.cells/datetime) | وقت تاريخ البدء |
| end | [DateTime](../../com.aspose.cells/datetime) | وقت تاريخ الانتهاء |
| احسب | boolean | يشير إلى ما إذا كان يجب حساب جداول Pivot النسبية |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


يضبط التسمية التوضيحية لهذا المخطط الزمني.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCurrentLevel(int value) {#setCurrentLevel-int-}
```
public void setCurrentLevel(int value)
```


المستوى الزمني الحالي للمخطط الزمني.

انظر [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


إرجاع أو تعيين ارتفاع المخطط الزمني المحدد، بوحدات البكسل.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية Shape.Height. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setLeftPixel(int value) {#setLeftPixel-int-}
```
public void setLeftPixel(int value)
```


إرجاع أو تعيين الإزاحة الأفقية لشكل المخطط الزمني من عموده الأيسر، بوحدات البكسل.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية Shape.Left. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


إرجاع أو تعيين اسم المخطط الزمني المحدد

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setSelectionLevel(int value) {#setSelectionLevel-int-}
```
public void setSelectionLevel(int value)
```


يضبط المستوى الزمني الذي تم فيه اختيار الحالي للمخطط الزمني.

انظر [TimelineLevelType](../../com.aspose.cells/timelineleveltype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setShowHeader(boolean value) {#setShowHeader-boolean-}
```
public void setShowHeader(boolean value)
```


يشير إلى ما إذا كان يجب عرض رأس هذا المخطط الزمني.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowHorizontalScrollbar(boolean value) {#setShowHorizontalScrollbar-boolean-}
```
public void setShowHorizontalScrollbar(boolean value)
```


يشير إلى ما إذا كان يجب عرض شريط التمرير الأفقي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowSelectionLabel(boolean value) {#setShowSelectionLabel-boolean-}
```
public void setShowSelectionLabel(boolean value)
```


يشير إلى ما إذا كان يجب عرض تسمية الاختيار.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowTimeLevel(boolean value) {#setShowTimeLevel-boolean-}
```
public void setShowTimeLevel(boolean value)
```


يشير إلى ما إذا كان يجب عرض صندوق الاختيار المنسدل للمستوى الزمني.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setStartDate(DateTime value) {#setStartDate-com.aspose.cells.DateTime-}
```
public void setStartDate(DateTime value)
```


يضبط تاريخ البدء لموضع التمرير للفترة الزمنية لهذا [Timeline](../../com.aspose.cells/timeline).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setTopPixel(int value) {#setTopPixel-int-}
```
public void setTopPixel(int value)
```


إرجاع أو تعيين الإزاحة العمودية لشكل المخطط الزمني من صفه العلوي، بوحدات البكسل.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية Shape.Top. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


إرجاع أو تعيين عرض المخطط الزمني المحدد، بوحدات البكسل.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية Shape.Width. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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

