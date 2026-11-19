---
title: "مقسم"
second_title: "Aspose.Cells for Java API Reference"
description: "وصف ملخص لعرض المقسم"
type: docs
url: /ar/java/com.aspose.cells/slicer/
---

**Inheritance:**
java.lang.Object
```
public class Slicer
```

وصف ملخص لعرض المقسم

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
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         pivot.calculateData();
 
         SlicerCollection slicers = sheet.getSlicers();
         int slicerIndex = slicers.add(pivot, "E12", "fruit");
         Slicer slicer = slicers.get(slicerIndex);
         slicer.setStyleType(SlicerStyleType.SLICER_STYLE_LIGHT_2);
 
         slicer.unselectItems(new String[] { "grape" });
         //do your business
         book.save("out.xlsx");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addPivotConnection(PivotTable pivot)](#addPivotConnection-com.aspose.cells.PivotTable-) | يضيف اتصال PivotTable. |
| [clearFilter()](#clearFilter--) | إزالة الفلاتر |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeText()](#getAlternativeText--) | يرجع أو يضبط النص الوصفي (البديل) لكائن Slicer. |
| [getCaption()](#getCaption--) | يرجع أو يضبط تسمية الـ slicer المحدد. |
| [getCaptionVisible()](#getCaptionVisible--) | يرجع أو يضبط ما إذا كان الرأس الذي يعرض Caption الـ slicer مرئيًا. |
| [getClass()](#getClass--) |  |
| [getColumnWidth()](#getColumnWidth--) | يرجع أو يضبط عرض كل عمود في الـ slicer بوحدة النقاط. |
| [getColumnWidthPixel()](#getColumnWidthPixel--) | يحصل على عرض\u807dكل عمود في\u807dالـ slicer، بوحدة\u807dالبكسل.\u807d |
| [getFirstItemIndex()](#getFirstItemIndex--) | يحدد الفهرس الصفري للعنصر الأول في الـ slicer. |
| [getHeight()](#getHeight--) | يرجع أو يضبط ارتفاع الـ slicer المحدد، بوحدة النقاط. |
| [getHeightPixel()](#getHeightPixel--) | إرجاع أو تعيين ارتفاع القاطع المحدد، بوحدة البكسل. |
| [getLeftPixel()](#getLeftPixel--) | إرجاع أو تعيين الإزاحة الأفقية لشكل القاطع من العمود الأيسر، بوحدة البكسل. |
| [getLockedAspectRatio()](#getLockedAspectRatio--) | يشير إلى ما إذا كان يتم قفل نسبة الأبعاد. |
| [getLockedPosition()](#getLockedPosition--) | يشير إلى ما إذا كان يمكن نقل القاطع المحدد أو تغيير حجمه باستخدام واجهة المستخدم. |
| [getName()](#getName--) | إرجاع أو تعيين اسم القاطع المحدد |
| [getNumberOfColumns()](#getNumberOfColumns--) | إرجاع أو تعيين عدد الأعمدة في القاطع. |
| [getParent()](#getParent--) | إرجاع كائن [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) الذي يحتوي على هذا القاطع. |
| [getPlacement()](#getPlacement--) | يمثل الطريقة التي يتم بها إرفاق كائن الرسم بالخلايا تحته. |
| [getRowHeight()](#getRowHeight--) | إرجاع أو تعيين ارتفاع كل صف في القاطع المحدد بوحدة النقاط. |
| [getRowHeightPixel()](#getRowHeightPixel--) | إرجاع أو تعيين ارتفاع كل صف في القاطع المحدد، بوحدة البكسل. |
| [getShape()](#getShape--) | إرجاع كائن Shape المرتبط بالقاطع المحدد. |
| [getShowAllItems()](#getShowAllItems--) | يشير إلى ما إذا كان يجب عرض جميع العناصر حتى في عدم وجود بيانات أو تم حذفها. |
| [getShowCaption()](#getShowCaption--) | يشير إلى ما إذا كان رأس القاطع مرئياً. |
| [getShowMissing()](#getShowMissing--) | يشير إلى ما إذا كان يجب عرض العناصر المحذوفة من مصدر البيانات. |
| [getShowTypeOfItemsWithNoData()](#getShowTypeOfItemsWithNoData--) | يشير إلى ما إذا كان يجب عرض العناصر المحذوفة من مصدر البيانات. |
| [getSlicerCache()](#getSlicerCache--) | إرجاع كائن SlicerCache المرتبط بالقاطع. |
| [getSortOrderType()](#getSortOrderType--) | يشير إلى نوع فرز العناصر. |
| [getStyleType()](#getStyleType--) | حدد نوع نمط القاطع المدمج. |
| [getTitle()](#getTitle--) | يحدد عنوان كائن القاطع الحالي. |
| [getTopPixel()](#getTopPixel--) | إرجاع أو تعيين الإزاحة العمودية لشكل القاطع من الصف العلوي، بوحدة البكسل. |
| [getWidth()](#getWidth--) | إرجاع أو تعيين عرض القاطع المحدد، بوحدة النقاط. |
| [getWidthPixel()](#getWidthPixel--) | إرجاع أو تعيين عرض القاطع المحدد، بوحدة البكسل. |
| [getWorksheet()](#getWorksheet--) | إرجاع كائن [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) الذي يحتوي على هذا القاطع. |
| [hashCode()](#hashCode--) |  |
| [isLocked()](#isLocked--) | يشير إلى ما إذا كان شكل القاطع مقفلاً. |
| [isPrintable()](#isPrintable--) | يشير إلى ما إذا كان كائن القاطع قابلًا للطباعة. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | تحديث عناصر القاطع من جداول Pivot المرتبطة. |
| [removePivotConnection(PivotTable pivot)](#removePivotConnection-com.aspose.cells.PivotTable-) | إزالة اتصال PivotTable. |
| [selectItems(String[] labels, boolean append)](#selectItems-java.lang.String---boolean-) | **ملاحظات** |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | يرجع أو يضبط النص الوصفي (البديل) لكائن Slicer. |
| [setCaption(String value)](#setCaption-java.lang.String-) | يرجع أو يضبط تسمية الـ slicer المحدد. |
| [setCaptionVisible(boolean value)](#setCaptionVisible-boolean-) | يرجع أو يضبط ما إذا كان الرأس الذي يعرض Caption الـ slicer مرئيًا. |
| [setColumnWidth(double value)](#setColumnWidth-double-) | يرجع أو يضبط عرض كل عمود في الـ slicer بوحدة النقاط. |
| [setColumnWidthPixel(int value)](#setColumnWidthPixel-int-) | تعيين عرض\u807dكل عمود في\u807dالقاطع، بوحدة\u807dالبكسل.\u807d |
| [setFirstItemIndex(int value)](#setFirstItemIndex-int-) | يحدد الفهرس الصفري للعنصر الأول في الـ slicer. |
| [setHeight(double value)](#setHeight-double-) | يرجع أو يضبط ارتفاع الـ slicer المحدد، بوحدة النقاط. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | إرجاع أو تعيين ارتفاع القاطع المحدد، بوحدة البكسل. |
| [setLeftPixel(int value)](#setLeftPixel-int-) | إرجاع أو تعيين الإزاحة الأفقية لشكل القاطع من العمود الأيسر، بوحدة البكسل. |
| [setLocked(boolean value)](#setLocked-boolean-) | يشير إلى ما إذا كان شكل القاطع مقفلاً. |
| [setLockedAspectRatio(boolean value)](#setLockedAspectRatio-boolean-) | يشير إلى ما إذا كان يتم قفل نسبة الأبعاد. |
| [setLockedPosition(boolean value)](#setLockedPosition-boolean-) | يشير إلى ما إذا كان يمكن نقل القاطع المحدد أو تغيير حجمه باستخدام واجهة المستخدم. |
| [setName(String value)](#setName-java.lang.String-) | إرجاع أو تعيين اسم القاطع المحدد |
| [setNumberOfColumns(int value)](#setNumberOfColumns-int-) | إرجاع أو تعيين عدد الأعمدة في القاطع. |
| [setPlacement(int value)](#setPlacement-int-) | يمثل الطريقة التي يتم بها إرفاق كائن الرسم بالخلايا تحته. |
| [setPrintable(boolean value)](#setPrintable-boolean-) | يشير إلى ما إذا كان كائن القاطع قابلًا للطباعة. |
| [setRowHeight(double value)](#setRowHeight-double-) | إرجاع أو تعيين ارتفاع كل صف في القاطع المحدد بوحدة النقاط. |
| [setRowHeightPixel(int value)](#setRowHeightPixel-int-) | إرجاع أو تعيين ارتفاع كل صف في القاطع المحدد، بوحدة البكسل. |
| [setShowAllItems(boolean value)](#setShowAllItems-boolean-) | يشير إلى ما إذا كان يجب عرض جميع العناصر حتى في عدم وجود بيانات أو تم حذفها. |
| [setShowCaption(boolean value)](#setShowCaption-boolean-) | يشير إلى ما إذا كان رأس القاطع مرئياً. |
| [setShowMissing(boolean value)](#setShowMissing-boolean-) | يشير إلى ما إذا كان يجب عرض العناصر المحذوفة من مصدر البيانات. |
| [setShowTypeOfItemsWithNoData(int value)](#setShowTypeOfItemsWithNoData-int-) | يشير إلى ما إذا كان يجب عرض العناصر المحذوفة من مصدر البيانات. |
| [setSortOrderType(int value)](#setSortOrderType-int-) | يشير إلى نوع فرز العناصر. |
| [setStyleType(int value)](#setStyleType-int-) | حدد نوع نمط القاطع المدمج. |
| [setTitle(String value)](#setTitle-java.lang.String-) | يحدد عنوان كائن القاطع الحالي. |
| [setTopPixel(int value)](#setTopPixel-int-) | إرجاع أو تعيين الإزاحة العمودية لشكل القاطع من الصف العلوي، بوحدة البكسل. |
| [setWidth(double value)](#setWidth-double-) | إرجاع أو تعيين عرض القاطع المحدد، بوحدة النقاط. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | إرجاع أو تعيين عرض القاطع المحدد، بوحدة البكسل. |
| [toString()](#toString--) |  |
| [unselectItems(String[] labels)](#unselectItems-java.lang.String---) | إزالة تسميات الفلاتر المحددة. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addPivotConnection(PivotTable pivot) {#addPivotConnection-com.aspose.cells.PivotTable-}
```
public void addPivotConnection(PivotTable pivot)
```


يضيف اتصال PivotTable.

**Example**

```
         slicer.addPivotConnection(pivot);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | كائن PivotTable |

### clearFilter() {#clearFilter--}
```
public void clearFilter()
```


إزالة الفلاتر

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
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


يرجع أو يضبط النص الوصفي (البديل) لكائن Slicer.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الخاصية [Shape.getAlternativeText()](../../com.aspose.cells/shape\#getAlternativeText--) . سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
java.lang.String
### getCaption() {#getCaption--}
```
public String getCaption()
```


يرجع أو يضبط تسمية الـ slicer المحدد.

**Example**

```
         slicer.setCaption("slicer caption");
```

**Returns:**
java.lang.String
### getCaptionVisible() {#getCaptionVisible--}
```
public boolean getCaptionVisible()
```


يرجع أو يضبط ما إذا كان رأس العنوان الذي يعرض Caption للـ slicer مرئيًا. القيمة الافتراضية هي true

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الخاصية [getShowCaption()](../../com.aspose.cells/slicer\#getShowCaption--) . سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Example**

```
         slicer.setCaption("slicer caption");
```

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnWidth() {#getColumnWidth--}
```
public double getColumnWidth()
```


يرجع أو يضبط عرض كل عمود في الـ slicer بوحدة النقاط.

**Example**

```
         slicer.setColumnWidth(80);
```

**Returns:**
double
### getColumnWidthPixel() {#getColumnWidthPixel--}
```
public int getColumnWidthPixel()
```


يحصل على عرض\u807dكل عمود في\u807dالـ slicer، بوحدة\u807dالبكسل.\u807d

**Example**

```
         slicer.setColumnWidthPixel(120);
```

**Returns:**
int
### getFirstItemIndex() {#getFirstItemIndex--}
```
public int getFirstItemIndex()
```


يحدد الفهرس الصفري للعنصر الأول في الـ slicer.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


يرجع أو يضبط ارتفاع الـ slicer المحدد، بوحدة النقاط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الخاصية Shape.HeightPt. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
double
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


إرجاع أو تعيين ارتفاع القاطع المحدد، بوحدة البكسل.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية Shape.Height. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getLeftPixel() {#getLeftPixel--}
```
public int getLeftPixel()
```


إرجاع أو تعيين الإزاحة الأفقية لشكل القاطع من العمود الأيسر، بوحدة البكسل.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية Shape.Left. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getLockedAspectRatio() {#getLockedAspectRatio--}
```
public boolean getLockedAspectRatio()
```


يشير إلى ما إذا كان يتم قفل نسبة الأبعاد.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الطريقة [Shape.isAspectRatioLocked()](../../com.aspose.cells/shape\#isAspectRatioLocked--) . سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
boolean
### getLockedPosition() {#getLockedPosition--}
```
public boolean getLockedPosition()
```


يشير إلى ما إذا كان يمكن نقل القاطع المحدد أو تغيير حجمه باستخدام واجهة المستخدم.

**Example**

```
         slicer.setLockedPosition(false);
```

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


إرجاع أو تعيين اسم القاطع المحدد

**Example**

```
         slicer.setName("slicer name");
```

**Returns:**
java.lang.String
### getNumberOfColumns() {#getNumberOfColumns--}
```
public int getNumberOfColumns()
```


يرجع أو يضبط عدد الأعمدة في الـ slicer. القيمة الافتراضية هي 1.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getParent() {#getParent--}
```
public Worksheet getParent()
```


يرجع الكائن [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) الذي يحتوي على هذا الـ slicer. للقراءة فقط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الخاصية [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) . سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Example**

```
         SlicerCache slicerCache = slicer.getSlicerCache();
```

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```


يمثل الطريقة التي يتم بها إرفاق كائن الرسم بالخلايا تحته. تتحكم الخاصية في وضع الكائن على ورقة العمل.

انظر [PlacementType](../../com.aspose.cells/placementtype).

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الخاصية [Shape.getPlacement()](../../com.aspose.cells/shape\#getPlacement--) . سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
int
### getRowHeight() {#getRowHeight--}
```
public double getRowHeight()
```


إرجاع أو تعيين ارتفاع كل صف في القاطع المحدد بوحدة النقاط.

**Example**

```
         slicer.setRowHeight(20);
```

**Returns:**
double
### getRowHeightPixel() {#getRowHeightPixel--}
```
public int getRowHeightPixel()
```


إرجاع أو تعيين ارتفاع كل صف في القاطع المحدد، بوحدة البكسل.

**Example**

```
         slicer.setRowHeightPixel(30);
```

**Returns:**
int
### getShape() {#getShape--}
```
public SlicerShape getShape()
```


يرجع كائن Shape المرتبط بالـ slicer المحدد. للقراءة فقط.

**Returns:**
[SlicerShape](../../com.aspose.cells/slicershape)
### getShowAllItems() {#getShowAllItems--}
```
public boolean getShowAllItems()
```


يشير إلى ما إذا كان يجب عرض جميع العناصر حتى إذا لم تكن هناك بيانات أو تم حذفها. القيمة الافتراضية هي true;

**Returns:**
boolean
### getShowCaption() {#getShowCaption--}
```
public boolean getShowCaption()
```


يشير إلى ما إذا كان رأس الـ slicer مرئيًا. القيمة الافتراضية هي true

**Example**

```
         slicer.setShowCaption(false);
```

**Returns:**
boolean
### getShowMissing() {#getShowMissing--}
```
public boolean getShowMissing()
```


يشير إلى ما إذا كان يجب عرض العناصر المحذوفة من مصدر البيانات.

**Remarks**

يعمل فقط عندما تكون [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) هي true.

**Returns:**
boolean
### getShowTypeOfItemsWithNoData() {#getShowTypeOfItemsWithNoData--}
```
public int getShowTypeOfItemsWithNoData()
```


يشير إلى ما إذا كان يجب عرض العناصر المحذوفة من مصدر البيانات.

انظر [ItemsWithNoDataShowMode](../../com.aspose.cells/itemswithnodatashowmode).

**Remarks**

يعمل فقط عندما تكون [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) هي true.

**Returns:**
int
### getSlicerCache() {#getSlicerCache--}
```
public SlicerCache getSlicerCache()
```


يرجع كائن SlicerCache المرتبط بالـ slicer. للقراءة فقط.

**Example**

```
         SlicerCache slicerCache = slicer.getSlicerCache();
```

**Returns:**
[SlicerCache](../../com.aspose.cells/slicercache)
### getSortOrderType() {#getSortOrderType--}
```
public int getSortOrderType()
```


يشير إلى نوع فرز العناصر.

انظر إلى [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getStyleType() {#getStyleType--}
```
public int getStyleType()
```


حدد نوع نمط الـ slicer المدمج. النوع الافتراضي هو SlicerStyleLight1.

انظر [SlicerStyleType](../../com.aspose.cells/slicerstyletype).

**Example**

```
         slicer.setStyleType(SlicerStyleType.SLICER_STYLE_LIGHT_2);
```

**Returns:**
int
### getTitle() {#getTitle--}
```
public String getTitle()
```


يحدد عنوان كائن القاطع الحالي.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الخاصية [Shape.getTitle()](../../com.aspose.cells/shape\#getTitle--) . سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
java.lang.String
### getTopPixel() {#getTopPixel--}
```
public int getTopPixel()
```


إرجاع أو تعيين الإزاحة العمودية لشكل القاطع من الصف العلوي، بوحدة البكسل.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية Shape.Top. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getWidth() {#getWidth--}
```
public double getWidth()
```


إرجاع أو تعيين عرض القاطع المحدد، بوحدة النقاط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الخاصية Shape.WidthPt. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
double
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


إرجاع أو تعيين عرض القاطع المحدد، بوحدة البكسل.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية Shape.Width. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


يرجع الكائن [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) الذي يحتوي على هذا الـ slicer. للقراءة فقط.

**Example**

```
         Worksheet currSheet = slicer.getParent();
```

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


يشير إلى ما إذا كان شكل القاطع مقفلاً.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الخاصية [Shape.isLocked()](../../com.aspose.cells/shape\#isLocked--) . سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
boolean
### isPrintable() {#isPrintable--}
```
public boolean isPrintable()
```


يشير إلى ما إذا كان كائن القاطع قابلًا للطباعة.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الخاصية [Shape.isPrintable()](../../com.aspose.cells/shape\#isPrintable--) . سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refresh() {#refresh--}
```
public void refresh()
```


تحديث عناصر القاطع من جداول Pivot المرتبطة.

**Example**

```
         slicer.refresh();
```

### removePivotConnection(PivotTable pivot) {#removePivotConnection-com.aspose.cells.PivotTable-}
```
public void removePivotConnection(PivotTable pivot)
```


إزالة اتصال PivotTable.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | كائن PivotTable |

### selectItems(String[] labels, boolean append) {#selectItems-java.lang.String---boolean-}
```
public void selectItems(String[] labels, boolean append)
```


**Remarks**

إذا كنت تريد تحديد جميع العناصر، يرجى استخدام الطريقة [clearFilter()](../../com.aspose.cells/slicer\#clearFilter--) .

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| تسميات | java.lang.String[] | التسميات المحددة. |
| إلحاق | boolean | False يعني اختيار هذه التسميات فقط وإلغاء اختيار الأخرى. True يعني الاحتفاظ بالعناصر المحددة القديمة واختيار هذه التسميات. |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


يرجع أو يضبط النص الوصفي (البديل) لكائن Slicer.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الخاصية [Shape.getAlternativeText()](../../com.aspose.cells/shape\#getAlternativeText--) . سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


يرجع أو يضبط تسمية الـ slicer المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCaptionVisible(boolean value) {#setCaptionVisible-boolean-}
```
public void setCaptionVisible(boolean value)
```


يرجع أو يضبط ما إذا كان رأس العنوان الذي يعرض Caption للـ slicer مرئيًا. القيمة الافتراضية هي true

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الخاصية [getShowCaption()](../../com.aspose.cells/slicer\#getShowCaption--) . سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setColumnWidth(double value) {#setColumnWidth-double-}
```
public void setColumnWidth(double value)
```


يرجع أو يضبط عرض كل عمود في الـ slicer بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setColumnWidthPixel(int value) {#setColumnWidthPixel-int-}
```
public void setColumnWidthPixel(int value)
```


تعيين عرض\u807dكل عمود في\u807dالقاطع، بوحدة\u807dالبكسل.\u807d

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setFirstItemIndex(int value) {#setFirstItemIndex-int-}
```
public void setFirstItemIndex(int value)
```


يحدد الفهرس الصفري للعنصر الأول في الـ slicer.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


يرجع أو يضبط ارتفاع الـ slicer المحدد، بوحدة النقاط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الخاصية Shape.HeightPt. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


إرجاع أو تعيين ارتفاع القاطع المحدد، بوحدة البكسل.

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


إرجاع أو تعيين الإزاحة الأفقية لشكل القاطع من العمود الأيسر، بوحدة البكسل.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية Shape.Left. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


يشير إلى ما إذا كان شكل القاطع مقفلاً.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الخاصية [Shape.isLocked()](../../com.aspose.cells/shape\#isLocked--) . سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setLockedAspectRatio(boolean value) {#setLockedAspectRatio-boolean-}
```
public void setLockedAspectRatio(boolean value)
```


يشير إلى ما إذا كان يتم قفل نسبة الأبعاد.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الطريقة [Shape.isAspectRatioLocked()](../../com.aspose.cells/shape\#isAspectRatioLocked--) . سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setLockedPosition(boolean value) {#setLockedPosition-boolean-}
```
public void setLockedPosition(boolean value)
```


يشير إلى ما إذا كان يمكن نقل القاطع المحدد أو تغيير حجمه باستخدام واجهة المستخدم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


إرجاع أو تعيين اسم القاطع المحدد

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setNumberOfColumns(int value) {#setNumberOfColumns-int-}
```
public void setNumberOfColumns(int value)
```


يرجع أو يضبط عدد الأعمدة في الـ slicer. القيمة الافتراضية هي 1.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


يمثل الطريقة التي يتم بها إرفاق كائن الرسم بالخلايا تحته. تتحكم الخاصية في وضع الكائن على ورقة العمل.

انظر [PlacementType](../../com.aspose.cells/placementtype).

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الخاصية [Shape.getPlacement()](../../com.aspose.cells/shape\#getPlacement--) . سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPrintable(boolean value) {#setPrintable-boolean-}
```
public void setPrintable(boolean value)
```


يشير إلى ما إذا كان كائن القاطع قابلًا للطباعة.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الخاصية [Shape.isPrintable()](../../com.aspose.cells/shape\#isPrintable--) . سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRowHeight(double value) {#setRowHeight-double-}
```
public void setRowHeight(double value)
```


إرجاع أو تعيين ارتفاع كل صف في القاطع المحدد بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setRowHeightPixel(int value) {#setRowHeightPixel-int-}
```
public void setRowHeightPixel(int value)
```


إرجاع أو تعيين ارتفاع كل صف في القاطع المحدد، بوحدة البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setShowAllItems(boolean value) {#setShowAllItems-boolean-}
```
public void setShowAllItems(boolean value)
```


يشير إلى ما إذا كان يجب عرض جميع العناصر حتى إذا لم تكن هناك بيانات أو تم حذفها. القيمة الافتراضية هي true;

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowCaption(boolean value) {#setShowCaption-boolean-}
```
public void setShowCaption(boolean value)
```


يشير إلى ما إذا كان رأس الـ slicer مرئيًا. القيمة الافتراضية هي true

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowMissing(boolean value) {#setShowMissing-boolean-}
```
public void setShowMissing(boolean value)
```


يشير إلى ما إذا كان يجب عرض العناصر المحذوفة من مصدر البيانات.

**Remarks**

يعمل فقط عندما تكون [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowTypeOfItemsWithNoData(int value) {#setShowTypeOfItemsWithNoData-int-}
```
public void setShowTypeOfItemsWithNoData(int value)
```


يشير إلى ما إذا كان يجب عرض العناصر المحذوفة من مصدر البيانات.

انظر [ItemsWithNoDataShowMode](../../com.aspose.cells/itemswithnodatashowmode).

**Remarks**

يعمل فقط عندما تكون [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setSortOrderType(int value) {#setSortOrderType-int-}
```
public void setSortOrderType(int value)
```


يشير إلى نوع فرز العناصر.

انظر إلى [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setStyleType(int value) {#setStyleType-int-}
```
public void setStyleType(int value)
```


حدد نوع نمط الـ slicer المدمج. النوع الافتراضي هو SlicerStyleLight1.

انظر [SlicerStyleType](../../com.aspose.cells/slicerstyletype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


يحدد عنوان كائن القاطع الحالي.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الخاصية [Shape.getTitle()](../../com.aspose.cells/shape\#getTitle--) . سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setTopPixel(int value) {#setTopPixel-int-}
```
public void setTopPixel(int value)
```


إرجاع أو تعيين الإزاحة العمودية لشكل القاطع من الصف العلوي، بوحدة البكسل.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية Shape.Top. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


إرجاع أو تعيين عرض القاطع المحدد، بوحدة النقاط.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الخاصية Shape.WidthPt. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


إرجاع أو تعيين عرض القاطع المحدد، بوحدة البكسل.

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
### unselectItems(String[] labels) {#unselectItems-java.lang.String---}
```
public void unselectItems(String[] labels)
```


إزالة تسميات الفلاتر المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| تسميات | java.lang.String[] | التسميات. |

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

