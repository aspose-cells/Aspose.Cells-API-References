---
title: "PivotTable"
second_title: "Aspose.Cells for Java API Reference"
description: "وصف ملخص لـ PivotTable."
type: docs
url: /ar/java/com.aspose.cells/pivottable/
---

**Inheritance:**
java.lang.Object
```
public class PivotTable
```

وصف ملخص لـ PivotTable.

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
 
         //Add PivotFilter
         PivotFilter filter = pivot.getRowFields().get(0).filterTop10(0, PivotFilterType.PERCENT, false, 2);
 
 
         //Add PivotFormatCondition
         int formatIndex = pivot.getConditionalFormats().add();
         PivotConditionalFormat pfc = pivot.getConditionalFormats().get(formatIndex);
         pfc.addCellArea(pivot.getDataBodyRange());
         FormatConditionCollection fcc = pfc.getFormatConditions();
         int ii = fcc.addCondition(FormatConditionType.CELL_VALUE, OperatorType.GREATER_OR_EQUAL, "100", null);
 
         FormatCondition fc = fcc.get(ii);
 
         fc.getStyle().setBackgroundColor(Color.getRed());
 
          PivotTableCalculateOption calculateOption = new PivotTableCalculateOption();
          calculateOption.setRefreshData(true);
          calculateOption.setRefreshCharts(true);
          pivot.calculateData(calculateOption); 
 
         //do your business
 
         book.save("out.xlsx");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addCalculatedField(String name, String formula)](#addCalculatedField-java.lang.String-java.lang.String-) | يضيف حقلًا محسوبًا إلى حقل المحور ويسحبه إلى منطقة البيانات. |
| [addCalculatedField(String name, String formula, boolean dragToDataArea)](#addCalculatedField-java.lang.String-java.lang.String-boolean-) | يضيف حقلًا محسوبًا إلى حقل المحور. |
| [addFieldToArea(int fieldType, PivotField pivotField)](#addFieldToArea-int-com.aspose.cells.PivotField-) | يضيف الحقل إلى المنطقة المحددة. |
| [addFieldToArea(int fieldType, int baseFieldIndex)](#addFieldToArea-int-int-) | يضيف الحقل إلى المنطقة المحددة. |
| [addFieldToArea(int fieldType, String fieldName)](#addFieldToArea-int-java.lang.String-) | يضيف الحقل إلى المنطقة المحددة. |
| [calculateData()](#calculateData--) | يحسب بيانات جدول المحور إلى الخلايا. |
| [calculateData(PivotTableCalculateOption option)](#calculateData-com.aspose.cells.PivotTableCalculateOption-) | يحسب جدول المحور مع الخيارات. |
| [calculateRange()](#calculateRange--) | يحسب نطاق جدول المحور. |
| [changeDataSource(String[] source)](#changeDataSource-java.lang.String---) | تغيير مصدر البيانات لجدول المحور. |
| [clearAll()](#clearAll--) | إزالة جميع الحقول من المناطق. |
| [clearData()](#clearData--) | مسح البيانات وتنسيق عرض جدول المحور. |
| [clearFilters()](#clearFilters--) | يمسح جميع عوامل التصفية لهذا جدول المحور. |
| [copyStyle(PivotTable pivotTable)](#copyStyle-com.aspose.cells.PivotTable-) | ينسخ النمط المسمى من جدول محوري آخر. |
| [dispose()](#dispose--) | ينفذ مهام محددة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة ضبط الموارد غير المُدارة. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportViewToJson(PivotViewToJsonOptions options)](#exportViewToJson-com.aspose.cells.PivotViewToJsonOptions-) | يصدّر عرض المحور كـ JSON. |
| [fields(int fieldType)](#fields-int-) | يحصل على الحقول المحددة حسب نوع الحقل. |
| [format(CellArea ca, Style style)](#format-com.aspose.cells.CellArea-com.aspose.cells.Style-) | يقوم بتنسيق المنطقة المحددة في PivotTable. |
| [format(PivotArea pivotArea, Style style)](#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-) | يقوم بتنسيق المنطقة المحددة في PivotTable. |
| [format(int row, int column, Style style)](#format-int-int-com.aspose.cells.Style-) | يقوم بتنسيق الخلية في منطقة PivotTable |
| [formatAll(Style style)](#formatAll-com.aspose.cells.Style-) | قم بتنسيق جميع الخلايا في منطقة PivotTable |
| [formatRow(int row, Style style)](#formatRow-int-com.aspose.cells.Style-) | قم بتنسيق بيانات الصف في منطقة PivotTable |
| [getAllowMultipleFiltersPerField()](#getAllowMultipleFiltersPerField--) | يحدد قيمة منطقية تشير إلى ما إذا كان بإمكان حقول PivotTable أن تحتوي على فلاتر متعددة مضبوطة عليها. |
| [getAltTextDescription()](#getAltTextDescription--) | يحصل على وصف النص البديل. |
| [getAltTextTitle()](#getAltTextTitle--) | يحصل على عنوان النص البديل. |
| [getAutoFormatType()](#getAutoFormatType--) | يحصل على نوع التنسيق التلقائي لـ PivotTable. |
| [getAutofitColumnWidthOnUpdate()](#getAutofitColumnWidthOnUpdate--) | يشير إلى ما إذا كان يجب ضبط عرض العمود تلقائيًا عند التحديث. |
| [getBaseFields()](#getBaseFields--) | يعيد جميع حقول المحور الأساسية في PivotTable. |
| [getButtonArea(int axisType)](#getButtonArea-int-) | يحصل على المنطقة التي تحتوي على زر الحقل. |
| [getCellByDisplayName(String displayName)](#getCellByDisplayName-java.lang.String-) | يحصل على كائن [Cell](../../com.aspose.cells/cell) حسب اسم العرض لـ PivotField. |
| [getChildren()](#getChildren--) | يحصل على جداول Pivot Children التي تستخدم بيانات هذا PivotTable كمصدر للبيانات. |
| [getClass()](#getClass--) |  |
| [getColumnFields()](#getColumnFields--) | يعيد كائن PivotFields الذي يُظهر حاليًا كحقول عمود. |
| [getColumnGrand()](#getColumnGrand--) | يشير إلى ما إذا كان تقرير PivotTable يعرض الإجماليات العامة للأعمدة. |
| [getColumnHeaderCaption()](#getColumnHeaderCaption--) | يحصل على التسمية المخصصة لرأس العمود في PivotTable. |
| [getColumnRange()](#getColumnRange--) | يعيد كائن CellArea الذي يمثل النطاق الذي يحتوي على منطقة العمود في تقرير PivotTable. |
| [getConditionalFormats()](#getConditionalFormats--) | يحصل على التنسيقات الشرطية لجدول pivot. |
| [getCustomListSort()](#getCustomListSort--) | يشير إلى ما إذا كان يجب اعتبار القائمة المخصصة المدمجة عند فرز البيانات |
| [getDataBodyRange()](#getDataBodyRange--) | يعيد كائن [CellArea](../../com.aspose.cells/cellarea) الذي يمثل النطاق الذي يحتوي على منطقة البيانات في القائمة بين صف الرأس وصف الإدراج. |
| [getDataField()](#getDataField--) | يحصل على كائن [PivotField](../../com.aspose.cells/pivotfield) الذي يمثل جميع حقول البيانات في PivotTable. |
| [getDataFieldHeaderName()](#getDataFieldHeaderName--) | يحصل على اسم رأس حقل منطقة القيمة في PivotTable. |
| [getDataFields()](#getDataFields--) | يحصل على [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) التي تمثل جميع حقول البيانات في PivotTable. |
| [getDataSource()](#getDataSource--) | يحصل على مصدر البيانات ل PivotTable. |
| [getDependentPivotTables()](#getDependentPivotTables--) | يحصل على جميع [PivotTable](../../com.aspose.cells/pivottable)s التي تستخدم هذا PivotTable كمصدر بيانات لها. |
| [getDisplayErrorString()](#getDisplayErrorString--) | يشير إلى ما إذا كان تقرير PivotTable يعرض سلسلة مخصصة في الخلايا التي تحتوي على أخطاء. |
| [getDisplayImmediateItems()](#getDisplayImmediateItems--) | يشير إلى ما إذا كانت العناصر في مناطق الصف والعمود مرئية عندما تكون منطقة البيانات في PivotTable فارغة. |
| [getDisplayNullString()](#getDisplayNullString--) | يشير إلى ما إذا كان تقرير PivotTable يعرض سلسلة مخصصة إذا كانت القيمة فارغة. |
| [getEnableDataValueEditing()](#getEnableDataValueEditing--) | يحدد قيمة منطقية تشير إلى ما إذا كان يُسمح للمستخدم بتحرير الخلايا في منطقة البيانات من pivottable. |
| [getEnableDrilldown()](#getEnableDrilldown--) | يشير إلى ما إذا كان التفصيل (drilldown) مفعلاً. |
| [getEnableFieldDialog()](#getEnableFieldDialog--) | يشير إلى ما إذا كان مربع حوار حقل PivotTable متاحًا عندما ينقر المستخدم مزدوجًا على حقل PivotTable. |
| [getEnableFieldList()](#getEnableFieldList--) | يشير إلى ما إذا كانت قائمة الحقول لـ PivotTable متاحة في عرض Excel. |
| [getEnableWizard()](#getEnableWizard--) | يشير إلى ما إذا كان معالج PivotTable متاحًا. |
| [getErrorString()](#getErrorString--) | يحصل على السلسلة المعروضة في الخلايا التي تحتوي على أخطاء عندما تكون خاصية DisplayErrorString صحيحة. القيمة الافتراضية هي سلسلة فارغة. |
| [getExternalConnectionDataSource()](#getExternalConnectionDataSource--) | يحصل على مصدر بيانات الاتصال الخارجي. |
| [getFieldListSortAscending()](#getFieldListSortAscending--) | يشير إلى ما إذا كانت الحقول في PivotTable مرتبة بترتيب غير افتراضي في قائمة الحقول. |
| [getFields(int fieldType)](#getFields-int-) | يحصل على قائمة الحقول المحورية المحددة حسب المنطقة. |
| [getFilterArea()](#getFilterArea--) | يحصل على منطقة منطقة التصفية. |
| [getGrandTotalName()](#getGrandTotalName--) | يرجع التسمية التي تُعرض في عنوان العمود أو الصف الإجمالي الكلي. |
| [getHorizontalBreaks()](#getHorizontalBreaks--) | يحصل على قائمة فهارس صفوف جدول المحور لفواصل الصفحات الأفقية. |
| [getHorizontalPageBreaks()](#getHorizontalPageBreaks--) | يحصل على فواصل الصفحات الأفقية لهذا جدول المحور. |
| [getIndent()](#getIndent--) | يحدد زيادة المسافة البادئة للمحور المدمج ويمكن استخدامها لتعيين تخطيط التقرير إلى الشكل المدمج. |
| [getItemPrintTitles()](#getItemPrintTitles--) | يشير إلى ما إذا كان يجب تكرار أسماء PivotItem في أعلى كل صفحة مطبوعة. |
| [getManualUpdate()](#getManualUpdate--) | يشير إلى ما إذا كان تقرير PivotTable يُعاد حسابه فقط عند طلب المستخدم. |
| [getMergeLabels()](#getMergeLabels--) | يحصل على ما إذا كان يجب دمج تسميات حقول الصف/العمود التي تمتد عبر خلايا متعددة. |
| [getMissingItemsLimit()](#getMissingItemsLimit--) | يحدد قيمة منطقية تشير إلى ما إذا كان بإمكان حقول PivotTable أن تحتوي على فلاتر متعددة مضبوطة عليها. |
| [getName()](#getName--) | يحصل على اسم PivotTable |
| [getNamesOfSourceDataConnections()](#getNamesOfSourceDataConnections--) | يحصل على أسماء اتصالات مصدر البيانات الخارجية. |
| [getNullString()](#getNullString--) | يحصل على السلسلة المعروضة في الخلايا التي تحتوي على قيم فارغة عندما تكون الخاصية DisplayNullString صحيحة. القيمة الافتراضية هي سلسلة فارغة. |
| [getPageFieldOrder()](#getPageFieldOrder--) | يحصل على الترتيب الذي تُضاف به حقول الصفحة إلى تخطيط تقرير PivotTable. |
| [getPageFieldWrapCount()](#getPageFieldWrapCount--) | يحصل على عدد حقول الصفحة في كل عمود أو صف في تقرير PivotTable. |
| [getPageFields()](#getPageFields--) | يعيد مجموعة [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) التي تُظهر حاليًا كحقول صفحة. |
| [getPivotCache()](#getPivotCache--) | يحصل على مصدر البيانات. |
| [getPivotFilters()](#getPivotFilters--) | يعيد جميع الفلاتر في جدول PivotTable. |
| [getPivotFormatConditions()](#getPivotFormatConditions--) | يحصل على شروط التنسيق (Format Conditions) لجدول PivotTable. |
| [getPivotFormats()](#getPivotFormats--) | يحصل على جميع تنسيقات الخلايا المطبقة على جدول PivotTable هذا. |
| [getPivotTableStyle()](#getPivotTableStyle--) | يحصل على إعدادات [TableStyle](../../com.aspose.cells/tablestyle) لهذا جدول PivotTable. |
| [getPivotTableStyleName()](#getPivotTableStyleName--) | يحصل على اسم النمط لجدول PivotTable. |
| [getPivotTableStyleType()](#getPivotTableStyleType--) | يحصل على نمط جدول PivotTable المدمج. |
| [getPivotTablesWithSamePivotCache()](#getPivotTablesWithSamePivotCache--) | يحصل على جميع جداول PivotTable التي تشترك في نفس ذاكرة التخزين المؤقت PivotCache. |
| [getPreserveCellFormattingOnUpdate()](#getPreserveCellFormattingOnUpdate--) | يشير إلى ما إذا كان يجب الحفاظ على تنسيق الخلايا ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) عند تحديث أو إعادة حساب جدول PivotTable. |
| [getPreserveFormatting()](#getPreserveFormatting--) | يشير إلى ما إذا كان تنسيق الخلايا ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) محفوظًا عند تحديث أو إعادة حساب جدول PivotTable. |
| [getPrintDrill()](#getPrintDrill--) | يحدد قيمة منطقية تشير إلى ما إذا كان يجب طباعة مؤشرات الحفر. |
| [getPrintTitles()](#getPrintTitles--) | يشير إلى ما إذا كانت عناوين الطباعة للورقة تُضبط بناءً على تقرير PivotTable. |
| [getRefreshDataOnOpeningFile()](#getRefreshDataOnOpeningFile--) | يشير إلى ما إذا كان يجب تحديث البيانات عند فتح الملف. |
| [getRefreshDate()](#getRefreshDate--) | يحصل على تاريخ ووقت آخر مرة تم فيها تحديث جدول PivotTable. |
| [getRefreshedByWho()](#getRefreshedByWho--) | يحصل على اسم آخر مستخدم قام بتحديث جدول PivotTable هذا. |
| [getRepeatItemsOnEachPrintedPage()](#getRepeatItemsOnEachPrintedPage--) | يشير إلى ما إذا كانت تسميات عنصر Pivot في منطقة الصف تُكرر في كل صفحة مطبوعة لحقول Pivot في الشكل الجدولي. |
| [getRowFields()](#getRowFields--) | يعيد مجموعة [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) التي تُظهر حاليًا كحقول صف. |
| [getRowGrand()](#getRowGrand--) | يشير إلى ما إذا كان يجب إظهار الإجماليات العامة للصفوف في جدول PivotTable هذا. |
| [getRowHeaderCaption()](#getRowHeaderCaption--) | يحصل على التسمية المخصصة لرأس الصف في جدول PivotTable هذا. |
| [getRowRange()](#getRowRange--) | يعيد كائن CellArea الذي يمثل النطاق الذي يحتوي على منطقة الصف في تقرير PivotTable. |
| [getSaveData()](#getSaveData--) | يشير إلى ما إذا كانت البيانات لتقرير PivotTable محفوظة مع المصنف. |
| [getShowColumnGrandTotals()](#getShowColumnGrandTotals--) | يشير إلى ما إذا كان يجب عرض الإجماليات العامة للأعمدة في جدول PivotTable هذا. |
| [getShowDataTips()](#getShowDataTips--) | يشير إلى ما إذا كان يجب عرض تلميحات الأدوات لخلايا بيانات PivotTable. |
| [getShowDrill()](#getShowDrill--) | يحصل على ما إذا كان يتم عرض أزرار التوسيع/الطي. |
| [getShowEmptyCol()](#getShowEmptyCol--) | يشير إلى ما إذا كان يجب تضمين الأعمدة الفارغة في الجدول |
| [getShowEmptyRow()](#getShowEmptyRow--) | يشير إلى ما إذا كان يجب تضمين الصفوف الفارغة في الجدول. |
| [getShowHeaders()](#getShowHeaders--) | ما إذا كان يجب عرض عناوين حقول البيانات وعناوين حقول Pivot على محور الصفوف ومحور الأعمدة في عرض PivotTable. |
| [getShowMemberPropertyTips()](#getShowMemberPropertyTips--) | يحدد قيمة منطقية تشير إلى ما إذا كان يجب حذف معلومات خصائص العضو من تلميحات أدوات PivotTable. |
| [getShowPivotStyleColumnHeader()](#getShowPivotStyleColumnHeader--) | يشير إلى ما إذا كان يجب تطبيق النمط على رأس العمود في جدول Pivot. |
| [getShowPivotStyleColumnStripes()](#getShowPivotStyleColumnStripes--) | يشير إلى ما إذا كان تنسيق الشرائط يُطبق على العمود. |
| [getShowPivotStyleLastColumn()](#getShowPivotStyleLastColumn--) | يشير إلى ما إذا كان تنسيق العمود يُطبق. |
| [getShowPivotStyleRowHeader()](#getShowPivotStyleRowHeader--) | يشير إلى ما إذا كان يجب تطبيق النمط على رأس الصف في جدول Pivot. |
| [getShowPivotStyleRowStripes()](#getShowPivotStyleRowStripes--) | يشير إلى ما إذا كان تنسيق الشرائط للصف يُطبق. |
| [getShowRowGrandTotals()](#getShowRowGrandTotals--) | يشير إلى ما إذا كان يجب عرض الإجماليات العامة للصفوف في جدول Pivot. |
| [getShowRowHeaderCaption()](#getShowRowHeaderCaption--) | يشير إلى ما إذا كان عنوان رأس الصف يُظهر في تقرير PivotTable يشير إلى ما إذا كان يتم عرض عناوين الحقول و قوائم الفلاتر المنسدلة. |
| [getShowValuesRow()](#getShowValuesRow--) | يشير إلى ما إذا كان يتم عرض صف القيم. |
| [getSource()](#getSource--) | احصل على مصدر البيانات لهذا جدول Pivot. |
| [getSource(boolean isOriginal)](#getSource-boolean-) | احصل على مصدر البيانات لهذا جدول Pivot. |
| [getSourceDataConnections()](#getSourceDataConnections--) | يحصل على مصادر بيانات الاتصال الخارجي. |
| [getSourceType()](#getSourceType--) | يحصل على نوع مصدر البيانات لجدول Pivot. |
| [getSubtotalHiddenPageItems()](#getSubtotalHiddenPageItems--) | يشير إلى ما إذا كانت عناصر حقل الصفحة المخفية في تقرير PivotTable مدرجة في المجاميع الفرعية للصفوف والأعمدة، ومجاميع الكتل، والإجماليات العامة. |
| [getTableRange1()](#getTableRange1--) | يرجع كائن CellArea يمثل النطاق الذي يحتوي على تقرير PivotTable بالكامل، لكنه لا يتضمن حقول الصفحة. |
| [getTableRange2()](#getTableRange2--) | يرجع كائن CellArea يمثل النطاق الذي يحتوي على تقرير PivotTable بالكامل، ويتضمن حقول الصفحة. |
| [getTag()](#getTag--) | يحصل على سلسلة معرفة من قبل المستخدم مرتبطة بعرض PivotTable هذا. |
| [getTopRightArea()](#getTopRightArea--) | يمثل المنطقة الفارغة في أعلى يمين PivotTable (أعلى يسار للأوراق RTL). |
| [getValuesField()](#getValuesField--) | يحصل على كائن [PivotField](../../com.aspose.cells/pivotfield) الذي يمثل جميع حقول البيانات في PivotTable. |
| [hasBlankRows()](#hasBlankRows--) | يشير إلى ما إذا كان يجب إضافة صفوف فارغة. |
| [hashCode()](#hashCode--) |  |
| [isAutoFormat()](#isAutoFormat--) | يشير إلى ما إذا كان تقرير PivotTable يتم تنسيقه تلقائيًا. |
| [isExcel2003Compatible()](#isExcel2003Compatible--) | يحدد ما إذا كان PivotTable متوافقًا مع Excel2003 عند تحديث PivotTable، إذا كان صحيحًا، يجب أن يكون النص أقل من أو يساوي 255 حرفًا، لذا إذا كان النص أطول من 255 حرفًا، سيتم قطعه. إذا كان خاطئًا، لن يخضع النص للقيود المذكورة أعلاه. |
| [isGridDropZones()](#isGridDropZones--) | يشير إلى ما إذا كان تقرير PivotTable يعرض تخطيط PivotTable الكلاسيكي. |
| [isMultipleFieldFilters()](#isMultipleFieldFilters--) | يحدد قيمة منطقية تشير إلى ما إذا كان بإمكان حقول PivotTable أن تحتوي على فلاتر متعددة مضبوطة عليها. |
| [isSelected()](#isSelected--) | يشير إلى ما إذا تم تحديد هذا الـ PivotTable. |
| [move(int row, int column)](#move-int-int-) | ينقل الـ PivotTable إلى موقع مختلف في ورقة العمل. |
| [move(String destCellName)](#move-java.lang.String-) | ينقل الـ PivotTable إلى موقع مختلف في ورقة العمل. |
| [moveItem(int region, String[] nodes, boolean absolute, int offset)](#moveItem-int-java.lang.String---boolean-int-) | نقل عنصر واحد للأعلى أو للأسفل. |
| [moveTo(int row, int column)](#moveTo-int-int-) | ينقل الـ PivotTable إلى موقع مختلف في ورقة العمل. |
| [moveTo(int sheetIndex, int row, int column)](#moveTo-int-int-int-) | ينقل الـ PivotTable إلى موقع مختلف في ورقة العمل. |
| [moveTo(String destCellName)](#moveTo-java.lang.String-) | ينقل الـ PivotTable إلى موقع مختلف في ورقة العمل. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | تحديث [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) من مصدر البيانات وحساب البيانات والنمط لعرض الـ pivot. |
| [refresh(PivotTableRefreshOption option)](#refresh-com.aspose.cells.PivotTableRefreshOption-) | تحديث [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) من مصدر البيانات وحساب البيانات والنمط لعرض الـ pivot. |
| [refreshData()](#refreshData--) | يقوم بتحديث البيانات من مصدر البيانات إلى ذاكرة التخزين المؤقت للـ pivot. |
| [refreshData(PivotTableRefreshOption option)](#refreshData-com.aspose.cells.PivotTableRefreshOption-) | يقوم بتحديث بيانات وإعدادات الـ pivottable من مصدر البيانات مع الخيارات. |
| [removeField(int fieldType, PivotField pivotField)](#removeField-int-com.aspose.cells.PivotField-) | إزالة الحقل من منطقة الحقل المحددة |
| [removeField(int fieldType, int baseFieldIndex)](#removeField-int-int-) | يزيل حقلًا من منطقة الـ pivot المحددة. |
| [removeField(int fieldType, String fieldName)](#removeField-int-java.lang.String-) | يزيل حقلًا من منطقة الحقل المحددة. |
| [selectArea(CellArea ca)](#selectArea-com.aspose.cells.CellArea-) | حدد منطقة من عرض جدول الـ pivot. |
| [setAllowMultipleFiltersPerField(boolean value)](#setAllowMultipleFiltersPerField-boolean-) | يحدد قيمة منطقية تشير إلى ما إذا كان بإمكان حقول PivotTable أن تحتوي على فلاتر متعددة مضبوطة عليها. |
| [setAltTextDescription(String value)](#setAltTextDescription-java.lang.String-) | يحصل على وصف النص البديل. |
| [setAltTextTitle(String value)](#setAltTextTitle-java.lang.String-) | يضبط عنوان النص البديل. |
| [setAutoFormat(boolean value)](#setAutoFormat-boolean-) | يشير إلى ما إذا كان تقرير PivotTable يتم تنسيقه تلقائيًا. |
| [setAutoFormatType(int value)](#setAutoFormatType-int-) | يضبط نوع التنسيق التلقائي للـ PivotTable. |
| [setAutofitColumnWidthOnUpdate(boolean value)](#setAutofitColumnWidthOnUpdate-boolean-) | يشير إلى ما إذا كان يجب ضبط عرض العمود تلقائيًا عند التحديث. |
| [setColumnGrand(boolean value)](#setColumnGrand-boolean-) | يشير إلى ما إذا كان تقرير PivotTable يعرض الإجماليات العامة للأعمدة. |
| [setColumnHeaderCaption(String value)](#setColumnHeaderCaption-java.lang.String-) | يضبط التسمية المخصصة لرأس العمود في الـ PivotTable. |
| [setCustomListSort(boolean value)](#setCustomListSort-boolean-) | يشير إلى ما إذا كان يجب اعتبار القائمة المخصصة المدمجة عند فرز البيانات |
| [setDataFieldHeaderName(String value)](#setDataFieldHeaderName-java.lang.String-) | يضبط اسم رأس حقل منطقة القيم في الـ PivotTable. |
| [setDataSource(String[] value)](#setDataSource-java.lang.String---) | يضبط مصدر البيانات لجدول الـ pivot. |
| [setDisplayErrorString(boolean value)](#setDisplayErrorString-boolean-) | يشير إلى ما إذا كان تقرير PivotTable يعرض سلسلة مخصصة في الخلايا التي تحتوي على أخطاء. |
| [setDisplayImmediateItems(boolean value)](#setDisplayImmediateItems-boolean-) | يشير إلى ما إذا كانت العناصر في مناطق الصف والعمود مرئية عندما تكون منطقة البيانات في PivotTable فارغة. |
| [setDisplayNullString(boolean value)](#setDisplayNullString-boolean-) | يشير إلى ما إذا كان تقرير PivotTable يعرض سلسلة مخصصة إذا كانت القيمة فارغة. |
| [setEnableDataValueEditing(boolean value)](#setEnableDataValueEditing-boolean-) | يحدد قيمة منطقية تشير إلى ما إذا كان يُسمح للمستخدم بتحرير الخلايا في منطقة البيانات من pivottable. |
| [setEnableDrilldown(boolean value)](#setEnableDrilldown-boolean-) | يشير إلى ما إذا كان التفصيل (drilldown) مفعلاً. |
| [setEnableFieldDialog(boolean value)](#setEnableFieldDialog-boolean-) | يشير إلى ما إذا كان مربع حوار حقل PivotTable متاحًا عندما ينقر المستخدم مزدوجًا على حقل PivotTable. |
| [setEnableFieldList(boolean value)](#setEnableFieldList-boolean-) | يشير إلى ما إذا كانت قائمة الحقول لـ PivotTable متاحة في عرض Excel. |
| [setEnableWizard(boolean value)](#setEnableWizard-boolean-) | يشير إلى ما إذا كان معالج PivotTable متاحًا. |
| [setErrorString(String value)](#setErrorString-java.lang.String-) | يحصل على السلسلة المعروضة في الخلايا التي تحتوي على أخطاء عندما تكون خاصية DisplayErrorString صحيحة. القيمة الافتراضية هي سلسلة فارغة. |
| [setExcel2003Compatible(boolean value)](#setExcel2003Compatible-boolean-) | يحدد ما إذا كان PivotTable متوافقًا مع Excel2003 عند تحديث PivotTable، إذا كان صحيحًا، يجب أن يكون النص أقل من أو يساوي 255 حرفًا، لذا إذا كان النص أطول من 255 حرفًا، سيتم قطعه. إذا كان خاطئًا، لن يخضع النص للقيود المذكورة أعلاه. |
| [setFieldListSortAscending(boolean value)](#setFieldListSortAscending-boolean-) | يشير إلى ما إذا كانت الحقول في PivotTable مرتبة بترتيب غير افتراضي في قائمة الحقول. |
| [setGrandTotalName(String value)](#setGrandTotalName-java.lang.String-) | يرجع التسمية التي تُعرض في عنوان العمود أو الصف الإجمالي الكلي. |
| [setGridDropZones(boolean value)](#setGridDropZones-boolean-) | يشير إلى ما إذا كان تقرير PivotTable يعرض تخطيط PivotTable الكلاسيكي. |
| [setHasBlankRows(boolean value)](#setHasBlankRows-boolean-) | يشير إلى ما إذا كان يجب إضافة صفوف فارغة. |
| [setIndent(int value)](#setIndent-int-) | يحدد زيادة المسافة البادئة للمحور المدمج ويمكن استخدامها لتعيين تخطيط التقرير إلى الشكل المدمج. |
| [setItemPrintTitles(boolean value)](#setItemPrintTitles-boolean-) | يشير إلى ما إذا كان يجب تكرار أسماء PivotItem في أعلى كل صفحة مطبوعة. |
| [setManualUpdate(boolean value)](#setManualUpdate-boolean-) | يشير إلى ما إذا كان تقرير PivotTable يُعاد حسابه فقط عند طلب المستخدم. |
| [setMergeLabels(boolean value)](#setMergeLabels-boolean-) | يضبط ما إذا كان سيتم دمج تسميات الحقول الصفية/العمودية التي تمتد عبر عدة خلايا. |
| [setMissingItemsLimit(int value)](#setMissingItemsLimit-int-) | يحدد قيمة منطقية تشير إلى ما إذا كان بإمكان حقول PivotTable أن تحتوي على فلاتر متعددة مضبوطة عليها. |
| [setMultipleFieldFilters(boolean value)](#setMultipleFieldFilters-boolean-) | يحدد قيمة منطقية تشير إلى ما إذا كان بإمكان حقول PivotTable أن تحتوي على فلاتر متعددة مضبوطة عليها. |
| [setName(String value)](#setName-java.lang.String-) | يحصل على اسم PivotTable |
| [setNullString(String value)](#setNullString-java.lang.String-) | يحصل على السلسلة المعروضة في الخلايا التي تحتوي على قيم فارغة عندما تكون الخاصية DisplayNullString صحيحة. القيمة الافتراضية هي سلسلة فارغة. |
| [setPageFieldOrder(int value)](#setPageFieldOrder-int-) | يضبط الترتيب الذي تُضاف به حقول الصفحة إلى تخطيط تقرير الـ PivotTable. |
| [setPageFieldWrapCount(int value)](#setPageFieldWrapCount-int-) | يحصل على عدد حقول الصفحة في كل عمود أو صف في تقرير PivotTable. |
| [setPivotTableStyle(TableStyle value)](#setPivotTableStyle-com.aspose.cells.TableStyle-) | يحصل على إعدادات [TableStyle](../../com.aspose.cells/tablestyle) لهذا جدول PivotTable. |
| [setPivotTableStyleName(String value)](#setPivotTableStyleName-java.lang.String-) | يضبط اسم النمط لجدول الـ pivot. |
| [setPivotTableStyleType(int value)](#setPivotTableStyleType-int-) | يضبط نمط جدول الـ pivot المدمج. |
| [setPreserveCellFormattingOnUpdate(boolean value)](#setPreserveCellFormattingOnUpdate-boolean-) | يشير إلى ما إذا كان يجب الحفاظ على تنسيق الخلايا ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) عند تحديث أو إعادة حساب جدول PivotTable. |
| [setPreserveFormatting(boolean value)](#setPreserveFormatting-boolean-) | يشير إلى ما إذا كان تنسيق الخلايا ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) محفوظًا عند تحديث أو إعادة حساب جدول PivotTable. |
| [setPrintDrill(boolean value)](#setPrintDrill-boolean-) | يحدد قيمة منطقية تشير إلى ما إذا كان يجب طباعة مؤشرات الحفر. |
| [setPrintTitles(boolean value)](#setPrintTitles-boolean-) | يشير إلى ما إذا كانت عناوين الطباعة للورقة تُضبط بناءً على تقرير PivotTable. |
| [setRefreshDataOnOpeningFile(boolean value)](#setRefreshDataOnOpeningFile-boolean-) | يشير إلى ما إذا كان يجب تحديث البيانات عند فتح الملف. |
| [setRepeatItemsOnEachPrintedPage(boolean value)](#setRepeatItemsOnEachPrintedPage-boolean-) | يشير إلى ما إذا كانت تسميات عنصر Pivot في منطقة الصف تُكرر في كل صفحة مطبوعة لحقول Pivot في الشكل الجدولي. |
| [setRowGrand(boolean value)](#setRowGrand-boolean-) | يشير إلى ما إذا كان يجب إظهار الإجماليات العامة للصفوف في جدول PivotTable هذا. |
| [setRowHeaderCaption(String value)](#setRowHeaderCaption-java.lang.String-) | يضبط التسمية المخصصة لرأس الصف في هذا الـ PivotTable. |
| [setSaveData(boolean value)](#setSaveData-boolean-) | يشير إلى ما إذا كانت البيانات لتقرير PivotTable محفوظة مع المصنف. |
| [setSelected(boolean value)](#setSelected-boolean-) | يشير إلى ما إذا تم تحديد هذا الـ PivotTable. |
| [setShowColumnGrandTotals(boolean value)](#setShowColumnGrandTotals-boolean-) | يشير إلى ما إذا كان يجب عرض الإجماليات العامة للأعمدة في جدول PivotTable هذا. |
| [setShowDataTips(boolean value)](#setShowDataTips-boolean-) | يشير إلى ما إذا كان يجب عرض تلميحات الأدوات لخلايا بيانات PivotTable. |
| [setShowDrill(boolean value)](#setShowDrill-boolean-) | يضبط ما إذا كان سيتم عرض أزرار التوسيع/الطي. |
| [setShowEmptyCol(boolean value)](#setShowEmptyCol-boolean-) | يشير إلى ما إذا كان يجب تضمين الأعمدة الفارغة في الجدول |
| [setShowEmptyRow(boolean value)](#setShowEmptyRow-boolean-) | يشير إلى ما إذا كان يجب تضمين الصفوف الفارغة في الجدول. |
| [setShowHeaders(boolean value)](#setShowHeaders-boolean-) | ما إذا كان يجب عرض عناوين حقول البيانات وعناوين حقول Pivot على محور الصفوف ومحور الأعمدة في عرض PivotTable. |
| [setShowMemberPropertyTips(boolean value)](#setShowMemberPropertyTips-boolean-) | يحدد قيمة منطقية تشير إلى ما إذا كان يجب حذف معلومات خصائص العضو من تلميحات أدوات PivotTable. |
| [setShowPivotStyleColumnHeader(boolean value)](#setShowPivotStyleColumnHeader-boolean-) | يشير إلى ما إذا كان يجب تطبيق النمط على رأس العمود في جدول Pivot. |
| [setShowPivotStyleColumnStripes(boolean value)](#setShowPivotStyleColumnStripes-boolean-) | يشير إلى ما إذا كان تنسيق الشرائط يُطبق على العمود. |
| [setShowPivotStyleLastColumn(boolean value)](#setShowPivotStyleLastColumn-boolean-) | يشير إلى ما إذا كان تنسيق العمود يُطبق. |
| [setShowPivotStyleRowHeader(boolean value)](#setShowPivotStyleRowHeader-boolean-) | يشير إلى ما إذا كان يجب تطبيق النمط على رأس الصف في جدول Pivot. |
| [setShowPivotStyleRowStripes(boolean value)](#setShowPivotStyleRowStripes-boolean-) | يشير إلى ما إذا كان تنسيق الشرائط للصف يُطبق. |
| [setShowRowGrandTotals(boolean value)](#setShowRowGrandTotals-boolean-) | يشير إلى ما إذا كان يجب عرض الإجماليات العامة للصفوف في جدول Pivot. |
| [setShowRowHeaderCaption(boolean value)](#setShowRowHeaderCaption-boolean-) | يشير إلى ما إذا كان عنوان رأس الصف يُظهر في تقرير PivotTable يشير إلى ما إذا كان يتم عرض عناوين الحقول و قوائم الفلاتر المنسدلة. |
| [setShowValuesRow(boolean value)](#setShowValuesRow-boolean-) | يشير إلى ما إذا كان يتم عرض صف القيم. |
| [setSubtotalHiddenPageItems(boolean value)](#setSubtotalHiddenPageItems-boolean-) | يشير إلى ما إذا كانت عناصر حقل الصفحة المخفية في تقرير PivotTable مدرجة في المجاميع الفرعية للصفوف والأعمدة، ومجاميع الكتل، والإجماليات العامة. |
| [setTag(String value)](#setTag-java.lang.String-) | يضبط سلسلة معرفة من قبل المستخدم مرتبطة بعرض الـ PivotTable هذا. |
| [showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn)](#showDetail-int-int-boolean-int-int-) | عرض تفاصيل عنصر واحد في منطقة البيانات إلى جدول جديد. |
| [showInCompactForm()](#showInCompactForm--) | يُنسق عرض PivotTable في الشكل المدمج. |
| [showInOutlineForm()](#showInOutlineForm--) | يُنسق PivotTable في الشكل المخطط. |
| [showInTabularForm()](#showInTabularForm--) | يُنسق PivotTable في الشكل الجدولي. |
| [showReportFilterPage(PivotField pageField)](#showReportFilterPage-com.aspose.cells.PivotField-) | عرض جميع صفحات مرشح التقرير وفقًا لـ PivotField، يجب أن يكون PivotField موجودًا في PageFields. |
| [showReportFilterPageByIndex(int posIndex)](#showReportFilterPageByIndex-int-) | عرض جميع صفحات مرشح التقرير وفقًا لمؤشر الموقع في PageFields. |
| [showReportFilterPageByName(String fieldName)](#showReportFilterPageByName-java.lang.String-) | عرض جميع صفحات مرشح التقرير وفقًا لاسم PivotField، يجب أن يكون PivotField موجودًا في PageFields. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCalculatedField(String name, String formula) {#addCalculatedField-java.lang.String-java.lang.String-}
```
public void addCalculatedField(String name, String formula)
```


يضيف حقلًا محسوبًا إلى حقل المحور ويسحبه إلى منطقة البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم الحقل المحسوب |
| formula | java.lang.String | صيغة الحقل المحسوب. |

### addCalculatedField(String name, String formula, boolean dragToDataArea) {#addCalculatedField-java.lang.String-java.lang.String-boolean-}
```
public void addCalculatedField(String name, String formula, boolean dragToDataArea)
```


يضيف حقلًا محسوبًا إلى حقل المحور.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم الحقل المحسوب |
| formula | java.lang.String | صيغة الحقل المحسوب. |
| dragToDataArea | boolean | True, اسحب هذا الحقل إلى منطقة البيانات فورًا |

### addFieldToArea(int fieldType, PivotField pivotField) {#addFieldToArea-int-com.aspose.cells.PivotField-}
```
public int addFieldToArea(int fieldType, PivotField pivotField)
```


يضيف الحقل إلى المنطقة المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). نوع منطقة الحقول. |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | الحقل في الحقول الأساسية. |

**Returns:**
int - موضع الحقل في الحقول المحددة.
### addFieldToArea(int fieldType, int baseFieldIndex) {#addFieldToArea-int-int-}
```
public int addFieldToArea(int fieldType, int baseFieldIndex)
```


يضيف الحقل إلى المنطقة المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). نوع منطقة الحقول. |
| baseFieldIndex | int | الفهرس في الحقول الأساسية. |

**Returns:**
int - موضع الحقل في الحقول المحددة.
### addFieldToArea(int fieldType, String fieldName) {#addFieldToArea-int-java.lang.String-}
```
public int addFieldToArea(int fieldType, String fieldName)
```


يضيف الحقل إلى المنطقة المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). نوع منطقة الحقول. |
| fieldName | java.lang.String | الاسم في الحقول الأساسية. |

**Returns:**
int - موضع الحقل في الحقول المحددة. إذا لم يكن هناك حقل يحمل هذا الاسم، أعد -1.
### calculateData() {#calculateData--}
```
public void calculateData()
```


يحسب بيانات جدول المحور إلى الخلايا.

**Remarks**

هذه الطريقة تحسب البيانات فقط باستخدام البيانات المخزنة مؤقتًا في [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--). لذلك إذا كنت تريد الحساب باستخدام مصدر البيانات الأحدث، يرجى استخدام طريقة [PivotCache.refresh()](../../com.aspose.cells/pivotcache\#refresh--) للحساب. إذا تم تغيير إعدادات جدول المحور فقط، فإن [calculateData()](../../com.aspose.cells/pivottable\#calculateData--) كافية.

### calculateData(PivotTableCalculateOption option) {#calculateData-com.aspose.cells.PivotTableCalculateOption-}
```
public PivotTable[] calculateData(PivotTableCalculateOption option)
```


يحسب جدول المحور مع الخيارات.

**Remarks**

إذا كان [PivotTableCalculateOption.getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\#getRefreshData--) صحيحًا، ستقوم هذه الطريقة بتحديث ذاكرة التخزين المؤقت للجدول المحوري من مصدر البيانات، ثم حساب جميع جداول المحور بناءً على نفس الذاكرة المؤقتة. وإلا، سيتم الحساب فقط باستخدام البيانات المخزنة مؤقتًا في الذاكرة المؤقتة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| option | [PivotTableCalculateOption](../../com.aspose.cells/pivottablecalculateoption) | الخيارات لحساب جدول المحور |

**Returns:**
com.aspose.cells.PivotTable[] - يُرجع جميع جداول المحور التي تم حسابها. إذا كان [PivotTableCalculateOption.getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\#getRefreshData--) صحيحًا، سيتم حساب جميع جداول المحور المستندة إلى نفس الذاكرة المؤقتة معًا.
### calculateRange() {#calculateRange--}
```
public void calculateRange()
```


يحسب نطاق جدول المحور.

**Remarks**

إذا لم يتم استدعاء هذه الطريقة، قد يكون نطاق جدول المحور غير صحيح.

### changeDataSource(String[] source) {#changeDataSource-java.lang.String---}
```
public void changeDataSource(String[] source)
```


تغيير مصدر البيانات لجدول المحور.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| المصدر | java.lang.String[] |  |

### clearAll() {#clearAll--}
```
public void clearAll()
```


إزالة جميع الحقول من المناطق.

### clearData() {#clearData--}
```
public void clearData()
```


مسح البيانات وتنسيق عرض جدول المحور.

**Remarks**

إذا لم يتم استدعاء هذه الطريقة قبل إضافة أو حذف PivotField، قد لا تكون بيانات PivotTable صحيحة

### clearFilters() {#clearFilters--}
```
public void clearFilters()
```


يمسح جميع عوامل التصفية لهذا جدول المحور.

### copyStyle(PivotTable pivotTable) {#copyStyle-com.aspose.cells.PivotTable-}
```
public void copyStyle(PivotTable pivotTable)
```


ينسخ النمط المسمى من جدول محوري آخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | جدول PivotTable المصدر. |

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
### exportViewToJson(PivotViewToJsonOptions options) {#exportViewToJson-com.aspose.cells.PivotViewToJsonOptions-}
```
public String exportViewToJson(PivotViewToJsonOptions options)
```


يصدّر عرض المحور كـ JSON.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| options | [PivotViewToJsonOptions](../../com.aspose.cells/pivotviewtojsonoptions) |  |

**Returns:**
java.lang.String -
### fields(int fieldType) {#fields-int-}
```
public PivotFieldCollection fields(int fieldType)
```


يحصل على الحقول المحددة حسب نوع الحقل.

**Remarks**

ملاحظة: هذه الطريقة أصبحت مهجورة الآن. بدلاً من ذلك، يرجى استخدام طريقة PivotField.GetFields(PivotFieldType). سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من مايو 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). نوع الحقل. |

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) - the specific field collection
### format(CellArea ca, Style style) {#format-com.aspose.cells.CellArea-com.aspose.cells.Style-}
```
public void format(CellArea ca, Style style)
```


يقوم بتنسيق المنطقة المحددة في PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | نطاق الخلايا. |
| style | [Style](../../com.aspose.cells/style) | النمط |

### format(PivotArea pivotArea, Style style) {#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-}
```
public void format(PivotArea pivotArea, Style style)
```


يقوم بتنسيق المنطقة المحددة في PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pivotArea | [PivotArea](../../com.aspose.cells/pivotarea) | منطقة عرض Pivot المحددة. |
| style | [Style](../../com.aspose.cells/style) | الإعداد المنسق. |

### format(int row, int column, Style style) {#format-int-int-com.aspose.cells.Style-}
```
public void format(int row, int column, Style style)
```


يقوم بتنسيق الخلية في منطقة PivotTable

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف للخلية |
| عمود | int | فهرس العمود للخلية |
| style | [Style](../../com.aspose.cells/style) | النمط المستخدم لتنسيق الخلية |

### formatAll(Style style) {#formatAll-com.aspose.cells.Style-}
```
public void formatAll(Style style)
```


قم بتنسيق جميع الخلايا في منطقة PivotTable

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | النمط المستخدم للتنسيق |

### formatRow(int row, Style style) {#formatRow-int-com.aspose.cells.Style-}
```
public void formatRow(int row, Style style)
```


قم بتنسيق بيانات الصف في منطقة PivotTable

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف لكائن Row |
| style | [Style](../../com.aspose.cells/style) | النمط المستخدم للتنسيق |

### getAllowMultipleFiltersPerField() {#getAllowMultipleFiltersPerField--}
```
public boolean getAllowMultipleFiltersPerField()
```


يحدد قيمة منطقية تشير إلى ما إذا كان بإمكان حقول PivotTable أن تحتوي على فلاتر متعددة مضبوطة عليها.

**Returns:**
boolean
### getAltTextDescription() {#getAltTextDescription--}
```
public String getAltTextDescription()
```


يحصل على وصف النص البديل.

**Returns:**
java.lang.String
### getAltTextTitle() {#getAltTextTitle--}
```
public String getAltTextTitle()
```


يحصل على عنوان النص البديل.

**Returns:**
java.lang.String
### getAutoFormatType() {#getAutoFormatType--}
```
public int getAutoFormatType()
```


يحصل على نوع التنسيق التلقائي لـ PivotTable.

انظر [PivotTableAutoFormatType](../../com.aspose.cells/pivottableautoformattype).

**Returns:**
int
### getAutofitColumnWidthOnUpdate() {#getAutofitColumnWidthOnUpdate--}
```
public boolean getAutofitColumnWidthOnUpdate()
```


يشير إلى ما إذا كان يجب ضبط عرض العمود تلقائيًا عند التحديث.

**Returns:**
boolean
### getBaseFields() {#getBaseFields--}
```
public PivotFieldCollection getBaseFields()
```


يعيد جميع حقول المحور الأساسية في PivotTable.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getButtonArea(int axisType) {#getButtonArea-int-}
```
public CellArea getButtonArea(int axisType)
```


يحصل على المنطقة التي تحتوي على زر الحقل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). نوع المنطقة. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - 
### getCellByDisplayName(String displayName) {#getCellByDisplayName-java.lang.String-}
```
public Cell getCellByDisplayName(String displayName)
```


يحصل على كائن [Cell](../../com.aspose.cells/cell) حسب اسم العرض لـ PivotField.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| displayName | java.lang.String | اسم العرض لـ PivotField |

**Returns:**
[Cell](../../com.aspose.cells/cell) - the Cell object
### getChildren() {#getChildren--}
```
public PivotTable[] getChildren()
```


يحصل على جداول Pivot Children التي تستخدم بيانات هذا PivotTable كمصدر للبيانات.

**Remarks**

ملاحظة: هذه الطريقة أصبحت مهجورة الآن. بدلاً من ذلك، يرجى استخدام طريقة PivotTable.GetDependentPivotTables(). سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من أبريل 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
com.aspose.cells.PivotTable[] - كائن مصفوفة PivotTable
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnFields() {#getColumnFields--}
```
public PivotFieldCollection getColumnFields()
```


يعيد كائن PivotFields الذي يُظهر حاليًا كحقول عمود.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getColumnGrand() {#getColumnGrand--}
```
public boolean getColumnGrand()
```


يشير إلى ما إذا كان تقرير PivotTable يعرض الإجماليات العامة للأعمدة.

**Remarks**

ملاحظة: هذه الخاصية أصبحت مهجورة الآن. بدلاً من ذلك، يرجى استخدام طريقة PivotTable.ShowColumnGrandTotals. سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من ديسمبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### getColumnHeaderCaption() {#getColumnHeaderCaption--}
```
public String getColumnHeaderCaption()
```


يحصل على التسمية المخصصة لرأس العمود في PivotTable.

**Returns:**
java.lang.String
### getColumnRange() {#getColumnRange--}
```
public CellArea getColumnRange()
```


يرجع كائن CellArea الذي يمثل النطاق الذي يحتوي على منطقة الأعمدة في تقرير PivotTable. للقراءة فقط.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getConditionalFormats() {#getConditionalFormats--}
```
public PivotConditionalFormatCollection getConditionalFormats()
```


يحصل على التنسيقات الشرطية لجدول pivot.

**Returns:**
[PivotConditionalFormatCollection](../../com.aspose.cells/pivotconditionalformatcollection)
### getCustomListSort() {#getCustomListSort--}
```
public boolean getCustomListSort()
```


يشير إلى ما إذا كان يجب اعتبار القائمة المخصصة المدمجة عند فرز البيانات

**Returns:**
boolean
### getDataBodyRange() {#getDataBodyRange--}
```
public CellArea getDataBodyRange()
```


يرجع كائن [CellArea](../../com.aspose.cells/cellarea) الذي يمثل النطاق الذي يحتوي على منطقة البيانات في القائمة بين صف الرأس وصف الإدراج. للقراءة فقط.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getDataField() {#getDataField--}
```
public PivotField getDataField()
```


يحصل على كائن [PivotField](../../com.aspose.cells/pivotfield) الذي يمثل جميع حقول البيانات في PivotTable. للقراءة فقط. يتم إنشاؤه فقط عندما يكون هناك حقلان بيانات أو أكثر في منطقة البيانات. بشكل افتراضي يكون في منطقة الصف. يمكنك سحبه إلى منطقة الصف/العمود باستخدام طريقة PivotTable.AddFieldToArea().

**Remarks**

ملاحظة: هذه الطريقة أصبحت مهجورة الآن. بدلاً من ذلك، يرجى استخدام خاصية PivotTable.ValuesField. سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من أكتوبر 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
### getDataFieldHeaderName() {#getDataFieldHeaderName--}
```
public String getDataFieldHeaderName()
```


يحصل على اسم رأس حقل منطقة القيمة في PivotTable.

**Returns:**
java.lang.String
### getDataFields() {#getDataFields--}
```
public PivotFieldCollection getDataFields()
```


يحصل على [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) التي تمثل جميع حقول البيانات في PivotTable.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getDataSource() {#getDataSource--}
```
public String[] getDataSource()
```


يحصل على مصدر البيانات ل PivotTable.

**Returns:**
java.lang.String[]
### getDependentPivotTables() {#getDependentPivotTables--}
```
public PivotTable[] getDependentPivotTables()
```


يحصل على جميع [PivotTable](../../com.aspose.cells/pivottable)s التي تستخدم هذا PivotTable كمصدر بيانات لها.

**Remarks**

نظرًا لأن جداول Pivot قد تعتمد على بيانات بعضها البعض، يجب تحديثها بالترتيب الصحيح لضمان اتساق البيانات.

**Returns:**
com.aspose.cells.PivotTable[] -
### getDisplayErrorString() {#getDisplayErrorString--}
```
public boolean getDisplayErrorString()
```


يشير إلى ما إذا كان تقرير PivotTable يعرض سلسلة مخصصة في الخلايا التي تحتوي على أخطاء.

**Returns:**
boolean
### getDisplayImmediateItems() {#getDisplayImmediateItems--}
```
public boolean getDisplayImmediateItems()
```


يشير إلى ما إذا كانت العناصر في مناطق الصف والعمود مرئية عندما تكون منطقة البيانات في PivotTable فارغة. القيمة الافتراضية هي true.

**Returns:**
boolean
### getDisplayNullString() {#getDisplayNullString--}
```
public boolean getDisplayNullString()
```


يشير إلى ما إذا كان تقرير PivotTable يعرض سلسلة مخصصة إذا كانت القيمة فارغة.

**Returns:**
boolean
### getEnableDataValueEditing() {#getEnableDataValueEditing--}
```
public boolean getEnableDataValueEditing()
```


يحدد قيمة منطقية تشير إلى ما إذا كان يُسمح للمستخدم بتحرير الخلايا في منطقة البيانات من pivottable. القيمة الافتراضية هي false.

**Returns:**
boolean
### getEnableDrilldown() {#getEnableDrilldown--}
```
public boolean getEnableDrilldown()
```


يشير إلى ما إذا كان التفصيل (drilldown) مفعلاً.

**Returns:**
boolean
### getEnableFieldDialog() {#getEnableFieldDialog--}
```
public boolean getEnableFieldDialog()
```


يشير إلى ما إذا كان مربع حوار حقل PivotTable متاحًا عندما ينقر المستخدم مزدوجًا على حقل PivotTable.

**Returns:**
boolean
### getEnableFieldList() {#getEnableFieldList--}
```
public boolean getEnableFieldList()
```


يشير إلى ما إذا كانت قائمة الحقول لـ PivotTable متاحة في عرض Excel.

**Returns:**
boolean
### getEnableWizard() {#getEnableWizard--}
```
public boolean getEnableWizard()
```


يشير إلى ما إذا كان معالج PivotTable متاحًا.

**Returns:**
boolean
### getErrorString() {#getErrorString--}
```
public String getErrorString()
```


يحصل على السلسلة المعروضة في الخلايا التي تحتوي على أخطاء عندما تكون خاصية DisplayErrorString صحيحة. القيمة الافتراضية هي سلسلة فارغة.

**Returns:**
java.lang.String
### getExternalConnectionDataSource() {#getExternalConnectionDataSource--}
```
public ExternalConnection getExternalConnectionDataSource()
```


يحصل على مصدر بيانات الاتصال الخارجي.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotTable.GetSourceDataConnections() method. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أكتوبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
[ExternalConnection](../../com.aspose.cells/externalconnection)
### getFieldListSortAscending() {#getFieldListSortAscending--}
```
public boolean getFieldListSortAscending()
```


يشير إلى ما إذا كانت الحقول في PivotTable مرتبة بترتيب غير افتراضي في قائمة الحقول.

**Returns:**
boolean
### getFields(int fieldType) {#getFields-int-}
```
public PivotFieldCollection getFields(int fieldType)
```


يحصل على قائمة الحقول المحورية المحددة حسب المنطقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). نوع المنطقة. |

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) - the specific pivot field collection
### getFilterArea() {#getFilterArea--}
```
public CellArea getFilterArea()
```


يحصل على منطقة منطقة التصفية.

**Remarks**

صالح فقط إذا كانت حقول التصفية موجودة. سيتم إرجاع منطقة فارغة إذا لم يحتوي هذا pivot table على حقول تصفية.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getGrandTotalName() {#getGrandTotalName--}
```
public String getGrandTotalName()
```


يرجع التسمية التي تُعرض في عمود أو رأس الصف الإجمالي. القيمة الافتراضية هي السلسلة "Grand Total".

**Returns:**
java.lang.String
### getHorizontalBreaks() {#getHorizontalBreaks--}
```
public ArrayList getHorizontalBreaks()
```


يحصل على قائمة فهارس صفوف جدول المحور لفواصل الصفحات الأفقية.

**Remarks**

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotTable.GetHorizontalPageBreaks() method. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ ديسمبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
java.util.ArrayList -
### getHorizontalPageBreaks() {#getHorizontalPageBreaks--}
```
public int[] getHorizontalPageBreaks()
```


يحصل على فواصل الصفحات الأفقية لهذا جدول المحور.

**Returns:**
int[] -
### getIndent() {#getIndent--}
```
public int getIndent()
```


يحدد زيادة المسافة البادئة للمحور المدمج ويمكن استخدامها لتعيين تخطيط التقرير إلى الشكل المدمج.

**Returns:**
int
### getItemPrintTitles() {#getItemPrintTitles--}
```
public boolean getItemPrintTitles()
```


يشير إلى ما إذا كان يجب تكرار أسماء PivotItem في أعلى كل صفحة مطبوعة.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام الخاصية PivotTable.RepeatItemsOnEachPrintedPage property. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أكتوبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### getManualUpdate() {#getManualUpdate--}
```
public boolean getManualUpdate()
```


يشير إلى ما إذا كان تقرير PivotTable يُعاد حسابه فقط عند طلب المستخدم.

**Returns:**
boolean
### getMergeLabels() {#getMergeLabels--}
```
public boolean getMergeLabels()
```


يحصل على ما إذا كان يجب دمج تسميات حقول الصف/العمود التي تمتد عبر خلايا متعددة.

**Returns:**
boolean
### getMissingItemsLimit() {#getMissingItemsLimit--}
```
public int getMissingItemsLimit()
```


يحدد قيمة منطقية تشير إلى ما إذا كان بإمكان حقول PivotTable أن تحتوي على فلاتر متعددة مضبوطة عليها.

انظر إلى [PivotMissingItemLimitType](../../com.aspose.cells/pivotmissingitemlimittype).

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام الخاصية PivotCache.MissingItemsLimit بدلاً من ذلك. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


يحصل على اسم PivotTable

**Returns:**
java.lang.String
### getNamesOfSourceDataConnections() {#getNamesOfSourceDataConnections--}
```
public String[] getNamesOfSourceDataConnections()
```


يحصل على أسماء اتصالات مصدر البيانات الخارجية.

**Returns:**
java.lang.String[]
### getNullString() {#getNullString--}
```
public String getNullString()
```


يحصل على السلسلة المعروضة في الخلايا التي تحتوي على قيم فارغة عندما تكون الخاصية DisplayNullString صحيحة. القيمة الافتراضية هي سلسلة فارغة.

**Returns:**
java.lang.String
### getPageFieldOrder() {#getPageFieldOrder--}
```
public int getPageFieldOrder()
```


يحصل على الترتيب الذي تُضاف به حقول الصفحة إلى تخطيط تقرير PivotTable.

انظر إلى [PrintOrderType](../../com.aspose.cells/printordertype).

**Returns:**
int
### getPageFieldWrapCount() {#getPageFieldWrapCount--}
```
public int getPageFieldWrapCount()
```


يحصل على عدد حقول الصفحة في كل عمود أو صف في تقرير PivotTable.

**Returns:**
int
### getPageFields() {#getPageFields--}
```
public PivotFieldCollection getPageFields()
```


يعيد مجموعة [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) التي تُظهر حاليًا كحقول صفحة.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getPivotCache() {#getPivotCache--}
```
public PivotCache getPivotCache()
```


يحصل على مصدر البيانات.

**Returns:**
[PivotCache](../../com.aspose.cells/pivotcache)
### getPivotFilters() {#getPivotFilters--}
```
public PivotFilterCollection getPivotFilters()
```


يعيد جميع الفلاتر في جدول PivotTable.

**Returns:**
[PivotFilterCollection](../../com.aspose.cells/pivotfiltercollection)
### getPivotFormatConditions() {#getPivotFormatConditions--}
```
public PivotFormatConditionCollection getPivotFormatConditions()
```


يحصل على شروط التنسيق (Format Conditions) لجدول PivotTable.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام الخاصية PivotTable.ConditionalFormats property. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
[PivotFormatConditionCollection](../../com.aspose.cells/pivotformatconditioncollection)
### getPivotFormats() {#getPivotFormats--}
```
public PivotTableFormatCollection getPivotFormats()
```


يحصل على جميع تنسيقات الخلايا المطبقة على جدول PivotTable هذا.

**Returns:**
[PivotTableFormatCollection](../../com.aspose.cells/pivottableformatcollection)
### getPivotTableStyle() {#getPivotTableStyle--}
```
public TableStyle getPivotTableStyle()
```


يحصل على إعدادات [TableStyle](../../com.aspose.cells/tablestyle) لهذا جدول PivotTable.

**Returns:**
[TableStyle](../../com.aspose.cells/tablestyle)
### getPivotTableStyleName() {#getPivotTableStyleName--}
```
public String getPivotTableStyleName()
```


يحصل على اسم النمط لجدول PivotTable.

**Returns:**
java.lang.String
### getPivotTableStyleType() {#getPivotTableStyleType--}
```
public int getPivotTableStyleType()
```


يحصل على نمط جدول PivotTable المدمج.

انظر إلى [PivotTableStyleType](../../com.aspose.cells/pivottablestyletype).

**Returns:**
int
### getPivotTablesWithSamePivotCache() {#getPivotTablesWithSamePivotCache--}
```
public PivotTable[] getPivotTablesWithSamePivotCache()
```


يحصل على جميع جداول PivotTable التي تشترك في نفس ذاكرة التخزين المؤقت PivotCache.

**Returns:**
com.aspose.cells.PivotTable[] -
### getPreserveCellFormattingOnUpdate() {#getPreserveCellFormattingOnUpdate--}
```
public boolean getPreserveCellFormattingOnUpdate()
```


يشير إلى ما إذا كان يجب الحفاظ على تنسيق الخلايا ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) عند تحديث أو إعادة حساب جدول PivotTable.

**Returns:**
boolean
### getPreserveFormatting() {#getPreserveFormatting--}
```
public boolean getPreserveFormatting()
```


يشير إلى ما إذا كان تنسيق الخلايا ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) محفوظًا عند تحديث أو إعادة حساب جدول PivotTable.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام الخاصية PivotTable.PreserveCellFormattingOnUpdate property. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### getPrintDrill() {#getPrintDrill--}
```
public boolean getPrintDrill()
```


يحدد قيمة منطقية تشير إلى ما إذا كان يجب طباعة مؤشرات الحفر. طباعة أزرار التوسيع/الطي عندما تُعرض على pivottable.

**Returns:**
boolean
### getPrintTitles() {#getPrintTitles--}
```
public boolean getPrintTitles()
```


يشير إلى ما إذا كانت عناوين الطباعة للورقة يتم تعيينها بناءً على تقرير PivotTable. القيمة الافتراضية هي false.

**Returns:**
boolean
### getRefreshDataOnOpeningFile() {#getRefreshDataOnOpeningFile--}
```
public boolean getRefreshDataOnOpeningFile()
```


يشير إلى ما إذا كان يجب تحديث البيانات عند فتح الملف.

**Returns:**
boolean
### getRefreshDate() {#getRefreshDate--}
```
public DateTime getRefreshDate()
```


يحصل على تاريخ ووقت آخر مرة تم فيها تحديث جدول PivotTable.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getRefreshedByWho() {#getRefreshedByWho--}
```
public String getRefreshedByWho()
```


يحصل على اسم آخر مستخدم قام بتحديث جدول PivotTable هذا.

**Returns:**
java.lang.String
### getRepeatItemsOnEachPrintedPage() {#getRepeatItemsOnEachPrintedPage--}
```
public boolean getRepeatItemsOnEachPrintedPage()
```


يشير إلى ما إذا كانت تسميات عنصر Pivot في منطقة الصف تُكرر في كل صفحة مطبوعة لحقول Pivot في الشكل الجدولي.

**Returns:**
boolean
### getRowFields() {#getRowFields--}
```
public PivotFieldCollection getRowFields()
```


يعيد مجموعة [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) التي تُظهر حاليًا كحقول صف.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getRowGrand() {#getRowGrand--}
```
public boolean getRowGrand()
```


يشير إلى ما إذا كان يجب إظهار الإجماليات العامة للصفوف في جدول PivotTable هذا.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotTable.ShowRowGrandTotals method. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ ديسمبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### getRowHeaderCaption() {#getRowHeaderCaption--}
```
public String getRowHeaderCaption()
```


يحصل على التسمية المخصصة لرأس الصف في جدول PivotTable هذا.

**Returns:**
java.lang.String
### getRowRange() {#getRowRange--}
```
public CellArea getRowRange()
```


يرجع كائن CellArea الذي يمثل النطاق الذي يحتوي على منطقة الصف في تقرير PivotTable. للقراءة فقط.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getSaveData() {#getSaveData--}
```
public boolean getSaveData()
```


يشير إلى ما إذا كانت البيانات لتقرير PivotTable محفوظة مع المصنف.

**Returns:**
boolean
### getShowColumnGrandTotals() {#getShowColumnGrandTotals--}
```
public boolean getShowColumnGrandTotals()
```


يشير إلى ما إذا كان يجب عرض الإجماليات العامة للأعمدة في جدول PivotTable هذا.

**Returns:**
boolean
### getShowDataTips() {#getShowDataTips--}
```
public boolean getShowDataTips()
```


يشير إلى ما إذا كان يجب عرض تلميحات الأدوات لخلايا بيانات PivotTable.

**Returns:**
boolean
### getShowDrill() {#getShowDrill--}
```
public boolean getShowDrill()
```


يحصل على ما إذا كان يتم عرض أزرار التوسيع/الطي.

**Returns:**
boolean
### getShowEmptyCol() {#getShowEmptyCol--}
```
public boolean getShowEmptyCol()
```


يشير إلى ما إذا كان يجب تضمين الأعمدة الفارغة في الجدول

**Returns:**
boolean
### getShowEmptyRow() {#getShowEmptyRow--}
```
public boolean getShowEmptyRow()
```


يشير إلى ما إذا كان يجب تضمين الصفوف الفارغة في الجدول.

**Returns:**
boolean
### getShowHeaders() {#getShowHeaders--}
```
public boolean getShowHeaders()
```


ما إذا كان يجب عرض عناوين حقول البيانات وعناوين حقول Pivot على محور الصفوف ومحور الأعمدة في عرض PivotTable.

**Returns:**
boolean
### getShowMemberPropertyTips() {#getShowMemberPropertyTips--}
```
public boolean getShowMemberPropertyTips()
```


يحدد قيمة منطقية تشير إلى ما إذا كان يجب حذف معلومات خصائص العضو من تلميحات أدوات PivotTable.

**Returns:**
boolean
### getShowPivotStyleColumnHeader() {#getShowPivotStyleColumnHeader--}
```
public boolean getShowPivotStyleColumnHeader()
```


يشير إلى ما إذا كان يجب تطبيق النمط على رأس العمود في جدول Pivot.

**Returns:**
boolean
### getShowPivotStyleColumnStripes() {#getShowPivotStyleColumnStripes--}
```
public boolean getShowPivotStyleColumnStripes()
```


يشير إلى ما إذا كان تنسيق الشرائط يُطبق على العمود.

**Returns:**
boolean
### getShowPivotStyleLastColumn() {#getShowPivotStyleLastColumn--}
```
public boolean getShowPivotStyleLastColumn()
```


يشير إلى ما إذا كان تنسيق العمود يُطبق.

**Returns:**
boolean
### getShowPivotStyleRowHeader() {#getShowPivotStyleRowHeader--}
```
public boolean getShowPivotStyleRowHeader()
```


يشير إلى ما إذا كان يجب تطبيق النمط على رأس الصف في جدول Pivot.

**Returns:**
boolean
### getShowPivotStyleRowStripes() {#getShowPivotStyleRowStripes--}
```
public boolean getShowPivotStyleRowStripes()
```


يشير إلى ما إذا كان تنسيق الشرائط للصف يُطبق.

**Returns:**
boolean
### getShowRowGrandTotals() {#getShowRowGrandTotals--}
```
public boolean getShowRowGrandTotals()
```


يشير إلى ما إذا كان يجب عرض الإجماليات العامة للصفوف في جدول Pivot.

**Remarks**

**Returns:**
boolean
### getShowRowHeaderCaption() {#getShowRowHeaderCaption--}
```
public boolean getShowRowHeaderCaption()
```


يشير إلى ما إذا كان عنوان رأس الصف يُظهر في تقرير PivotTable يشير إلى ما إذا كان يتم عرض عناوين الحقول و قوائم الفلاتر المنسدلة.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام الخاصية PivotTable.ShowHeaders property. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أبريل 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### getShowValuesRow() {#getShowValuesRow--}
```
public boolean getShowValuesRow()
```


يشير إلى ما إذا كان يتم عرض صف القيم.

**Returns:**
boolean
### getSource() {#getSource--}
```
public String[] getSource()
```


احصل على مصدر البيانات لهذا جدول Pivot.

**Returns:**
java.lang.String[]
### getSource(boolean isOriginal) {#getSource-boolean-}
```
public String[] getSource(boolean isOriginal)
```


احصل على مصدر البيانات لهذا جدول Pivot.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isOriginal | boolean | يشير إلى ما إذا كان يجب إرجاع المصدر الأصلي أو مصدر البيانات للعرض. |

**Returns:**
java.lang.String[] -
### getSourceDataConnections() {#getSourceDataConnections--}
```
public ExternalConnection[] getSourceDataConnections()
```


يحصل على مصادر بيانات الاتصال الخارجي.

**Returns:**
com.aspose.cells.ExternalConnection[]
### getSourceType() {#getSourceType--}
```
public byte getSourceType()
```


يحصل على نوع مصدر البيانات لجدول Pivot.

انظر [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype).

**Returns:**
byte
### getSubtotalHiddenPageItems() {#getSubtotalHiddenPageItems--}
```
public boolean getSubtotalHiddenPageItems()
```


يشير إلى ما إذا كانت عناصر حقل الصفحة المخفية في تقرير PivotTable مشمولة في المجاميع الفرعية للصف والعمود، ومجاميع الكتلة، والمجاميع الكلية. القيمة الافتراضية هي False.

**Returns:**
boolean
### getTableRange1() {#getTableRange1--}
```
public CellArea getTableRange1()
```


إرجاع كائن CellArea يمثل النطاق الذي يحتوي على تقرير PivotTable بالكامل، لكنه لا يتضمن حقول الصفحات. للقراءة فقط.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getTableRange2() {#getTableRange2--}
```
public CellArea getTableRange2()
```


إرجاع كائن CellArea يمثل النطاق الذي يحتوي على تقرير PivotTable بالكامل، ويتضمن حقول الصفحات. للقراءة فقط.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getTag() {#getTag--}
```
public String getTag()
```


يحصل على سلسلة معرفة من قبل المستخدم مرتبطة بعرض PivotTable هذا.

**Returns:**
java.lang.String
### getTopRightArea() {#getTopRightArea--}
```
public CellArea getTopRightArea()
```


يمثل المنطقة الفارغة في أعلى يمين PivotTable (أعلى يسار للأوراق RTL).

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getValuesField() {#getValuesField--}
```
public PivotField getValuesField()
```


يحصل على كائن [PivotField](../../com.aspose.cells/pivotfield) الذي يمثل جميع حقول البيانات في PivotTable. للقراءة فقط. يتم إنشاؤه فقط عندما يكون هناك حقلان بيانات أو أكثر في منطقة البيانات. بشكل افتراضي يكون في منطقة الصف. يمكنك سحبه إلى منطقة الصف/العمود باستخدام طريقة PivotTable.AddFieldToArea().

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
### hasBlankRows() {#hasBlankRows--}
```
public boolean hasBlankRows()
```


يشير إلى ما إذا كان يجب إضافة صفوف فارغة. هذه الخاصية تنطبق فقط على أنواع تنسيق PivotTable التلقائي التي تحتاج إلى إضافة صفوف فارغة.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.InsertBlankRow. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أبريل 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoFormat() {#isAutoFormat--}
```
public boolean isAutoFormat()
```


يشير إلى ما إذا كان تقرير PivotTable مُنسقًا تلقائيًا. خانة الاختيار \"autoformat table\" الموجودة في خيار pivottable لبرنامج Excel 2003.

**Returns:**
boolean
### isExcel2003Compatible() {#isExcel2003Compatible--}
```
public boolean isExcel2003Compatible()
```


يحدد ما إذا كان PivotTable متوافقًا مع Excel2003 عند تحديثه؛ إذا كان true، يجب أن يكون النص أقل من أو يساوي 255 حرفًا، وبالتالي إذا كان النص أطول من 255 حرفًا سيتم قطعه. إذا كان false، لن يخضع النص لهذا القيد. القيمة الافتراضية هي true.

**Returns:**
boolean
### isGridDropZones() {#isGridDropZones--}
```
public boolean isGridDropZones()
```


يشير إلى ما إذا كان تقرير PivotTable يعرض تخطيط pivottable الكلاسيكي. (يتيح سحب الحقول داخل الشبكة)

**Returns:**
boolean
### isMultipleFieldFilters() {#isMultipleFieldFilters--}
```
public boolean isMultipleFieldFilters()
```


يحدد قيمة منطقية تشير إلى ما إذا كان بإمكان حقول PivotTable أن تحتوي على فلاتر متعددة مضبوطة عليها.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotTable.AllowMultipleFiltersPerField. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ ديسمبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### isSelected() {#isSelected--}
```
public boolean isSelected()
```


يشير إلى ما إذا تم تحديد هذا الـ PivotTable.

**Returns:**
boolean
### move(int row, int column) {#move-int-int-}
```
public void move(int row, int column)
```


ينقل الـ PivotTable إلى موقع مختلف في ورقة العمل.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotTable.MoveTo(). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ ديسمبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف. |
| عمود | int | فهرس العمود. |

### move(String destCellName) {#move-java.lang.String-}
```
public void move(String destCellName)
```


ينقل الـ PivotTable إلى موقع مختلف في ورقة العمل.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotTable.MoveTo(). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ ديسمبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| destCellName | java.lang.String | اسم الخلية الوجهة. |

### moveItem(int region, String[] nodes, boolean absolute, int offset) {#moveItem-int-java.lang.String---boolean-int-}
```
public void moveItem(int region, String[] nodes, boolean absolute, int offset)
```


نقل عنصر واحد للأعلى أو للأسفل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| region | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). المنطقة. فقط للصف أو العمود. |
| العقد | java.lang.String[] | العنصر. |
| مطلق | boolean | يشير إلى ما إذا كان الإزاحة موقعًا مطلقًا. |
| الإزاحة | int | إذا كان absolute true: 0 يعني الانتقال إلى البداية، -1 يعني الانتقال إلى النهاية، والقيم الأخرى تعني موقعًا مطلقًا؛ وإلا فإن الإزاحة تكون موقعًا نسبيًا. |

### moveTo(int row, int column) {#moveTo-int-int-}
```
public void moveTo(int row, int column)
```


ينقل الـ PivotTable إلى موقع مختلف في ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف. |
| عمود | int | فهرس العمود. |

### moveTo(int sheetIndex, int row, int column) {#moveTo-int-int-int-}
```
public void moveTo(int sheetIndex, int row, int column)
```


ينقل الـ PivotTable إلى موقع مختلف في ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetIndex | int | فهرس ورقة العمل المستهدفة |
| صف | int | فهرس الصف. |
| عمود | int | فهرس العمود. |

### moveTo(String destCellName) {#moveTo-java.lang.String-}
```
public void moveTo(String destCellName)
```


ينقل الـ PivotTable إلى موقع مختلف في ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| destCellName | java.lang.String | اسم الخلية الوجهة. |

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
public int refresh()
```


تحديث [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) من مصدر البيانات وحساب البيانات والنمط لعرض الـ pivot.

**Remarks**

سيتم إعادة حساب جميع جداول pivot التي تعتمد على نفس PivotCache.

**Returns:**
int - [PivotRefreshState](../../com.aspose.cells/pivotrefreshstate).
### refresh(PivotTableRefreshOption option) {#refresh-com.aspose.cells.PivotTableRefreshOption-}
```
public int refresh(PivotTableRefreshOption option)
```


تحديث [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) من مصدر البيانات وحساب البيانات والنمط لعرض الـ pivot.

**Remarks**

سيتم إعادة حساب جميع جداول pivot التي تعتمد على نفس PivotCache.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) |  |

**Returns:**
int - [PivotRefreshState](../../com.aspose.cells/pivotrefreshstate).
### refreshData() {#refreshData--}
```
public int refreshData()
```


يقوم بتحديث البيانات من مصدر البيانات إلى ذاكرة التخزين المؤقت للـ pivot.

**Remarks**

سنقوم بجمع البيانات من مصدر البيانات إلى PivotCache، ثم حساب البيانات في الذاكرة إلى الخلايا. ومن الأفضل أن تستدعي ببساطة [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) لتحديث وحساب جميع جداول pivot في الملف، بدلاً من تحديث كل واحدة على حدة. ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة [PivotCache.refresh()](../../com.aspose.cells/pivotcache\#refresh--) وإزالة ما يلي [calculateData()](../../com.aspose.cells/pivottable\#calculateData--) لأن هذا الجدول سيُحسب عند تحديث [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ يونيو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### refreshData(PivotTableRefreshOption option) {#refreshData-com.aspose.cells.PivotTableRefreshOption-}
```
public int refreshData(PivotTableRefreshOption option)
```


يقوم بتحديث بيانات وإعدادات الـ pivottable من مصدر البيانات مع الخيارات.

**Remarks**

سنقوم بجمع البيانات من مصدر البيانات إلى PivotCache، ثم حساب البيانات في الذاكرة إلى الخلايا. ومن الأفضل أن تستدعي ببساطة [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) لتحديث وحساب جميع جداول pivot في الملف، بدلاً من تحديث كل واحدة على حدة. ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة [PivotCache.refresh()](../../com.aspose.cells/pivotcache\#refresh--) وإزالة ما يلي [calculateData()](../../com.aspose.cells/pivottable\#calculateData--) لأن هذا الجدول سيُحسب عند تحديث [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ يونيو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | الخيارات لتحديث مصدر بيانات الجدول المحوري. |

**Returns:**
int
### removeField(int fieldType, PivotField pivotField) {#removeField-int-com.aspose.cells.PivotField-}
```
public void removeField(int fieldType, PivotField pivotField)
```


إزالة الحقل من منطقة الحقل المحددة

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). نوع منطقة الحقول. |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | الحقل في الحقول الأساسية. |

### removeField(int fieldType, int baseFieldIndex) {#removeField-int-int-}
```
public void removeField(int fieldType, int baseFieldIndex)
```


يزيل حقلًا من منطقة الـ pivot المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). نوع منطقة الحقول. |
| baseFieldIndex | int | فهرس الحقل في الحقول الأساسية. |

### removeField(int fieldType, String fieldName) {#removeField-int-java.lang.String-}
```
public void removeField(int fieldType, String fieldName)
```


يزيل حقلًا من منطقة الحقل المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). نوع منطقة الحقول. |
| fieldName | java.lang.String | الاسم في الحقول الأساسية. |

### selectArea(CellArea ca) {#selectArea-com.aspose.cells.CellArea-}
```
public PivotAreaCollection selectArea(CellArea ca)
```


حدد منطقة من عرض جدول الـ pivot.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | منطقة الخلية. |

**Returns:**
[PivotAreaCollection](../../com.aspose.cells/pivotareacollection) - 
### setAllowMultipleFiltersPerField(boolean value) {#setAllowMultipleFiltersPerField-boolean-}
```
public void setAllowMultipleFiltersPerField(boolean value)
```


يحدد قيمة منطقية تشير إلى ما إذا كان بإمكان حقول PivotTable أن تحتوي على فلاتر متعددة مضبوطة عليها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAltTextDescription(String value) {#setAltTextDescription-java.lang.String-}
```
public void setAltTextDescription(String value)
```


يحصل على وصف النص البديل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setAltTextTitle(String value) {#setAltTextTitle-java.lang.String-}
```
public void setAltTextTitle(String value)
```


يضبط عنوان النص البديل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setAutoFormat(boolean value) {#setAutoFormat-boolean-}
```
public void setAutoFormat(boolean value)
```


يشير إلى ما إذا كان تقرير PivotTable مُنسقًا تلقائيًا. خانة الاختيار \"autoformat table\" الموجودة في خيار pivottable لبرنامج Excel 2003.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAutoFormatType(int value) {#setAutoFormatType-int-}
```
public void setAutoFormatType(int value)
```


يضبط نوع التنسيق التلقائي للـ PivotTable.

انظر [PivotTableAutoFormatType](../../com.aspose.cells/pivottableautoformattype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setAutofitColumnWidthOnUpdate(boolean value) {#setAutofitColumnWidthOnUpdate-boolean-}
```
public void setAutofitColumnWidthOnUpdate(boolean value)
```


يشير إلى ما إذا كان يجب ضبط عرض العمود تلقائيًا عند التحديث.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setColumnGrand(boolean value) {#setColumnGrand-boolean-}
```
public void setColumnGrand(boolean value)
```


يشير إلى ما إذا كان تقرير PivotTable يعرض الإجماليات العامة للأعمدة.

**Remarks**

ملاحظة: هذه الخاصية أصبحت مهجورة الآن. بدلاً من ذلك، يرجى استخدام طريقة PivotTable.ShowColumnGrandTotals. سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من ديسمبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setColumnHeaderCaption(String value) {#setColumnHeaderCaption-java.lang.String-}
```
public void setColumnHeaderCaption(String value)
```


يضبط التسمية المخصصة لرأس العمود في الـ PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCustomListSort(boolean value) {#setCustomListSort-boolean-}
```
public void setCustomListSort(boolean value)
```


يشير إلى ما إذا كان يجب اعتبار القائمة المخصصة المدمجة عند فرز البيانات

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDataFieldHeaderName(String value) {#setDataFieldHeaderName-java.lang.String-}
```
public void setDataFieldHeaderName(String value)
```


يضبط اسم رأس حقل منطقة القيم في الـ PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setDataSource(String[] value) {#setDataSource-java.lang.String---}
```
public void setDataSource(String[] value)
```


يضبط مصدر البيانات لجدول الـ pivot.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String[] |  |

### setDisplayErrorString(boolean value) {#setDisplayErrorString-boolean-}
```
public void setDisplayErrorString(boolean value)
```


يشير إلى ما إذا كان تقرير PivotTable يعرض سلسلة مخصصة في الخلايا التي تحتوي على أخطاء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDisplayImmediateItems(boolean value) {#setDisplayImmediateItems-boolean-}
```
public void setDisplayImmediateItems(boolean value)
```


يشير إلى ما إذا كانت العناصر في مناطق الصف والعمود مرئية عندما تكون منطقة البيانات في PivotTable فارغة. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDisplayNullString(boolean value) {#setDisplayNullString-boolean-}
```
public void setDisplayNullString(boolean value)
```


يشير إلى ما إذا كان تقرير PivotTable يعرض سلسلة مخصصة إذا كانت القيمة فارغة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEnableDataValueEditing(boolean value) {#setEnableDataValueEditing-boolean-}
```
public void setEnableDataValueEditing(boolean value)
```


يحدد قيمة منطقية تشير إلى ما إذا كان يُسمح للمستخدم بتحرير الخلايا في منطقة البيانات من pivottable. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEnableDrilldown(boolean value) {#setEnableDrilldown-boolean-}
```
public void setEnableDrilldown(boolean value)
```


يشير إلى ما إذا كان التفصيل (drilldown) مفعلاً.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEnableFieldDialog(boolean value) {#setEnableFieldDialog-boolean-}
```
public void setEnableFieldDialog(boolean value)
```


يشير إلى ما إذا كان مربع حوار حقل PivotTable متاحًا عندما ينقر المستخدم مزدوجًا على حقل PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEnableFieldList(boolean value) {#setEnableFieldList-boolean-}
```
public void setEnableFieldList(boolean value)
```


يشير إلى ما إذا كانت قائمة الحقول لـ PivotTable متاحة في عرض Excel.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEnableWizard(boolean value) {#setEnableWizard-boolean-}
```
public void setEnableWizard(boolean value)
```


يشير إلى ما إذا كان معالج PivotTable متاحًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setErrorString(String value) {#setErrorString-java.lang.String-}
```
public void setErrorString(String value)
```


يحصل على السلسلة المعروضة في الخلايا التي تحتوي على أخطاء عندما تكون خاصية DisplayErrorString صحيحة. القيمة الافتراضية هي سلسلة فارغة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setExcel2003Compatible(boolean value) {#setExcel2003Compatible-boolean-}
```
public void setExcel2003Compatible(boolean value)
```


يحدد ما إذا كان PivotTable متوافقًا مع Excel2003 عند تحديثه؛ إذا كان true، يجب أن يكون النص أقل من أو يساوي 255 حرفًا، وبالتالي إذا كان النص أطول من 255 حرفًا سيتم قطعه. إذا كان false، لن يخضع النص لهذا القيد. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFieldListSortAscending(boolean value) {#setFieldListSortAscending-boolean-}
```
public void setFieldListSortAscending(boolean value)
```


يشير إلى ما إذا كانت الحقول في PivotTable مرتبة بترتيب غير افتراضي في قائمة الحقول.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setGrandTotalName(String value) {#setGrandTotalName-java.lang.String-}
```
public void setGrandTotalName(String value)
```


يرجع التسمية التي تُعرض في عمود أو رأس الصف الإجمالي. القيمة الافتراضية هي السلسلة "Grand Total".

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setGridDropZones(boolean value) {#setGridDropZones-boolean-}
```
public void setGridDropZones(boolean value)
```


يشير إلى ما إذا كان تقرير PivotTable يعرض تخطيط pivottable الكلاسيكي. (يتيح سحب الحقول داخل الشبكة)

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHasBlankRows(boolean value) {#setHasBlankRows-boolean-}
```
public void setHasBlankRows(boolean value)
```


يشير إلى ما إذا كان يجب إضافة صفوف فارغة. هذه الخاصية تنطبق فقط على أنواع تنسيق PivotTable التلقائي التي تحتاج إلى إضافة صفوف فارغة.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotField.InsertBlankRow. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أبريل 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setIndent(int value) {#setIndent-int-}
```
public void setIndent(int value)
```


يحدد زيادة المسافة البادئة للمحور المدمج ويمكن استخدامها لتعيين تخطيط التقرير إلى الشكل المدمج.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setItemPrintTitles(boolean value) {#setItemPrintTitles-boolean-}
```
public void setItemPrintTitles(boolean value)
```


يشير إلى ما إذا كان يجب تكرار أسماء PivotItem في أعلى كل صفحة مطبوعة.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام الخاصية PivotTable.RepeatItemsOnEachPrintedPage property. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أكتوبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setManualUpdate(boolean value) {#setManualUpdate-boolean-}
```
public void setManualUpdate(boolean value)
```


يشير إلى ما إذا كان تقرير PivotTable يُعاد حسابه فقط عند طلب المستخدم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setMergeLabels(boolean value) {#setMergeLabels-boolean-}
```
public void setMergeLabels(boolean value)
```


يضبط ما إذا كان سيتم دمج تسميات الحقول الصفية/العمودية التي تمتد عبر عدة خلايا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setMissingItemsLimit(int value) {#setMissingItemsLimit-int-}
```
public void setMissingItemsLimit(int value)
```


يحدد قيمة منطقية تشير إلى ما إذا كان بإمكان حقول PivotTable أن تحتوي على فلاتر متعددة مضبوطة عليها.

انظر إلى [PivotMissingItemLimitType](../../com.aspose.cells/pivotmissingitemlimittype).

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام الخاصية PivotCache.MissingItemsLimit بدلاً من ذلك. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMultipleFieldFilters(boolean value) {#setMultipleFieldFilters-boolean-}
```
public void setMultipleFieldFilters(boolean value)
```


يحدد قيمة منطقية تشير إلى ما إذا كان بإمكان حقول PivotTable أن تحتوي على فلاتر متعددة مضبوطة عليها.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotTable.AllowMultipleFiltersPerField. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ ديسمبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


يحصل على اسم PivotTable

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setNullString(String value) {#setNullString-java.lang.String-}
```
public void setNullString(String value)
```


يحصل على السلسلة المعروضة في الخلايا التي تحتوي على قيم فارغة عندما تكون الخاصية DisplayNullString صحيحة. القيمة الافتراضية هي سلسلة فارغة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setPageFieldOrder(int value) {#setPageFieldOrder-int-}
```
public void setPageFieldOrder(int value)
```


يضبط الترتيب الذي تُضاف به حقول الصفحة إلى تخطيط تقرير الـ PivotTable.

انظر إلى [PrintOrderType](../../com.aspose.cells/printordertype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPageFieldWrapCount(int value) {#setPageFieldWrapCount-int-}
```
public void setPageFieldWrapCount(int value)
```


يحصل على عدد حقول الصفحة في كل عمود أو صف في تقرير PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPivotTableStyle(TableStyle value) {#setPivotTableStyle-com.aspose.cells.TableStyle-}
```
public void setPivotTableStyle(TableStyle value)
```


يحصل على إعدادات [TableStyle](../../com.aspose.cells/tablestyle) لهذا جدول PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [TableStyle](../../com.aspose.cells/tablestyle) |  |

### setPivotTableStyleName(String value) {#setPivotTableStyleName-java.lang.String-}
```
public void setPivotTableStyleName(String value)
```


يضبط اسم النمط لجدول الـ pivot.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setPivotTableStyleType(int value) {#setPivotTableStyleType-int-}
```
public void setPivotTableStyleType(int value)
```


يضبط نمط جدول الـ pivot المدمج.

انظر إلى [PivotTableStyleType](../../com.aspose.cells/pivottablestyletype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPreserveCellFormattingOnUpdate(boolean value) {#setPreserveCellFormattingOnUpdate-boolean-}
```
public void setPreserveCellFormattingOnUpdate(boolean value)
```


يشير إلى ما إذا كان يجب الحفاظ على تنسيق الخلايا ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) عند تحديث أو إعادة حساب جدول PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPreserveFormatting(boolean value) {#setPreserveFormatting-boolean-}
```
public void setPreserveFormatting(boolean value)
```


يشير إلى ما إذا كان تنسيق الخلايا ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) محفوظًا عند تحديث أو إعادة حساب جدول PivotTable.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام الخاصية PivotTable.PreserveCellFormattingOnUpdate property. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPrintDrill(boolean value) {#setPrintDrill-boolean-}
```
public void setPrintDrill(boolean value)
```


يحدد قيمة منطقية تشير إلى ما إذا كان يجب طباعة مؤشرات الحفر. طباعة أزرار التوسيع/الطي عندما تُعرض على pivottable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPrintTitles(boolean value) {#setPrintTitles-boolean-}
```
public void setPrintTitles(boolean value)
```


يشير إلى ما إذا كانت عناوين الطباعة للورقة يتم تعيينها بناءً على تقرير PivotTable. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRefreshDataOnOpeningFile(boolean value) {#setRefreshDataOnOpeningFile-boolean-}
```
public void setRefreshDataOnOpeningFile(boolean value)
```


يشير إلى ما إذا كان يجب تحديث البيانات عند فتح الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRepeatItemsOnEachPrintedPage(boolean value) {#setRepeatItemsOnEachPrintedPage-boolean-}
```
public void setRepeatItemsOnEachPrintedPage(boolean value)
```


يشير إلى ما إذا كانت تسميات عنصر Pivot في منطقة الصف تُكرر في كل صفحة مطبوعة لحقول Pivot في الشكل الجدولي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRowGrand(boolean value) {#setRowGrand-boolean-}
```
public void setRowGrand(boolean value)
```


يشير إلى ما إذا كان يجب إظهار الإجماليات العامة للصفوف في جدول PivotTable هذا.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة PivotTable.ShowRowGrandTotals method. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ ديسمبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRowHeaderCaption(String value) {#setRowHeaderCaption-java.lang.String-}
```
public void setRowHeaderCaption(String value)
```


يضبط التسمية المخصصة لرأس الصف في هذا الـ PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setSaveData(boolean value) {#setSaveData-boolean-}
```
public void setSaveData(boolean value)
```


يشير إلى ما إذا كانت البيانات لتقرير PivotTable محفوظة مع المصنف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


يشير إلى ما إذا تم تحديد هذا الـ PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowColumnGrandTotals(boolean value) {#setShowColumnGrandTotals-boolean-}
```
public void setShowColumnGrandTotals(boolean value)
```


يشير إلى ما إذا كان يجب عرض الإجماليات العامة للأعمدة في جدول PivotTable هذا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowDataTips(boolean value) {#setShowDataTips-boolean-}
```
public void setShowDataTips(boolean value)
```


يشير إلى ما إذا كان يجب عرض تلميحات الأدوات لخلايا بيانات PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowDrill(boolean value) {#setShowDrill-boolean-}
```
public void setShowDrill(boolean value)
```


يضبط ما إذا كان سيتم عرض أزرار التوسيع/الطي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowEmptyCol(boolean value) {#setShowEmptyCol-boolean-}
```
public void setShowEmptyCol(boolean value)
```


يشير إلى ما إذا كان يجب تضمين الأعمدة الفارغة في الجدول

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowEmptyRow(boolean value) {#setShowEmptyRow-boolean-}
```
public void setShowEmptyRow(boolean value)
```


يشير إلى ما إذا كان يجب تضمين الصفوف الفارغة في الجدول.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowHeaders(boolean value) {#setShowHeaders-boolean-}
```
public void setShowHeaders(boolean value)
```


ما إذا كان يجب عرض عناوين حقول البيانات وعناوين حقول Pivot على محور الصفوف ومحور الأعمدة في عرض PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowMemberPropertyTips(boolean value) {#setShowMemberPropertyTips-boolean-}
```
public void setShowMemberPropertyTips(boolean value)
```


يحدد قيمة منطقية تشير إلى ما إذا كان يجب حذف معلومات خصائص العضو من تلميحات أدوات PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowPivotStyleColumnHeader(boolean value) {#setShowPivotStyleColumnHeader-boolean-}
```
public void setShowPivotStyleColumnHeader(boolean value)
```


يشير إلى ما إذا كان يجب تطبيق النمط على رأس العمود في جدول Pivot.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowPivotStyleColumnStripes(boolean value) {#setShowPivotStyleColumnStripes-boolean-}
```
public void setShowPivotStyleColumnStripes(boolean value)
```


يشير إلى ما إذا كان تنسيق الشرائط يُطبق على العمود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowPivotStyleLastColumn(boolean value) {#setShowPivotStyleLastColumn-boolean-}
```
public void setShowPivotStyleLastColumn(boolean value)
```


يشير إلى ما إذا كان تنسيق العمود يُطبق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowPivotStyleRowHeader(boolean value) {#setShowPivotStyleRowHeader-boolean-}
```
public void setShowPivotStyleRowHeader(boolean value)
```


يشير إلى ما إذا كان يجب تطبيق النمط على رأس الصف في جدول Pivot.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowPivotStyleRowStripes(boolean value) {#setShowPivotStyleRowStripes-boolean-}
```
public void setShowPivotStyleRowStripes(boolean value)
```


يشير إلى ما إذا كان تنسيق الشرائط للصف يُطبق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowRowGrandTotals(boolean value) {#setShowRowGrandTotals-boolean-}
```
public void setShowRowGrandTotals(boolean value)
```


يشير إلى ما إذا كان يجب عرض الإجماليات العامة للصفوف في جدول Pivot.

**Remarks**

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowRowHeaderCaption(boolean value) {#setShowRowHeaderCaption-boolean-}
```
public void setShowRowHeaderCaption(boolean value)
```


يشير إلى ما إذا كان عنوان رأس الصف يُظهر في تقرير PivotTable يشير إلى ما إذا كان يتم عرض عناوين الحقول و قوائم الفلاتر المنسدلة.

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام الخاصية PivotTable.ShowHeaders property. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أبريل 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowValuesRow(boolean value) {#setShowValuesRow-boolean-}
```
public void setShowValuesRow(boolean value)
```


يشير إلى ما إذا كان يتم عرض صف القيم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSubtotalHiddenPageItems(boolean value) {#setSubtotalHiddenPageItems-boolean-}
```
public void setSubtotalHiddenPageItems(boolean value)
```


يشير إلى ما إذا كانت عناصر حقل الصفحة المخفية في تقرير PivotTable مشمولة في المجاميع الفرعية للصف والعمود، ومجاميع الكتلة، والمجاميع الكلية. القيمة الافتراضية هي False.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setTag(String value) {#setTag-java.lang.String-}
```
public void setTag(String value)
```


يضبط سلسلة معرفة من قبل المستخدم مرتبطة بعرض الـ PivotTable هذا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn) {#showDetail-int-int-boolean-int-int-}
```
public void showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn)
```


عرض تفاصيل عنصر واحد في منطقة البيانات إلى جدول جديد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowOffset | int | الإزاحة إلى الصف البيانات الأول في منطقة البيانات. |
| columnOffset | int | الإزاحة إلى العمود البيانات الأول في منطقة البيانات. |
| newSheet | boolean | عرض التفاصيل إلى ورقة عمل جديدة. |
| destRow | int | الصف المستهدف. |
| destColumn | int | العمود المستهدف. |

### showInCompactForm() {#showInCompactForm--}
```
public void showInCompactForm()
```


يُنسق عرض PivotTable في الشكل المدمج.

### showInOutlineForm() {#showInOutlineForm--}
```
public void showInOutlineForm()
```


يُنسق PivotTable في الشكل المخطط.

### showInTabularForm() {#showInTabularForm--}
```
public void showInTabularForm()
```


يُنسق PivotTable في الشكل الجدولي.

### showReportFilterPage(PivotField pageField) {#showReportFilterPage-com.aspose.cells.PivotField-}
```
public void showReportFilterPage(PivotField pageField)
```


عرض جميع صفحات مرشح التقرير وفقًا لـ PivotField، يجب أن يكون PivotField موجودًا في PageFields.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pageField | [PivotField](../../com.aspose.cells/pivotfield) | كائن PivotField |

### showReportFilterPageByIndex(int posIndex) {#showReportFilterPageByIndex-int-}
```
public void showReportFilterPageByIndex(int posIndex)
```


عرض جميع صفحات مرشح التقرير وفقًا لمؤشر الموقع في PageFields.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| posIndex | int | فهرس الموقع في PageFields |

### showReportFilterPageByName(String fieldName) {#showReportFilterPageByName-java.lang.String-}
```
public void showReportFilterPageByName(String fieldName)
```


عرض جميع صفحات مرشح التقرير وفقًا لاسم PivotField، يجب أن يكون PivotField موجودًا في PageFields.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldName | java.lang.String | اسم PivotField |

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

