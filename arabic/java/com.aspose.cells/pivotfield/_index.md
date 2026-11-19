---
title: "PivotField"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل حقلًا في تقرير جدول المحور."
type: docs
url: /ar/java/com.aspose.cells/pivotfield/
---

**Inheritance:**
java.lang.Object
```
public class PivotField
```

يمثل حقلًا في تقرير جدول المحور.

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
 
          //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
          pivot.calculateData(new PivotTableCalculateOption());
 
         //do your business
 
         book.save("out.xlsx");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addCalculatedItem(String name, String formula)](#addCalculatedItem-java.lang.String-java.lang.String-) | إضافة عنصر صيغة محسوبة إلى حقل PivotField. |
| [clearFilter()](#clearFilter--) | مسح إعدادات الفلتر على هذا الحقل PivotField. |
| [dispose()](#dispose--) | ينفذ مهام محددة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة ضبط الموارد غير المُدارة. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filterByDate(int type, DateTime dateTime1, DateTime dateTime2)](#filterByDate-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-) | تصفية حسب قيم التاريخ لحقل PivotField الصف أو العمود. |
| [filterByLabel(int type, String label1, String label2)](#filterByLabel-int-java.lang.String-java.lang.String-) | يفلتر حسب عناوين حقل محور الصف أو العمود. |
| [filterByValue(int valueFieldIndex, int type, double value1, double value2)](#filterByValue-int-int-double-double-) | يفلتر حسب قيم حقل محور البيانات. |
| [filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount)](#filterTop10-int-int-boolean-int-) | يفلتر حسب قيم حقل محور البيانات. |
| [getAllowDraggingToColumn()](#getAllowDraggingToColumn--) | يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة العمود. |
| [getAllowDraggingToData()](#getAllowDraggingToData--) | يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة القيم. |
| [getAllowDraggingToPage()](#getAllowDraggingToPage--) | يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الصفحة. |
| [getAllowDraggingToRow()](#getAllowDraggingToRow--) | يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الصف. |
| [getAllowRemovingFromView()](#getAllowRemovingFromView--) | يشير إلى ما إذا كان يمكن إزالة هذا الحقل PivotField من عرض PivotTable. |
| [getAutoShowCount()](#getAutoShowCount--) | يمثل عدد العناصر العليا أو السفلى التي تُظهر تلقائيًا في حقل PivotTable المحدد. |
| [getAutoShowField()](#getAutoShowField--) | يمثل فهرس الحقل العرض التلقائي. -1 يعني PivotField نفسه. |
| [getAutoSortField()](#getAutoSortField--) | يمثل فهرس الحقل الذي يتم فرزه تلقائيًا. |
| [getBaseIndex()](#getBaseIndex--) | يمثل الفهرس في حقول PivotField المصدر. |
| [getCalculatedFieldFormula()](#getCalculatedFieldFormula--) | احصل على سلسلة الصيغة للحقل المحسوب المحدد. |
| [getClass()](#getClass--) |  |
| [getCurrentPageItem()](#getCurrentPageItem--) | يحصل على عنصر الصفحة المعروض حاليًا لهذا الحقل PivotField (حقل الصفحة فقط). |
| [getCurrentPageItemText()](#getCurrentPageItemText--) | يحصل على نص العرض للعنصر الحالي للصفحة لهذا الحقل المحوري (حقل الصفحة فقط). |
| [getDisplayName()](#getDisplayName--) | يمثل اسم العرض لحقل المحور في عرض جدول المحور. |
| [getDragToColumn()](#getDragToColumn--) | يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة العمود. |
| [getDragToData()](#getDragToData--) | يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة القيم. |
| [getDragToHide()](#getDragToHide--) | يشير إلى ما إذا كان يمكن إزالة هذا الحقل PivotField من عرض PivotTable. |
| [getDragToPage()](#getDragToPage--) | يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الصفحة. |
| [getDragToRow()](#getDragToRow--) | يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الصف. |
| [getFilters()](#getFilters--) | يحصل على جميع عوامل تصفية المحور المطبقة لهذا الحقل المحوري. |
| [getFormula()](#getFormula--) | يحصل على صيغة الحقل المحسوب. |
| [getFunction()](#getFunction--) | يمثل الدالة المستخدمة لتلخيص حقل بيانات جدول المحور هذا. |
| [getGroupSettings()](#getGroupSettings--) | يحصل على إعدادات التجميع للحقل المحوري. |
| [getInsertBlankRow()](#getInsertBlankRow--) | يشير إلى ما إذا كان يجب إدراج سطر فارغ بعد كل عنصر. |
| [getItemCount()](#getItemCount--) | يحصل على عدد العناصر الأساسية في هذا الحقل المحوري. |
| [getItems()](#getItems--) | احصل على جميع تسميات عناصر المحور في هذا الحقل. |
| [getMaxValue()](#getMaxValue--) | يحصل على القيمة القصوى لهذا الحقل. |
| [getMinValue()](#getMinValue--) | يحصل على القيمة القصوى لهذا الحقل. |
| [getName()](#getName--) | يمثل اسم حقل المحور. |
| [getNonAutoSortDefault()](#getNonAutoSortDefault--) | يشير إلى ما إذا كانت عملية الفرز التي ستُطبق على هذا الحقل المحوري هي عملية فرز تلقائي أم فرز بيانات بسيط. |
| [getNumber()](#getNumber--) | يمثل تنسيق العرض المدمج للأرقام والتواريخ. |
| [getNumberFormat()](#getNumberFormat--) | يمثل تنسيق العرض المخصص للأرقام والتواريخ. |
| [getOriginalItems()](#getOriginalItems--) | احصل على العناصر الأساسية الأصلية؛ |
| [getPivotFilterByType(int type)](#getPivotFilterByType-int-) | يحصل على مرشح المحور للحقل المحوري حسب النوع |
| [getPivotFilters()](#getPivotFilters--) | يحصل على عوامل تصفية المحور للحقل المحوري |
| [getPivotItems()](#getPivotItems--) | يحصل على عناصر المحور للحقل المحوري |
| [getPosition()](#getPosition--) | يمثل الفهرس لـ [PivotField](../../com.aspose.cells/pivotfield) في المنطقة. |
| [getRegionType()](#getRegionType--) | يحدد منطقة جدول المحور التي يُعرض فيها هذا الحقل. |
| [getShowAllItems()](#getShowAllItems--) | يشير إلى ما إذا كان يجب عرض جميع العناصر في عرض جدول المحور، حتى إذا لم تحتوي على بيانات ملخص. |
| [getShowCompact()](#getShowCompact--) | يشير إلى ما إذا كان يجب عرض تسميات الحقل التالي في نفس العمود في عرض جدول المحور. |
| [getShowInCompactForm()](#getShowInCompactForm--) | يحصل على قيمة تشير إلى ما إذا كان حقل الصف هذا يستخدم تخطيط الشكل المدمج. |
| [getShowInOutlineForm()](#getShowInOutlineForm--) | يحصل على قيمة تشير إلى ما إذا كان حقل الصف هذا يستخدم تخطيط المخطط. |
| [getShowSubtotalAtTop()](#getShowSubtotalAtTop--) | يشير إلى ما إذا كان يجب عرض المجاميع الفرعية في أعلى أو أسفل العناصر. |
| [getShowValuesSetting()](#getShowValuesSetting--) | يحصل على إعدادات عرض القيم كما عندما يكون حساب ShowDataAs قيد الاستخدام. |
| [getSortSetting()](#getSortSetting--) | يحصل على جميع إعدادات الفرز التلقائي |
| [getSubtotals()](#getSubtotals--) | يحصل على المجاميع الفرعية للحقل. |
| [getSubtotals(int subtotalType)](#getSubtotals-int-) | يحدد ما إذا كان سيتم عرض المجمل الفرعي المحدد لهذا الحقل المحوري. |
| [getTop10AutoShowSettings()](#getTop10AutoShowSettings--) | يحصل على إعدادات AutoShow لأفضل 10 لحقل محوري. |
| [group()](#group--) | يقوم بتجميع الحقل تلقائيًا. |
| [group(PivotFieldGroupOptions options)](#group-com.aspose.cells.PivotFieldGroupOptions-) | يقوم بتجميع الحقل المحوري مع الخيارات. |
| [groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField)](#groupBy-boolean-com.aspose.cells.DateTime-boolean-com.aspose.cells.DateTime-int---double-boolean-) | قم بتجميع الملف حسب أنواع تجميع التاريخ. |
| [groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField)](#groupBy-boolean-double-boolean-double-double-boolean-) | قم بتجميع الملف حسب الرقم. |
| [groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField)](#groupBy-com.aspose.cells.CustomPiovtFieldGroupItem---boolean-) | قم بتجميع الحقل مخصصًا. |
| [groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField)](#groupBy-com.aspose.cells.DateTime-com.aspose.cells.DateTime-int---double-boolean-) | قم بتجميع الملف حسب أنواع تجميع التاريخ. |
| [groupBy(DiscreteGroupItem[] customGroupItems, boolean newField)](#groupBy-com.aspose.cells.DiscreteGroupItem---boolean-) | قم بتجميع الحقل مخصصًا. |
| [groupBy(double interval, boolean newField)](#groupBy-double-boolean-) | قم بتجميع الحقل تلقائيًا باستخدام الفاصل الزمني |
| [groupBy(double start, double end, double interval, boolean newField)](#groupBy-double-double-double-boolean-) | قم بتجميع الملف حسب الرقم. |
| [groupBy(int[] groups, double interval, boolean newField)](#groupBy-int---double-boolean-) | قم بتجميع الحقل تلقائيًا باستخدام internal |
| [hashCode()](#hashCode--) |  |
| [hideAllDetails()](#hideAllDetails--) | يخفي جميع تفاصيل كل عنصر محوري. |
| [hideDetail(boolean isHiddenDetail)](#hideDetail-boolean-) | يحدد ما إذا كانت تفاصيل جميع PivotItems في حقل محوري مخفية. |
| [hideItem(int index, boolean isHidden)](#hideItem-int-boolean-) | يحدد ما إذا كان PivotItem المحدد في حقل البيانات مخفيًا. |
| [hideItem(String itemValue, boolean isHidden)](#hideItem-java.lang.String-boolean-) | يحدد ما إذا كان PivotItem المحدد في حقل البيانات مخفيًا. |
| [hideItemDetail(int index, boolean isHiddenDetail)](#hideItemDetail-int-boolean-) | يحدد ما إذا كانت تفاصيل PivotItem المحدد في حقل محوري مخفية. |
| [initPivotItems()](#initPivotItems--) | تهيئة عناصر pivot للحقل المحوري |
| [isAscendShow()](#isAscendShow--) | يشير إلى ما إذا كان حقل PivotTable المحدد يُعرض تلقائيًا تصاعديًا. |
| [isAscendSort()](#isAscendSort--) | يحدد ما إذا كانت عناصر هذا الحقل المحوري مرتبة تلقائيًا تصاعديًا. |
| [isAutoShow()](#isAutoShow--) | يحدد ما إذا كان حقل PivotTable المحدد يُظهر تلقائيًا. |
| [isAutoSort()](#isAutoSort--) | يحدد ما إذا كانت عناصر حقل PivotTable هذا مرتبة تلقائيًا. |
| [isAutoSubtotals()](#isAutoSubtotals--) | يحدد ما إذا كان الحقل المحدد يعرض المجاميع الفرعية التلقائية. |
| [isCalculatedField()](#isCalculatedField--) | يحدد ما إذا كان هذا الحقل المحوري حقلًا محسوبًا. |
| [isHiddenItem(int index)](#isHiddenItem-int-) | يحدد ما إذا كان PivotItem المحدد مخفيًا. |
| [isHiddenItemDetail(int index)](#isHiddenItemDetail-int-) | يحدد ما إذا كان يجب إخفاء تفاصيل PivotItem المحدد.. |
| [isIncludeNewItemsInFilter()](#isIncludeNewItemsInFilter--) | يحدد ما إذا كان يجب تضمين عناصر جديدة إلى الحقل في الفلتر اليدوي. |
| [isInsertPageBreaksBetweenItems()](#isInsertPageBreaksBetweenItems--) | يشير إلى ما إذا كان يجب إدراج فواصل صفحات بعد كل عنصر. |
| [isMultipleItemSelectionAllowed()](#isMultipleItemSelectionAllowed--) | يشير إلى ما إذا كان يمكن اختيار عناصر متعددة في حقل الصفحة. |
| [isRepeatItemLabels()](#isRepeatItemLabels--) | يشير إلى ما إذا كان يجب تكرار تسميات الحقل في منطقة الصف أو العمود. |
| [isValueFields()](#isValueFields--) | يشير إلى ما إذا كان هذا الحقل يمثل حقول القيم. |
| [isValuesField()](#isValuesField--) | يشير إلى ما إذا كان هذا الحقل يمثل حقل القيم. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowDraggingToColumn(boolean value)](#setAllowDraggingToColumn-boolean-) | يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة العمود. |
| [setAllowDraggingToData(boolean value)](#setAllowDraggingToData-boolean-) | يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة القيم. |
| [setAllowDraggingToPage(boolean value)](#setAllowDraggingToPage-boolean-) | يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الصفحة. |
| [setAllowDraggingToRow(boolean value)](#setAllowDraggingToRow-boolean-) | يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الصف. |
| [setAllowRemovingFromView(boolean value)](#setAllowRemovingFromView-boolean-) | يشير إلى ما إذا كان يمكن إزالة هذا الحقل PivotField من عرض PivotTable. |
| [setAscendShow(boolean value)](#setAscendShow-boolean-) | يشير إلى ما إذا كان حقل PivotTable المحدد يُعرض تلقائيًا تصاعديًا. |
| [setAscendSort(boolean value)](#setAscendSort-boolean-) | يحدد ما إذا كانت عناصر هذا الحقل المحوري مرتبة تلقائيًا تصاعديًا. |
| [setAutoShow(boolean value)](#setAutoShow-boolean-) | يحدد ما إذا كان حقل PivotTable المحدد يُظهر تلقائيًا. |
| [setAutoShowCount(int value)](#setAutoShowCount-int-) | يمثل عدد العناصر العليا أو السفلى التي تُظهر تلقائيًا في حقل PivotTable المحدد. |
| [setAutoShowField(int value)](#setAutoShowField-int-) | يمثل فهرس الحقل العرض التلقائي. -1 يعني PivotField نفسه. |
| [setAutoSort(boolean value)](#setAutoSort-boolean-) | يحدد ما إذا كانت عناصر حقل PivotTable هذا مرتبة تلقائيًا. |
| [setAutoSortField(int value)](#setAutoSortField-int-) | يمثل فهرس الحقل الذي يتم فرزه تلقائيًا. |
| [setAutoSubtotals(boolean value)](#setAutoSubtotals-boolean-) | يحدد ما إذا كان الحقل المحدد يعرض المجاميع الفرعية التلقائية. |
| [setBaseIndex(int value)](#setBaseIndex-int-) | يمثل الفهرس في حقول PivotField المصدر. |
| [setCurrentPageItem(short value)](#setCurrentPageItem-short-) | يضبط العنصر الصفحي المعروض حاليًا لهذا الحقل المحوري (حقل الصفحة فقط). |
| [setCurrentPageItemText(String value)](#setCurrentPageItemText-java.lang.String-) | يحصل على نص العرض للعنصر الحالي للصفحة لهذا الحقل المحوري (حقل الصفحة فقط). |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | يمثل اسم العرض لحقل المحور في عرض جدول المحور. |
| [setDragToColumn(boolean value)](#setDragToColumn-boolean-) | يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة العمود. |
| [setDragToData(boolean value)](#setDragToData-boolean-) | يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة القيم. |
| [setDragToHide(boolean value)](#setDragToHide-boolean-) | يشير إلى ما إذا كان يمكن إزالة هذا الحقل PivotField من عرض PivotTable. |
| [setDragToPage(boolean value)](#setDragToPage-boolean-) | يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الصفحة. |
| [setDragToRow(boolean value)](#setDragToRow-boolean-) | يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الصف. |
| [setFunction(int value)](#setFunction-int-) | يمثل الدالة المستخدمة لتلخيص حقل بيانات جدول المحور هذا. |
| [setIncludeNewItemsInFilter(boolean value)](#setIncludeNewItemsInFilter-boolean-) | يحدد ما إذا كان يجب تضمين عناصر جديدة إلى الحقل في الفلتر اليدوي. |
| [setInsertBlankRow(boolean value)](#setInsertBlankRow-boolean-) | يشير إلى ما إذا كان يجب إدراج سطر فارغ بعد كل عنصر. |
| [setInsertPageBreaksBetweenItems(boolean value)](#setInsertPageBreaksBetweenItems-boolean-) | يشير إلى ما إذا كان يجب إدراج فواصل صفحات بعد كل عنصر. |
| [setMultipleItemSelectionAllowed(boolean value)](#setMultipleItemSelectionAllowed-boolean-) | يشير إلى ما إذا كان يمكن اختيار عناصر متعددة في حقل الصفحة. |
| [setName(String value)](#setName-java.lang.String-) | يمثل اسم حقل المحور. |
| [setNonAutoSortDefault(boolean value)](#setNonAutoSortDefault-boolean-) | يشير إلى ما إذا كانت عملية الفرز التي ستُطبق على هذا الحقل المحوري هي عملية فرز تلقائي أم فرز بيانات بسيط. |
| [setNumber(int value)](#setNumber-int-) | يمثل تنسيق العرض المدمج للأرقام والتواريخ. |
| [setNumberFormat(String value)](#setNumberFormat-java.lang.String-) | يمثل تنسيق العرض المخصص للأرقام والتواريخ. |
| [setRepeatItemLabels(boolean value)](#setRepeatItemLabels-boolean-) | يشير إلى ما إذا كان يجب تكرار تسميات الحقل في منطقة الصف أو العمود. |
| [setShowAllItems(boolean value)](#setShowAllItems-boolean-) | يشير إلى ما إذا كان يجب عرض جميع العناصر في عرض جدول المحور، حتى إذا لم تحتوي على بيانات ملخص. |
| [setShowCompact(boolean value)](#setShowCompact-boolean-) | يشير إلى ما إذا كان يجب عرض تسميات الحقل التالي في نفس العمود في عرض جدول المحور. |
| [setShowInCompactForm(boolean value)](#setShowInCompactForm-boolean-) | يضبط قيمة تشير إلى ما إذا كان حقل الصف هذا يستخدم تخطيط الشكل المدمج. |
| [setShowInOutlineForm(boolean value)](#setShowInOutlineForm-boolean-) | يضبط قيمة تشير إلى ما إذا كان حقل الصف هذا يستخدم تخطيط المخطط. |
| [setShowSubtotalAtTop(boolean value)](#setShowSubtotalAtTop-boolean-) | يشير إلى ما إذا كان يجب عرض المجاميع الفرعية في أعلى أو أسفل العناصر. |
| [setSubtotals(int value)](#setSubtotals-int-) | يضبط المجاميع الفرعية للحقل. |
| [setSubtotals(int subtotalType, boolean shown)](#setSubtotals-int-boolean-) | يضبط طريقة تجميع الحقل المحدد. |
| [showAllDetails()](#showAllDetails--) | اعرض جميع تفاصيل كل عنصر محوري. |
| [showValuesAs(int showValuesAsType, int baseField, int baseItem)](#showValuesAs-int-int-int-) | يضبط حساب "عرض القيم كـ" لهذا الحقل المحوري. |
| [showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem)](#showValuesAs-int-int-int-int-) | يعرض قيم حقل البيانات بتنسيق عرض مختلف عندما يكون حساب ShowDataAs قيد الاستخدام. |
| [showValuesAs(int showValuesAsType, String baseField, String baseItem)](#showValuesAs-int-java.lang.String-java.lang.String-) | يضبط تكوين حساب "عرض القيم كـ" لهذا حقل البيانات. |
| [sortBy(int sortType)](#sortBy-int-) | يرتب هذا الحقل المحوري. |
| [sortBy(int sortType, int fieldSortedBy)](#sortBy-int-int-) | يرتب هذا الحقل المحوري. |
| [sortBy(int sortType, int fieldSortedBy, int dataType, String cellName)](#sortBy-int-int-int-java.lang.String-) | يرتب هذا الحقل المحوري. |
| [sortBy(int sortType, int fieldSortedBy, String cellName)](#sortBy-int-int-java.lang.String-) | يرتب هذا الحقل المحوري. |
| [toString()](#toString--) |  |
| [top10AutoShow(boolean isAutoShow, boolean isTop, int count, int rankBy)](#top10AutoShow-boolean-boolean-int-int-) | يضبط إعدادات العرض التلقائي Top10 لهذا الحقل المحوري. |
| [ungroup()](#ungroup--) | إلغاء تجميع الحقل المحوري. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCalculatedItem(String name, String formula) {#addCalculatedItem-java.lang.String-java.lang.String-}
```
public void addCalculatedItem(String name, String formula)
```


إضافة عنصر صيغة محسوبة إلى حقل PivotField.

**Remarks**

يدعم فقط إضافة عنصر محسوب إلى حقل الصف/العمود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم العنصر. |
| formula | java.lang.String | صيغة العنصر المحوري. |

### clearFilter() {#clearFilter--}
```
public void clearFilter()
```


مسح إعدادات الفلتر على هذا الحقل PivotField.

### dispose() {#dispose--}
```
public void dispose()
```


ينفذ مهام محددة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة ضبط الموارد غير المُدارة.

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
### filterByDate(int type, DateTime dateTime1, DateTime dateTime2) {#filterByDate-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-}
```
public PivotFilter filterByDate(int type, DateTime dateTime1, DateTime dateTime2)
```


تصفية حسب قيم التاريخ لحقل PivotField الصف أو العمود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). نوع تصفية البيانات. |
| dateTime1 | [DateTime](../../com.aspose.cells/datetime) | تسمية التاريخ لشرط الفلترة |
| dateTime2 | [DateTime](../../com.aspose.cells/datetime) | تسمية التاريخ الحد الأعلى لشرط الفلترة بين |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterByLabel(int type, String label1, String label2) {#filterByLabel-int-java.lang.String-java.lang.String-}
```
public PivotFilter filterByLabel(int type, String label1, String label2)
```


يفلتر حسب عناوين حقل محور الصف أو العمود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). نوع تصفية البيانات. |
| label1 | java.lang.String | تسمية شرط الفلترة |
| label2 | java.lang.String | العلامة العليا لشرط الفلتر بين |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterByValue(int valueFieldIndex, int type, double value1, double value2) {#filterByValue-int-int-double-double-}
```
public PivotFilter filterByValue(int valueFieldIndex, int type, double value1, double value2)
```


يفلتر حسب قيم حقل محور البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| valueFieldIndex | int | فهرس حقل القيمة في منطقة القيمة. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). نوع تصفية البيانات. |
| value1 | double | قيمة شرط الفلتر |
| value2 | double | القيمة العليا لشرط الفلتر بين |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount) {#filterTop10-int-int-boolean-int-}
```
public PivotFilter filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount)
```


يفلتر حسب قيم حقل محور البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| valueFieldIndex | int | فهرس حقل البيانات في منطقة البيانات. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). نوع تصفية البيانات. يمكن أن يكون فقط Count,Sum و Percent. |
| isTop | boolean | يشير إلى ما إذا كان الفلتر من الأعلى أو الأسفل |
| itemCount | int | عدد العناصر |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### getAllowDraggingToColumn() {#getAllowDraggingToColumn--}
```
public boolean getAllowDraggingToColumn()
```


يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة العمود. القيمة الافتراضية هي true.

**Returns:**
boolean
### getAllowDraggingToData() {#getAllowDraggingToData--}
```
public boolean getAllowDraggingToData()
```


يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة القيم. القيمة الافتراضية هي true.

**Returns:**
boolean
### getAllowDraggingToPage() {#getAllowDraggingToPage--}
```
public boolean getAllowDraggingToPage()
```


يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الصفحة. القيمة الافتراضية هي true.

**Returns:**
boolean
### getAllowDraggingToRow() {#getAllowDraggingToRow--}
```
public boolean getAllowDraggingToRow()
```


يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الصف. القيمة الافتراضية هي true.

**Returns:**
boolean
### getAllowRemovingFromView() {#getAllowRemovingFromView--}
```
public boolean getAllowRemovingFromView()
```


يشير إلى ما إذا كان يمكن إزالة هذا الحقل المحوري من عرض PivotTable. القيمة الافتراضية هي true.

**Returns:**
boolean
### getAutoShowCount() {#getAutoShowCount--}
```
public int getAutoShowCount()
```


يمثل عدد العناصر العليا أو السفلى التي تُظهر تلقائيًا في حقل PivotTable المحدد.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.Top10AutoShowSettings.AutoShowCount أو طريقة PivotField.Top10AutoShow() بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getAutoShowField() {#getAutoShowField--}
```
public int getAutoShowField()
```


يمثل فهرس الحقل المعروض تلقائيًا. -1 يعني PivotField نفسه. يجب أن يكون فهرس حقول البيانات.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.Top10AutoShowSettings.RankBy أو طريقة PivotField.Top10AutoShow() بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getAutoSortField() {#getAutoSortField--}
```
public int getAutoSortField()
```


يمثل فهرس الحقل الذي يتم فرزه تلقائيًا. -1 يعني PivotField نفسه، والقيم الأخرى تعني موقع حقول البيانات.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.SortSetting.SortBy أو طريقة PivotField.SortBy() بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getBaseIndex() {#getBaseIndex--}
```
public int getBaseIndex()
```


يمثل الفهرس في حقول PivotField المصدر.

**Remarks**

ملاحظة: هذه الدالة الضابطة لهذه الخاصية أصبحت الآن غير صالحة. سيتم إزالة هذه الدالة الضابطة بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getCalculatedFieldFormula() {#getCalculatedFieldFormula--}
```
public String getCalculatedFieldFormula()
```


احصل على سلسلة الصيغة للحقل المحسوب المحدد.

**Remarks**

ملاحظة: هذه الطريقة أصبحت الآن غير صالحة. بدلاً من ذلك، يرجى استخدام طريقة PivotField.GetFormula(). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أغسطس 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentPageItem() {#getCurrentPageItem--}
```
public short getCurrentPageItem()
```


يحصل على عنصر الصفحة المعروض حاليًا لهذا الحقل PivotField (حقل الصفحة فقط).

**Remarks**

استخدم [PivotItem.ALL\_PAGE\_ITEMS\_INDEX](../../com.aspose.cells/pivotitem\#ALL-PAGE-ITEMS-INDEX) (0x7FFD) كقيمة إشارة لتحديد "Select All". هذه علامة معرفة مسبقًا وليست فهرس عنصر صالح.

**Returns:**
short
### getCurrentPageItemText() {#getCurrentPageItemText--}
```
public String getCurrentPageItemText()
```


يحصل على نص العرض للعنصر الحالي للصفحة لهذا الحقل المحوري (حقل الصفحة فقط).

**Remarks**

يرجع "(All)" عندما تكون [getCurrentPageItem()](../../com.aspose.cells/pivotfield\#getCurrentPageItem--) مساوية لـ [PivotItem.ALL\_PAGE\_ITEMS\_INDEX](../../com.aspose.cells/pivotitem\#ALL-PAGE-ITEMS-INDEX). للقيم الأخرى، يرجع تمثيل السلسلة لفهرس العنصر.

**Returns:**
java.lang.String
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


يمثل اسم العرض لحقل المحور في عرض جدول المحور.

**Returns:**
java.lang.String
### getDragToColumn() {#getDragToColumn--}
```
public boolean getDragToColumn()
```


يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة العمود. القيمة الافتراضية هي true.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.AllowDraggingToColumn بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### getDragToData() {#getDragToData--}
```
public boolean getDragToData()
```


يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة القيم. القيمة الافتراضية هي true.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.AllowDraggingToData بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### getDragToHide() {#getDragToHide--}
```
public boolean getDragToHide()
```


يشير إلى ما إذا كان يمكن إزالة هذا الحقل المحوري من عرض PivotTable. القيمة الافتراضية هي true.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.AllowRemovingFromView بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### getDragToPage() {#getDragToPage--}
```
public boolean getDragToPage()
```


يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الصفحة. القيمة الافتراضية هي true.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.AllowDraggingToPage بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### getDragToRow() {#getDragToRow--}
```
public boolean getDragToRow()
```


يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الصف. القيمة الافتراضية هي true.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.AllowDraggingToRow بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### getFilters() {#getFilters--}
```
public PivotFilter[] getFilters()
```


يحصل على جميع عوامل تصفية المحور المطبقة لهذا الحقل المحوري.

**Returns:**
com.aspose.cells.PivotFilter[]
### getFormula() {#getFormula--}
```
public String getFormula()
```


يحصل على صيغة الحقل المحسوب. يعمل فقط مع الحقل المحسوب.

**Returns:**
java.lang.String
### getFunction() {#getFunction--}
```
public int getFunction()
```


يمثل الدالة المستخدمة لتلخيص حقل بيانات جدول المحور هذا.

انظر [ConsolidationFunction](../../com.aspose.cells/consolidationfunction).

**Returns:**
int
### getGroupSettings() {#getGroupSettings--}
```
public PivotFieldGroupSettings getGroupSettings()
```


يحصل على إعدادات التجميع للحقل المحوري.

**Remarks**

إذا لم يكن هذا الحقل مُجَمَّعًا، سيتم إرجاع Null.

**Returns:**
[PivotFieldGroupSettings](../../com.aspose.cells/pivotfieldgroupsettings)
### getInsertBlankRow() {#getInsertBlankRow--}
```
public boolean getInsertBlankRow()
```


يشير إلى ما إذا كان يجب إدراج سطر فارغ بعد كل عنصر. فقط لحقول الصفوف.

**Returns:**
boolean
### getItemCount() {#getItemCount--}
```
public int getItemCount()
```


يحصل على عدد العناصر الأساسية في هذا الحقل المحوري.

**Remarks**

ملاحظة: هذه الطريقة أصبحت الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.PivotItems.Count بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أغسطس 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getItems() {#getItems--}
```
public String[] getItems()
```


احصل على جميع تسميات عناصر المحور في هذا الحقل.

**Returns:**
java.lang.String[]
### getMaxValue() {#getMaxValue--}
```
public CellValue getMaxValue()
```


يحصل على القيمة القصوى لهذا الحقل.

**Remarks**

يعمل فقط لحقول الصف أو العمود التي يجب أن تكون قيمتها تاريخًا/وقتًا أو رقمًا أو فارغًا.

**Returns:**
[CellValue](../../com.aspose.cells/cellvalue) - 
### getMinValue() {#getMinValue--}
```
public CellValue getMinValue()
```


يحصل على القيمة القصوى لهذا الحقل.

**Remarks**

يعمل فقط لحقول الصف أو العمود التي يجب أن تكون قيمتها تاريخًا/وقتًا أو رقمًا أو فارغًا.

**Returns:**
[CellValue](../../com.aspose.cells/cellvalue) - 
### getName() {#getName--}
```
public String getName()
```


يمثل اسم حقل المحور.

**Returns:**
java.lang.String
### getNonAutoSortDefault() {#getNonAutoSortDefault--}
```
public boolean getNonAutoSortDefault()
```


يشير إلى ما إذا كانت عملية الفرز التي ستُطبق على هذا الحقل المحوري هي عملية فرز تلقائي أم فرز بيانات بسيط.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية !PivotField.SortSetting.IsSimpleSort بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### getNumber() {#getNumber--}
```
public int getNumber()
```


يمثل تنسيق العرض المدمج للأرقام والتواريخ.

**Returns:**
int
### getNumberFormat() {#getNumberFormat--}
```
public String getNumberFormat()
```


يمثل تنسيق العرض المخصص للأرقام والتواريخ.

**Returns:**
java.lang.String
### getOriginalItems() {#getOriginalItems--}
```
public String[] getOriginalItems()
```


احصل على العناصر الأساسية الأصلية؛

**Returns:**
java.lang.String[]
### getPivotFilterByType(int type) {#getPivotFilterByType-int-}
```
public PivotFilter getPivotFilterByType(int type)
```


يحصل على مرشح المحور للحقل المحوري حسب النوع

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| النوع | int |  |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### getPivotFilters() {#getPivotFilters--}
```
public ArrayList getPivotFilters()
```


يحصل على عوامل تصفية المحور للحقل المحوري

**Remarks**

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotField.GetFilters(). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ نوفمبر 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
java.util.ArrayList
### getPivotItems() {#getPivotItems--}
```
public PivotItemCollection getPivotItems()
```


يحصل على عناصر المحور للحقل المحوري

**Returns:**
[PivotItemCollection](../../com.aspose.cells/pivotitemcollection)
### getPosition() {#getPosition--}
```
public int getPosition()
```


يمثل الفهرس لـ [PivotField](../../com.aspose.cells/pivotfield) في المنطقة.

**Returns:**
int
### getRegionType() {#getRegionType--}
```
public int getRegionType()
```


يحدد منطقة جدول المحور التي يُعرض فيها هذا الحقل.

انظر [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Returns:**
int
### getShowAllItems() {#getShowAllItems--}
```
public boolean getShowAllItems()
```


يشير إلى ما إذا كان يجب عرض جميع العناصر في عرض PivotTable، حتى إذا لم تحتوي على بيانات ملخص. القيمة الافتراضية هي false.

**Returns:**
boolean
### getShowCompact() {#getShowCompact--}
```
public boolean getShowCompact()
```


يشير إلى ما إذا كان يجب عرض تسميات الحقل التالي في نفس العمود في عرض Pivot Table. يقتصر على حقول الصف.

**Remarks**

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.ShowInCompactForm بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ نوفمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### getShowInCompactForm() {#getShowInCompactForm--}
```
public boolean getShowInCompactForm()
```


يحصل على قيمة تشير إلى ما إذا كان حقل الصف هذا يستخدم تخطيط الشكل المدمج. يطبق فقط على حقول الصف.

**Remarks**

الشكل المدمج هو وضع فرعي من تخطيط المخطط التفصيلي. هذا الإعداد يعمل فقط عندما تكون [getShowInOutlineForm()](../../com.aspose.cells/pivotfield\#getShowInOutlineForm--) true.

**Returns:**
boolean
### getShowInOutlineForm() {#getShowInOutlineForm--}
```
public boolean getShowInOutlineForm()
```


يحصل على قيمة تشير إلى ما إذا كان حقل الصف هذا يستخدم تخطيط المخطط التفصيلي. يطبق فقط على حقول الصف.

**Returns:**
boolean
### getShowSubtotalAtTop() {#getShowSubtotalAtTop--}
```
public boolean getShowSubtotalAtTop()
```


يشير إلى ما إذا كان يجب عرض المجاميع الفرعية في أعلى أو أسفل العناصر.

**Remarks**

يعمل فقط على حقول المحور في منطقة الصف عندما تكون ShowInOutlineForm true.

**Returns:**
boolean
### getShowValuesSetting() {#getShowValuesSetting--}
```
public PivotShowValuesSetting getShowValuesSetting()
```


يحصل على إعدادات عرض القيم كما عندما يكون حساب ShowDataAs قيد الاستخدام.

**Returns:**
[PivotShowValuesSetting](../../com.aspose.cells/pivotshowvaluessetting)
### getSortSetting() {#getSortSetting--}
```
public PivotFieldSortSetting getSortSetting()
```


يحصل على جميع إعدادات الفرز التلقائي

**Returns:**
[PivotFieldSortSetting](../../com.aspose.cells/pivotfieldsortsetting)
### getSubtotals() {#getSubtotals--}
```
public int getSubtotals()
```


يحصل على المجاميع الفرعية للحقل. يقتصر على حقول المحور من نوع الصف أو العمود.

انظر [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype).

**Example**

```
         //No subtotals
         rowField.setSubtotals(PivotFieldSubtotalType.NONE);
         //Automatic subtotals
         //rowField.Subtotals = PivotFieldSubtotalType.Automatic;
         //Single subtotals: Sum
         //rowField.Subtotals = PivotFieldSubtotalType.Sum;
         //Multipl subtotals: Sum and count numbers 
         //rowField.Subtotals = PivotFieldSubtotalType.Sum | PivotFieldSubtotalType.Count;
```

**Returns:**
int
### getSubtotals(int subtotalType) {#getSubtotals-int-}
```
public boolean getSubtotals(int subtotalType)
```


يحدد ما إذا كان سيتم عرض المجمل الفرعي المحدد لهذا الحقل المحوري.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). نوع المجموع الفرعي. |

**Returns:**
boolean - يُرجع ما إذا كان يتم عرض المجموع الفرعي المحدد.
### getTop10AutoShowSettings() {#getTop10AutoShowSettings--}
```
public PivotFieldTop10AutoShowSettings getTop10AutoShowSettings()
```


يحصل على إعدادات AutoShow لأفضل 10 لحقل محوري.

**Returns:**
[PivotFieldTop10AutoShowSettings](../../com.aspose.cells/pivotfieldtop10autoshowsettings)
### group() {#group--}
```
public boolean group()
```


يقوم بتجميع الحقل تلقائيًا.

**Remarks**

إذا كان الحقل يحتوي فقط على فراغ وتاريخ/وقت، فسيتم تجميع الحقل حسب الأشهر. إذا كان الحقل يحتوي فقط على فراغ ورقم، فسيتم تجميعه حسب الرقم. وإلا سيُرجع false فقط دون أي تجميع.

**Returns:**
boolean
### group(PivotFieldGroupOptions options) {#group-com.aspose.cells.PivotFieldGroupOptions-}
```
public boolean group(PivotFieldGroupOptions options)
```


يقوم بتجميع الحقل المحوري مع الخيارات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| options | [PivotFieldGroupOptions](../../com.aspose.cells/pivotfieldgroupoptions) | خيارات إعدادات تجميع حقل المحور. |

**Returns:**
boolean -
### groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField) {#groupBy-boolean-com.aspose.cells.DateTime-boolean-com.aspose.cells.DateTime-int---double-boolean-}
```
public boolean groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField)
```


قم بتجميع الملف حسب أنواع تجميع التاريخ.

**Remarks**

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotField.Group(PivotFieldGroupOptions). سيتم إزالة هذه الطريقة بعد 6 أشهر منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isAutoStart | boolean | يشير إلى ما إذا كان يجب الكشف التلقائي عن قيمة تاريخ/وقت البدء. |
| start | [DateTime](../../com.aspose.cells/datetime) | تاريخ/وقت البدء |
| isAutoEnd | boolean | يشير إلى ما إذا كان يجب الكشف التلقائي عن قيمة تاريخ/وقت النهاية. |
| end | [DateTime](../../com.aspose.cells/datetime) | نهاية تاريخ/وقت |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). أنواع التجميع |
| الفاصل الزمني | double | الفاصل الزمني |
| firstAsNewField | boolean | يشير إلى ما إذا كان يتم إضافة حقل جديد إلى pivottable. يقتصر على العنصر الأول في المجموعة. |

**Returns:**
منطقي - False يعني أن هذا الحقل لا يمكن تجميعه حسب التاريخ والوقت.
### groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField) {#groupBy-boolean-double-boolean-double-double-boolean-}
```
public boolean groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField)
```


قم بتجميع الملف حسب الرقم.

**Remarks**

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotField.Group(PivotFieldGroupOptions). سيتم إزالة هذه الطريقة بعد 6 أشهر منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isAutoStart | boolean | يشير إلى ما إذا كان يجب اكتشاف قيمة البداية تلقائيًا. |
| البداية | double | قيمة البداية |
| isAutoEnd | boolean | يشير إلى ما إذا كان يجب اكتشاف قيمة النهاية تلقائيًا. |
| النهاية | double | نهاية القيمة |
| الفاصل الزمني | double | الفاصل الزمني |
| newField | boolean | يشير إلى ما إذا كان سيتم إضافة حقل جديد إلى جدول المحور. |

**Returns:**
منطقي - False يعني أن هذا الحقل لا يمكن تجميعه حسب التاريخ والوقت.
### groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField) {#groupBy-com.aspose.cells.CustomPiovtFieldGroupItem---boolean-}
```
public boolean groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField)
```


قم بتجميع الحقل مخصصًا.

**Remarks**

ملاحظة: هذه الطريقة الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotField.Group(PivotFieldGroupOptions options) مع الخاصية PivotFieldGroupOptions.DiscreteGroupItems. سيتم إزالة هذه الطريقة بعد 6 أشهر منذ يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| customGroupItems | [CustomPiovtFieldGroupItem\[\]](../../com.aspose.cells/custompiovtfieldgroupitem) | عناصر المجموعة المخصصة. |
| newField | boolean | يشير إلى ما إذا كان سيتم إضافة حقل جديد إلى جدول المحور. |

**Returns:**
منطقي - False يعني أن هذا الحقل لا يمكن تجميعه حسب التاريخ والوقت.
### groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField) {#groupBy-com.aspose.cells.DateTime-com.aspose.cells.DateTime-int---double-boolean-}
```
public boolean groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField)
```


قم بتجميع الملف حسب أنواع تجميع التاريخ.

**Remarks**

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotField.Group(PivotFieldGroupOptions). سيتم إزالة هذه الطريقة بعد 6 أشهر منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| start | [DateTime](../../com.aspose.cells/datetime) | تاريخ/وقت البدء |
| end | [DateTime](../../com.aspose.cells/datetime) | نهاية تاريخ/وقت |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). أنواع التجميع |
| الفاصل الزمني | double | الفاصل الزمني |
| firstAsNewField | boolean | يشير إلى ما إذا كان يتم إضافة حقل جديد إلى pivottable. يقتصر على العنصر الأول في المجموعة. |

**Returns:**
منطقي - False يعني أن هذا الحقل لا يمكن تجميعه حسب التاريخ والوقت.
### groupBy(DiscreteGroupItem[] customGroupItems, boolean newField) {#groupBy-com.aspose.cells.DiscreteGroupItem---boolean-}
```
public boolean groupBy(DiscreteGroupItem[] customGroupItems, boolean newField)
```


قم بتجميع الحقل مخصصًا.

**Remarks**

ملاحظة: هذه الطريقة الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotField.Group(PivotFieldGroupOptions options) مع الخاصية PivotFieldGroupOptions.DiscreteGroupItems. سيتم إزالة هذه الطريقة بعد 6 أشهر منذ يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| customGroupItems | [DiscreteGroupItem\[\]](../../com.aspose.cells/discretegroupitem) | عناصر المجموعة المخصصة. |
| newField | boolean | يشير إلى ما إذا كان سيتم إضافة حقل جديد إلى جدول المحور. |

**Returns:**
boolean -
### groupBy(double interval, boolean newField) {#groupBy-double-boolean-}
```
public void groupBy(double interval, boolean newField)
```


قم بتجميع الحقل تلقائيًا باستخدام الفاصل الزمني

**Remarks**

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotField.Group(PivotFieldGroupOptions). سيتم إزالة هذه الطريقة بعد 6 أشهر منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفاصل الزمني | double | الداخلية للمجموعة. سيتم تعيين قيمة تلقائية إذا كانت صفرًا، |
| newField | boolean | يشير إلى ما إذا كان سيتم إضافة حقل جديد إلى جدول المحور. فقط لمجموعة DateTime. |

### groupBy(double start, double end, double interval, boolean newField) {#groupBy-double-double-double-boolean-}
```
public boolean groupBy(double start, double end, double interval, boolean newField)
```


قم بتجميع الملف حسب الرقم.

**Remarks**

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotField.Group(PivotFieldGroupOptions). سيتم إزالة هذه الطريقة بعد 6 أشهر منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| البداية | double | قيمة البداية |
| النهاية | double | نهاية القيمة |
| الفاصل الزمني | double | الفاصل الزمني |
| newField | boolean | يشير إلى ما إذا كان سيتم إضافة حقل جديد إلى جدول المحور. |

**Returns:**
منطقي - False يعني أن هذا الحقل لا يمكن تجميعه حسب التاريخ والوقت.
### groupBy(int[] groups, double interval, boolean newField) {#groupBy-int---double-boolean-}
```
public void groupBy(int[] groups, double interval, boolean newField)
```


قم بتجميع الحقل تلقائيًا باستخدام internal

**Remarks**

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotField.Group(PivotFieldGroupOptions). سيتم إزالة هذه الطريقة بعد 6 أشهر منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). أنواع التجميع |
| الفاصل الزمني | double | الداخلية للمجموعة. سيتم تعيين قيمة تلقائية إذا كانت صفرًا، يعمل فقط لتجميع حسب الأرقام أو الأيام. |
| newField | boolean | يشير إلى ما إذا كان سيتم إضافة حقل جديد إلى جدول المحور. |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hideAllDetails() {#hideAllDetails--}
```
public void hideAllDetails()
```


يخفي جميع تفاصيل كل عنصر محوري.

### hideDetail(boolean isHiddenDetail) {#hideDetail-boolean-}
```
public void hideDetail(boolean isHiddenDetail)
```


يضبط ما إذا كانت تفاصيل جميع PivotItems في حقل محور مخفية. أي طي/فتح هذا الحقل.

**Remarks**

ملاحظة: هذه الطريقة الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotItemsCollection.HideAllDetails() وطريقة UnhideAllDetails() بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ نوفمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isHiddenDetail | boolean | ما إذا كان سيتم إخفاء تفاصيل حقل المحور. |

### hideItem(int index, boolean isHidden) {#hideItem-int-boolean-}
```
public void hideItem(int index, boolean isHidden)
```


يحدد ما إذا كان PivotItem المحدد في حقل البيانات مخفيًا.

**Remarks**

ملاحظة: هذه الطريقة الآن مهجورة. بدلاً من ذلك، يرجى استخدام الخاصية PivotField.PivotItems[int].IsHidden بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أغسطس 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس الـ pivotItem في الـ pivotField. |
| isHidden | boolean | ما إذا كان PivotItem المحدد مخفيًا |

### hideItem(String itemValue, boolean isHidden) {#hideItem-java.lang.String-boolean-}
```
public void hideItem(String itemValue, boolean isHidden)
```


يحدد ما إذا كان PivotItem المحدد في حقل البيانات مخفيًا.

**Remarks**

ملاحظة: هذه الطريقة الآن مهجورة. بدلاً من ذلك، يرجى استخدام الخاصية PivotField.PivotItems[string].IsHidden بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أغسطس 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| itemValue | java.lang.String | اسم الـ pivotItem في الـ pivotField. |
| isHidden | boolean | ما إذا كان PivotItem المحدد مخفيًا |

### hideItemDetail(int index, boolean isHiddenDetail) {#hideItemDetail-int-boolean-}
```
public void hideItemDetail(int index, boolean isHiddenDetail)
```


يحدد ما إذا كانت تفاصيل PivotItem المحدد في حقل محوري مخفية.

**Remarks**

ملاحظة: هذه الطريقة الآن مهجورة. بدلاً من ذلك، يرجى استخدام الخاصية PivotField.PivotItems[int].IsDetailHidden بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أغسطس 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس الـ pivotItem في الـ pivotField. |
| isHiddenDetail | boolean | ما إذا كان PivotItem المحدد مخفيًا |

### initPivotItems() {#initPivotItems--}
```
public void initPivotItems()
```


تهيئة عناصر pivot للحقل المحوري

**Remarks**

ملاحظة: هذه الطريقة الآن مهجورة. يرجى ببساطة إزالة استدعاء هذه الطريقة. سيتم إزالة هذه الطريقة بعد 6 أشهر منذ أكتوبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### isAscendShow() {#isAscendShow--}
```
public boolean isAscendShow()
```


يشير إلى ما إذا كان حقل PivotTable المحدد يُعرض تلقائيًا تصاعديًا.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.Top10AutoShowSettings.IsTop أو طريقة PivotField.Top10AutoShow() بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### isAscendSort() {#isAscendSort--}
```
public boolean isAscendSort()
```


يحدد ما إذا كانت عناصر هذا الحقل المحوري مرتبة تلقائيًا تصاعديًا.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.SortSetting.SortType أو طريقة PivotField.SortBy() بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### isAutoShow() {#isAutoShow--}
```
public boolean isAutoShow()
```


يحدد ما إذا كان حقل PivotTable المحدد يُظهر تلقائيًا.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.Top10AutoShowSettings.IsAutoShow أو طريقة PivotField.Top10AutoShow() بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### isAutoSort() {#isAutoSort--}
```
public boolean isAutoSort()
```


يحدد ما إذا كانت عناصر حقل PivotTable هذا مرتبة تلقائيًا.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.SortSetting.SortType أو طريقة PivotField.SortBy() بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### isAutoSubtotals() {#isAutoSubtotals--}
```
public boolean isAutoSubtotals()
```


يشير إلى ما إذا كان الحقل المحدد يعرض المجاميع الفرعية التلقائية. القيمة الافتراضية هي true.

**Returns:**
boolean
### isCalculatedField() {#isCalculatedField--}
```
public boolean isCalculatedField()
```


يحدد ما إذا كان هذا الحقل المحوري حقلًا محسوبًا.

**Returns:**
boolean
### isHiddenItem(int index) {#isHiddenItem-int-}
```
public boolean isHiddenItem(int index)
```


يحدد ما إذا كان PivotItem المحدد مخفيًا.

**Remarks**

ملاحظة: هذه الطريقة الآن مهجورة. بدلاً من ذلك، يرجى استخدام الخاصية PivotField.PivotItems[int].IsHidden بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أغسطس 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس الـ pivotItem في الـ pivotField. |

**Returns:**
منطقي - ما إذا كان PivotItem المحدد مخفيًا
### isHiddenItemDetail(int index) {#isHiddenItemDetail-int-}
```
public boolean isHiddenItemDetail(int index)
```


يحدد ما إذا كان يجب إخفاء تفاصيل PivotItem المحدد..

**Remarks**

ملاحظة: هذه الطريقة الآن مهجورة. بدلاً من ذلك، يرجى استخدام الخاصية PivotField.PivotItems[int].IsDetailHidden بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أغسطس 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس الـ pivotItem في الـ pivotField. |

**Returns:**
منطقي - ما إذا كان تفاصيل PivotItem المحدد مخفية
### isIncludeNewItemsInFilter() {#isIncludeNewItemsInFilter--}
```
public boolean isIncludeNewItemsInFilter()
```


يشير إلى ما إذا كان يجب تضمين عناصر جديدة إلى الحقل في الفلتر اليدوي. القيمة الافتراضية هي false.

**Returns:**
boolean
### isInsertPageBreaksBetweenItems() {#isInsertPageBreaksBetweenItems--}
```
public boolean isInsertPageBreaksBetweenItems()
```


يشير إلى ما إذا كان يجب إدراج فواصل صفحات بعد كل عنصر. القيمة الافتراضية هي false.

**Returns:**
boolean
### isMultipleItemSelectionAllowed() {#isMultipleItemSelectionAllowed--}
```
public boolean isMultipleItemSelectionAllowed()
```


يشير إلى ما إذا كان يمكن اختيار عناصر متعددة في حقل الصفحة. القيمة الافتراضية هي false.

**Remarks**

فقط لحقول الصفحة (الفلتر).

**Returns:**
boolean
### isRepeatItemLabels() {#isRepeatItemLabels--}
```
public boolean isRepeatItemLabels()
```


يشير إلى ما إذا كان يجب تكرار تسميات الحقل في منطقة الصف أو العمود. القيمة الافتراضية هي false.

**Returns:**
boolean
### isValueFields() {#isValueFields--}
```
public boolean isValueFields()
```


يشير إلى ما إذا كان هذا الحقل يمثل حقول القيم.

**Remarks**

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.IsValuesField. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ نوفمبر 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### isValuesField() {#isValuesField--}
```
public boolean isValuesField()
```


يشير إلى ما إذا كان هذا الحقل يمثل حقل القيم.

**Remarks**

يعمل فقط عندما يكون هناك حقلان بيانات أو أكثر في عرض جدول المحور.

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




### setAllowDraggingToColumn(boolean value) {#setAllowDraggingToColumn-boolean-}
```
public void setAllowDraggingToColumn(boolean value)
```


يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة العمود. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAllowDraggingToData(boolean value) {#setAllowDraggingToData-boolean-}
```
public void setAllowDraggingToData(boolean value)
```


يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة القيم. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAllowDraggingToPage(boolean value) {#setAllowDraggingToPage-boolean-}
```
public void setAllowDraggingToPage(boolean value)
```


يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الصفحة. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAllowDraggingToRow(boolean value) {#setAllowDraggingToRow-boolean-}
```
public void setAllowDraggingToRow(boolean value)
```


يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الصف. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAllowRemovingFromView(boolean value) {#setAllowRemovingFromView-boolean-}
```
public void setAllowRemovingFromView(boolean value)
```


يشير إلى ما إذا كان يمكن إزالة هذا الحقل المحوري من عرض PivotTable. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAscendShow(boolean value) {#setAscendShow-boolean-}
```
public void setAscendShow(boolean value)
```


يشير إلى ما إذا كان حقل PivotTable المحدد يُعرض تلقائيًا تصاعديًا.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.Top10AutoShowSettings.IsTop أو طريقة PivotField.Top10AutoShow() بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAscendSort(boolean value) {#setAscendSort-boolean-}
```
public void setAscendSort(boolean value)
```


يحدد ما إذا كانت عناصر هذا الحقل المحوري مرتبة تلقائيًا تصاعديًا.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.SortSetting.SortType أو طريقة PivotField.SortBy() بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAutoShow(boolean value) {#setAutoShow-boolean-}
```
public void setAutoShow(boolean value)
```


يحدد ما إذا كان حقل PivotTable المحدد يُظهر تلقائيًا.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.Top10AutoShowSettings.IsAutoShow أو طريقة PivotField.Top10AutoShow() بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAutoShowCount(int value) {#setAutoShowCount-int-}
```
public void setAutoShowCount(int value)
```


يمثل عدد العناصر العليا أو السفلى التي تُظهر تلقائيًا في حقل PivotTable المحدد.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.Top10AutoShowSettings.AutoShowCount أو طريقة PivotField.Top10AutoShow() بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setAutoShowField(int value) {#setAutoShowField-int-}
```
public void setAutoShowField(int value)
```


يمثل فهرس الحقل المعروض تلقائيًا. -1 يعني PivotField نفسه. يجب أن يكون فهرس حقول البيانات.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.Top10AutoShowSettings.RankBy أو طريقة PivotField.Top10AutoShow() بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setAutoSort(boolean value) {#setAutoSort-boolean-}
```
public void setAutoSort(boolean value)
```


يحدد ما إذا كانت عناصر حقل PivotTable هذا مرتبة تلقائيًا.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.SortSetting.SortType أو طريقة PivotField.SortBy() بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAutoSortField(int value) {#setAutoSortField-int-}
```
public void setAutoSortField(int value)
```


يمثل فهرس الحقل الذي يتم فرزه تلقائيًا. -1 يعني PivotField نفسه، والقيم الأخرى تعني موقع حقول البيانات.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.SortSetting.SortBy أو طريقة PivotField.SortBy() بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setAutoSubtotals(boolean value) {#setAutoSubtotals-boolean-}
```
public void setAutoSubtotals(boolean value)
```


يشير إلى ما إذا كان الحقل المحدد يعرض المجاميع الفرعية التلقائية. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setBaseIndex(int value) {#setBaseIndex-int-}
```
public void setBaseIndex(int value)
```


يمثل الفهرس في حقول PivotField المصدر.

**Remarks**

ملاحظة: هذه الدالة الضابطة لهذه الخاصية أصبحت الآن غير صالحة. سيتم إزالة هذه الدالة الضابطة بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setCurrentPageItem(short value) {#setCurrentPageItem-short-}
```
public void setCurrentPageItem(short value)
```


يضبط العنصر الصفحي المعروض حاليًا لهذا الحقل المحوري (حقل الصفحة فقط).

**Remarks**

استخدم [PivotItem.ALL\_PAGE\_ITEMS\_INDEX](../../com.aspose.cells/pivotitem\#ALL-PAGE-ITEMS-INDEX) (0x7FFD) كقيمة إشارة لتحديد "Select All". هذه علامة معرفة مسبقًا وليست فهرس عنصر صالح.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | short |  |

### setCurrentPageItemText(String value) {#setCurrentPageItemText-java.lang.String-}
```
public void setCurrentPageItemText(String value)
```


يحصل على نص العرض للعنصر الحالي للصفحة لهذا الحقل المحوري (حقل الصفحة فقط).

**Remarks**

يرجع "(All)" عندما تكون [getCurrentPageItem()](../../com.aspose.cells/pivotfield\#getCurrentPageItem--) مساوية لـ [PivotItem.ALL\_PAGE\_ITEMS\_INDEX](../../com.aspose.cells/pivotitem\#ALL-PAGE-ITEMS-INDEX). للقيم الأخرى، يرجع تمثيل السلسلة لفهرس العنصر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


يمثل اسم العرض لحقل المحور في عرض جدول المحور.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setDragToColumn(boolean value) {#setDragToColumn-boolean-}
```
public void setDragToColumn(boolean value)
```


يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة العمود. القيمة الافتراضية هي true.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.AllowDraggingToColumn بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDragToData(boolean value) {#setDragToData-boolean-}
```
public void setDragToData(boolean value)
```


يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة القيم. القيمة الافتراضية هي true.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.AllowDraggingToData بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDragToHide(boolean value) {#setDragToHide-boolean-}
```
public void setDragToHide(boolean value)
```


يشير إلى ما إذا كان يمكن إزالة هذا الحقل المحوري من عرض PivotTable. القيمة الافتراضية هي true.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.AllowRemovingFromView بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDragToPage(boolean value) {#setDragToPage-boolean-}
```
public void setDragToPage(boolean value)
```


يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الصفحة. القيمة الافتراضية هي true.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.AllowDraggingToPage بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDragToRow(boolean value) {#setDragToRow-boolean-}
```
public void setDragToRow(boolean value)
```


يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الصف. القيمة الافتراضية هي true.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.AllowDraggingToRow بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFunction(int value) {#setFunction-int-}
```
public void setFunction(int value)
```


يمثل الدالة المستخدمة لتلخيص حقل بيانات جدول المحور هذا.

انظر [ConsolidationFunction](../../com.aspose.cells/consolidationfunction).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setIncludeNewItemsInFilter(boolean value) {#setIncludeNewItemsInFilter-boolean-}
```
public void setIncludeNewItemsInFilter(boolean value)
```


يشير إلى ما إذا كان يجب تضمين عناصر جديدة إلى الحقل في الفلتر اليدوي. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setInsertBlankRow(boolean value) {#setInsertBlankRow-boolean-}
```
public void setInsertBlankRow(boolean value)
```


يشير إلى ما إذا كان يجب إدراج سطر فارغ بعد كل عنصر. فقط لحقول الصفوف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setInsertPageBreaksBetweenItems(boolean value) {#setInsertPageBreaksBetweenItems-boolean-}
```
public void setInsertPageBreaksBetweenItems(boolean value)
```


يشير إلى ما إذا كان يجب إدراج فواصل صفحات بعد كل عنصر. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setMultipleItemSelectionAllowed(boolean value) {#setMultipleItemSelectionAllowed-boolean-}
```
public void setMultipleItemSelectionAllowed(boolean value)
```


يشير إلى ما إذا كان يمكن اختيار عناصر متعددة في حقل الصفحة. القيمة الافتراضية هي false.

**Remarks**

فقط لحقول الصفحة (الفلتر).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


يمثل اسم حقل المحور.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setNonAutoSortDefault(boolean value) {#setNonAutoSortDefault-boolean-}
```
public void setNonAutoSortDefault(boolean value)
```


يشير إلى ما إذا كانت عملية الفرز التي ستُطبق على هذا الحقل المحوري هي عملية فرز تلقائي أم فرز بيانات بسيط.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية !PivotField.SortSetting.IsSimpleSort بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


يمثل تنسيق العرض المدمج للأرقام والتواريخ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setNumberFormat(String value) {#setNumberFormat-java.lang.String-}
```
public void setNumberFormat(String value)
```


يمثل تنسيق العرض المخصص للأرقام والتواريخ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setRepeatItemLabels(boolean value) {#setRepeatItemLabels-boolean-}
```
public void setRepeatItemLabels(boolean value)
```


يشير إلى ما إذا كان يجب تكرار تسميات الحقل في منطقة الصف أو العمود. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowAllItems(boolean value) {#setShowAllItems-boolean-}
```
public void setShowAllItems(boolean value)
```


يشير إلى ما إذا كان يجب عرض جميع العناصر في عرض PivotTable، حتى إذا لم تحتوي على بيانات ملخص. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowCompact(boolean value) {#setShowCompact-boolean-}
```
public void setShowCompact(boolean value)
```


يشير إلى ما إذا كان يجب عرض تسميات الحقل التالي في نفس العمود في عرض Pivot Table. يقتصر على حقول الصف.

**Remarks**

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.ShowInCompactForm بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ نوفمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowInCompactForm(boolean value) {#setShowInCompactForm-boolean-}
```
public void setShowInCompactForm(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان حقل الصف هذا يستخدم تخطيط الشكل المدمج. ينطبق فقط على حقول الصف.

**Remarks**

الشكل المدمج هو وضع فرعي من تخطيط المخطط التفصيلي. هذا الإعداد يعمل فقط عندما تكون [getShowInOutlineForm()](../../com.aspose.cells/pivotfield\#getShowInOutlineForm--) true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowInOutlineForm(boolean value) {#setShowInOutlineForm-boolean-}
```
public void setShowInOutlineForm(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان حقل الصف هذا يستخدم تخطيط المخطط التفصيلي. ينطبق فقط على حقول الصف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowSubtotalAtTop(boolean value) {#setShowSubtotalAtTop-boolean-}
```
public void setShowSubtotalAtTop(boolean value)
```


يشير إلى ما إذا كان يجب عرض المجاميع الفرعية في أعلى أو أسفل العناصر.

**Remarks**

يعمل فقط على حقول المحور في منطقة الصف عندما تكون ShowInOutlineForm true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSubtotals(int value) {#setSubtotals-int-}
```
public void setSubtotals(int value)
```


يضبط المجاميع الفرعية للحقل. يخص فقط حقول الصف أو العمود في المحور.

انظر [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setSubtotals(int subtotalType, boolean shown) {#setSubtotals-int-boolean-}
```
public void setSubtotals(int subtotalType, boolean shown)
```


يضبط طريقة تجميع الحقل المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |
| معروض | boolean | ما إذا كان الحقل المحدد يعرض تلك المجاميع الفرعية. |

### showAllDetails() {#showAllDetails--}
```
public void showAllDetails()
```


اعرض جميع تفاصيل كل عنصر محوري.

### showValuesAs(int showValuesAsType, int baseField, int baseItem) {#showValuesAs-int-int-int-}
```
public void showValuesAs(int showValuesAsType, int baseField, int baseItem)
```


يضبط حساب "عرض القيم كـ" لهذا الحقل المحوري.

**Remarks**

فقط لحقل البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| showValuesAsType | int | [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype). نوع حساب \"إظهار القيم كـ\". |
| baseField | int | فهرس الحقل الأساسي المستخدم في الحساب. |
| baseItem | int | فهرس العنصر الأساسي المستخدم في الحساب. استخدم [PivotShowValuesSetting.PREVIOUS\\_PIVOT\\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\\#PREVIOUS-PIVOT-ITEM) (-1) للعنصر السابق، [PivotShowValuesSetting.NEXT\\_PIVOT\\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\\#NEXT-PIVOT-ITEM) (-2) للعنصر التالي؛ القيم غير\\u9225\\u6182egative تشير إلى الفهرس الترتيبي لعنصر محور محدد. |

### showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem) {#showValuesAs-int-int-int-int-}
```
public void showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem)
```


يعرض قيم حقل البيانات بتنسيق عرض مختلف عندما يكون حساب ShowDataAs قيد الاستخدام.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotField.ShowValuesAs(PivotShowValuesAsType,int,int). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ نوفمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| displayFormat | int | [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat). نوع تنسيق عرض البيانات. |
| baseField | int | الفهرس إلى الحقل الذي تستند إليه عملية حساب ShowDataAs. |
| baseItemPositionType | int | [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype). نوع موضع العنصر الأساسي. |
| baseItem | int | الفهرس إلى العنصر الأساسي الذي تستند إليه عملية حساب ShowDataAs. يعمل فقط عندما يكون baseItemPositionType مخصصًا. |

### showValuesAs(int showValuesAsType, String baseField, String baseItem) {#showValuesAs-int-java.lang.String-java.lang.String-}
```
public void showValuesAs(int showValuesAsType, String baseField, String baseItem)
```


يضبط تكوين حساب "عرض القيم كـ" لهذا حقل البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| showValuesAsType | int | [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype). نوع العملية الحسابية لـ Show Values As. |
| baseField | java.lang.String | اسم الحقل الأساسي المستخدم في العملية الحسابية. |
| baseItem | java.lang.String | تسمية عنصر محور عادي. يقبل أيضًا الكلمات المفتاحية المحجوزة: `(previous)` للعنصر السابق، `(next)` للعنصر التالي. مرر `null` إذا كان نوع العملية الحسابية المحدد لا يتطلب عنصرًا أساسيًا. |

### sortBy(int sortType) {#sortBy-int-}
```
public void sortBy(int sortType)
```


يرتب هذا الحقل المحوري.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). نوع فرز هذا الحقل. |

### sortBy(int sortType, int fieldSortedBy) {#sortBy-int-int-}
```
public void sortBy(int sortType, int fieldSortedBy)
```


يرتب هذا الحقل المحوري.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotField.SortBy(SortOrder, int,string) أو خاصية PivotField.IsAutoSort. سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). نوع فرز هذا الحقل. |
| fieldSortedBy | int | فهرس حقل المحور الذي يتم الفرز بناءً عليه. -1 يعني الفرز حسب تسميات البيانات لهذا الحقل، والقيم الأخرى تعني فهرس حقل البيانات الذي يتم الفرز بناءً عليه. |

### sortBy(int sortType, int fieldSortedBy, int dataType, String cellName) {#sortBy-int-int-int-java.lang.String-}
```
public void sortBy(int sortType, int fieldSortedBy, int dataType, String cellName)
```


يرتب هذا الحقل المحوري.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotField.SortBy(SortOrder, int,string). سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). نوع فرز هذا الحقل. |
| fieldSortedBy | int | فهرس حقل المحور الذي يتم الفرز بناءً عليه. -1 يعني الفرز حسب تسميات البيانات لهذا الحقل، والقيم الأخرى تعني فهرس حقل البيانات الذي يتم الفرز بناءً عليه. |
| dataType | int | [PivotLineType](../../com.aspose.cells/pivotlinetype). نوع البيانات التي يتم الفرز بناءً عليها. |
| cellName | java.lang.String | الفرز حسب القيم في الصف أو العمود |

### sortBy(int sortType, int fieldSortedBy, String cellName) {#sortBy-int-int-java.lang.String-}
```
public void sortBy(int sortType, int fieldSortedBy, String cellName)
```


يرتب هذا الحقل المحوري.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). نوع فرز هذا الحقل. |
| fieldSortedBy | int | فهرس حقل المحور الذي يتم الفرز بناءً عليه. -1 يعني الفرز حسب تسميات البيانات لهذا الحقل، والقيم الأخرى تعني فهرس حقل البيانات الذي يتم الفرز بناءً عليه. |
| cellName | java.lang.String | الفرز حسب القيم في الصف أو العمود. إذا كان Null، يتم التجميع حسب إجمالي الحقل، وإلا يتم التجميع حسب القيم في العمود أو الصف المحدد. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### top10AutoShow(boolean isAutoShow, boolean isTop, int count, int rankBy) {#top10AutoShow-boolean-boolean-int-int-}
```
public void top10AutoShow(boolean isAutoShow, boolean isTop, int count, int rankBy)
```


يضبط إعدادات العرض التلقائي Top10 لهذا الحقل المحوري.

**Remarks**

تقوم هذه الطريقة بتكوين تنسيق .XLS الثنائي: AutoShow (Top10) هو الخيار الأصلي والوحيد المدعوم. XLSX (OpenXML): تنسيق الملف الأساسي يدعم Top10 AutoShow، لكن واجهة المستخدم في Excel 2007 وما بعده تعرض ذلك فقط عبر مرشح Top10. إذا لم تكن توافقية XLS مطلوبة، يُنصح باستخدام مرشح Top10 بدلاً من ذلك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isAutoShow | boolean | true لتمكين AutoShow؛ false لتعطيله. |
| isTop | boolean | إذا كان true، يعرض العناصر العليا؛ إذا كان false، يعرض العناصر السفلى. |
| العدد | int | عدد العناصر العليا/السفلى التي سيتم عرضها. |
| rankBy | int | فهرس حقل البيانات المستخدم للترتيب. استخدم -1 للترتيب حسب قيم عنصر المحور نفسه. |

### ungroup() {#ungroup--}
```
public void ungroup()
```


إلغاء تجميع الحقل المحوري.

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

