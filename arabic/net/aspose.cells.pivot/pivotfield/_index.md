---
title: "الفئة PivotField"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Pivot.PivotField. تمثل حقلًا في تقرير PivotTable"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/
---
## PivotField class

يمثل حقلًا في تقرير PivotTable.

```csharp
public class PivotField : IDisposable
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AllowDraggingToColumn](../../aspose.cells.pivot/pivotfield/allowdraggingtocolumn/) { get; set; } | يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الأعمدة. القيمة الافتراضية هي true. |
| [AllowDraggingToData](../../aspose.cells.pivot/pivotfield/allowdraggingtodata/) { get; set; } | يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة القيم. القيمة الافتراضية هي true. |
| [AllowDraggingToPage](../../aspose.cells.pivot/pivotfield/allowdraggingtopage/) { get; set; } | يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الصفحات. القيمة الافتراضية هي true. |
| [AllowDraggingToRow](../../aspose.cells.pivot/pivotfield/allowdraggingtorow/) { get; set; } | يشير إلى ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الصفوف. القيمة الافتراضية هي true. |
| [AllowRemovingFromView](../../aspose.cells.pivot/pivotfield/allowremovingfromview/) { get; set; } | يشير إلى ما إذا كان يمكن إزالة حقل الـ Pivot هذا من عرض PivotTable. القيمة الافتراضية هي true. |
| [AutoShowCount](../../aspose.cells.pivot/pivotfield/autoshowcount/) { get; set; } | (**Obsolete.**) تمثّل عدد العناصر العليا أو السفلية التي تُظهر تلقائيًا في الحقل المحدد لجدول PivotTable. |
| [AutoShowField](../../aspose.cells.pivot/pivotfield/autoshowfield/) { get; set; } | (**Obsolete.**) يمثل فهرس الحقل المعروض تلقائيًا. -1 يعني PivotField نفسه. يجب أن يكون فهرس حقول البيانات. |
| [AutoSortField](../../aspose.cells.pivot/pivotfield/autosortfield/) { get; set; } | (**Obsolete.**) يمثل فهرس الحقل الذي يتم فرزه تلقائيًا. -1 يعني PivotField نفسه، والآخرون يعني موضع حقول البيانات. |
| [BaseIndex](../../aspose.cells.pivot/pivotfield/baseindex/) { get; set; } | يمثل الفهرس في حقول Pivot المصدر. |
| [CurrentPageItem](../../aspose.cells.pivot/pivotfield/currentpageitem/) { get; set; } | يحصل أو يعيّن عنصر الصفحة المعروض حاليًا لهذا الحقل المحوري (حقل الصفحة فقط). |
| [CurrentPageItemText](../../aspose.cells.pivot/pivotfield/currentpageitemtext/) { get; set; } | يحصل على نص العرض لعنصر الصفحة الحالي لهذا الحقل المحوري (حقل الصفحة فقط). |
| [DisplayName](../../aspose.cells.pivot/pivotfield/displayname/) { get; set; } | يمثل الاسم المعروض لحقل Pivot في عرض جدول Pivot. |
| [DragToColumn](../../aspose.cells.pivot/pivotfield/dragtocolumn/) { get; set; } | (**Obsolete.**) يحدد ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الأعمدة. القيمة الافتراضية هي true. |
| [DragToData](../../aspose.cells.pivot/pivotfield/dragtodata/) { get; set; } | (**Obsolete.**) يحدد ما إذا كان يمكن سحب الحقل المحدد إلى منطقة القيم. القيمة الافتراضية هي true. |
| [DragToHide](../../aspose.cells.pivot/pivotfield/dragtohide/) { get; set; } | (**Obsolete.**) يحدد ما إذا كان يمكن إزالة هذا الحقل المحوري من عرض PivotTable. القيمة الافتراضية هي true. |
| [DragToPage](../../aspose.cells.pivot/pivotfield/dragtopage/) { get; set; } | (**Obsolete.**) يحدد ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الصفحة. القيمة الافتراضية هي true. |
| [DragToRow](../../aspose.cells.pivot/pivotfield/dragtorow/) { get; set; } | (**Obsolete.**) يحدد ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الصفوف. القيمة الافتراضية هي true. |
| [Function](../../aspose.cells.pivot/pivotfield/function/) { get; set; } | يمثل الدالة المستخدمة لتلخيص حقل بيانات PivotTable هذا. |
| [GroupSettings](../../aspose.cells.pivot/pivotfield/groupsettings/) { get; } | يحصل على إعدادات التجميع للحقل المحوري. |
| [InsertBlankRow](../../aspose.cells.pivot/pivotfield/insertblankrow/) { get; set; } | يحدد ما إذا كان يجب إدراج سطر فارغ بعد كل عنصر. فقط لحقول الصفوف. |
| [IsAscendShow](../../aspose.cells.pivot/pivotfield/isascendshow/) { get; set; } | (**Obsolete.**) يحدد ما إذا كان الحقل المحدد في PivotTable يُعرض تلقائيًا بترتيب تصاعدي. |
| [IsAscendSort](../../aspose.cells.pivot/pivotfield/isascendsort/) { get; set; } | (**Obsolete.**) يحدد ما إذا كانت عناصر هذا الحقل المحوري مُرتبة تلقائيًا تصاعديًا. |
| [IsAutoShow](../../aspose.cells.pivot/pivotfield/isautoshow/) { get; set; } | (**Obsolete.**) يحدد ما إذا كان الحقل المحدد في PivotTable يُظهر تلقائيًا. |
| [IsAutoSort](../../aspose.cells.pivot/pivotfield/isautosort/) { get; set; } | (**Obsolete.**) يحدد ما إذا كانت عناصر هذا الحقل في PivotTable مُرتبة تلقائيًا. |
| [IsAutoSubtotals](../../aspose.cells.pivot/pivotfield/isautosubtotals/) { get; set; } | يحدد ما إذا كان الحقل المحدد يُظهر المجاميع الفرعية التلقائية. القيمة الافتراضية هي true. |
| [IsCalculatedField](../../aspose.cells.pivot/pivotfield/iscalculatedfield/) { get; } | يحدد ما إذا كان هذا الحقل المحوري حقلًا محسوبًا. |
| [IsIncludeNewItemsInFilter](../../aspose.cells.pivot/pivotfield/isincludenewitemsinfilter/) { get; set; } | يحدد ما إذا كان يجب تضمين عناصر جديدة إلى الحقل في الفلتر اليدوي. القيمة الافتراضية هي false. |
| [IsInsertPageBreaksBetweenItems](../../aspose.cells.pivot/pivotfield/isinsertpagebreaksbetweenitems/) { get; set; } | يحدد ما إذا كان يجب إدراج فواصل صفحات بعد كل عنصر. القيمة الافتراضية هي false. |
| [IsMultipleItemSelectionAllowed](../../aspose.cells.pivot/pivotfield/ismultipleitemselectionallowed/) { get; set; } | يحدد ما إذا كان يمكن اختيار عناصر متعددة في حقل الصفحة. القيمة الافتراضية هي false. |
| [IsRepeatItemLabels](../../aspose.cells.pivot/pivotfield/isrepeatitemlabels/) { get; set; } | يحدد ما إذا كان يجب تكرار تسميات الحقل في منطقة الصف أو العمود. القيمة الافتراضية هي false. |
| [IsValueFields](../../aspose.cells.pivot/pivotfield/isvaluefields/) { get; } | (**Obsolete.**) يشير إلى ما إذا كان هذا الحقل يمثل حقول القيم. |
| [IsValuesField](../../aspose.cells.pivot/pivotfield/isvaluesfield/) { get; } | يشير إلى ما إذا كان هذا الحقل يمثل حقل القيم. |
| [ItemCount](../../aspose.cells.pivot/pivotfield/itemcount/) { get; } | (**Obsolete.**) يحصل على عدد العناصر الأساسية في هذا الحقل المحوري. |
| [Items](../../aspose.cells.pivot/pivotfield/items/) { get; } | احصل على جميع تسميات عناصر المحور في هذا الحقل. |
| [Name](../../aspose.cells.pivot/pivotfield/name/) { get; set; } | يمثل اسم PivotField. |
| [NonAutoSortDefault](../../aspose.cells.pivot/pivotfield/nonautosortdefault/) { get; set; } | (**Obsolete.**) يشير إلى ما إذا كانت عملية الفرز التي ستُطبق على هذا الحقل المحوري هي عملية فرز تلقائي أو فرز بيانات بسيط. |
| [Number](../../aspose.cells.pivot/pivotfield/number/) { get; set; } | يمثل تنسيق العرض المدمج للأرقام والتواريخ. |
| [NumberFormat](../../aspose.cells.pivot/pivotfield/numberformat/) { get; set; } | يمثل تنسيق العرض المخصص للأرقام والتواريخ. |
| [OriginalItems](../../aspose.cells.pivot/pivotfield/originalitems/) { get; } | احصل على العناصر الأساسية الأصلية؛ |
| [PivotItems](../../aspose.cells.pivot/pivotfield/pivotitems/) { get; } | يحصل على عناصر المحور في الحقل المحوري |
| [Position](../../aspose.cells.pivot/pivotfield/position/) { get; } | يمثل فهرس `PivotField` في المنطقة. |
| [RegionType](../../aspose.cells.pivot/pivotfield/regiontype/) { get; } | يحدد منطقة جدول المحور التي يُعرض فيها هذا الحقل. |
| [ShowAllItems](../../aspose.cells.pivot/pivotfield/showallitems/) { get; set; } | يشير إلى ما إذا كان يجب عرض جميع العناصر في عرض PivotTable، حتى إذا لم تحتوي على بيانات ملخص. القيمة الافتراضية هي false. |
| [ShowCompact](../../aspose.cells.pivot/pivotfield/showcompact/) { get; set; } | (**Obsolete.**) يشير إلى ما إذا كان يجب عرض تسميات الحقل التالي في نفس العمود في عرض Pivot Table. فقط لحقول الصف. |
| [ShowInCompactForm](../../aspose.cells.pivot/pivotfield/showincompactform/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان حقل الصف هذا يستخدم تخطيط الشكل المدمج. ينطبق فقط على حقول الصف. |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivotfield/showinoutlineform/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان حقل الصف هذا يستخدم تخطيط المخطط التفصيلي. ينطبق فقط على حقول الصف. |
| [ShowSubtotalAtTop](../../aspose.cells.pivot/pivotfield/showsubtotalattop/) { get; set; } | يشير إلى ما إذا كان يجب عرض المجاميع الفرعية في أعلى أو أسفل العناصر. |
| [ShowValuesSetting](../../aspose.cells.pivot/pivotfield/showvaluessetting/) { get; } | يحصل على إعدادات عرض القيم كما عندما يكون حساب ShowDataAs قيد الاستخدام. |
| [SortSetting](../../aspose.cells.pivot/pivotfield/sortsetting/) { get; } | يحصل على جميع إعدادات الفرز التلقائي |
| [Subtotals](../../aspose.cells.pivot/pivotfield/subtotals/) { get; set; } | يحصل أو يعيّن المجاميع الفرعية للحقل. فقط لحقل المحور الصف أو العمود. |
| [Top10AutoShowSettings](../../aspose.cells.pivot/pivotfield/top10autoshowsettings/) { get; } | يحصل على إعدادات Top 10 AutoShow لحقل محوري. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [AddCalculatedItem](../../aspose.cells.pivot/pivotfield/addcalculateditem/)(string, string) | أضف عنصر صيغة محسوبة إلى الحقل المحوري. |
| [ClearFilter](../../aspose.cells.pivot/pivotfield/clearfilter/)() | يمسح إعداد الفلتر على هذا الحقل المحوري. |
| [Dispose](../../aspose.cells.pivot/pivotfield/dispose/)() | ينفّذ مهامًا معرفة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة تعيين الموارد غير المُدارة. |
| [FilterByDate](../../aspose.cells.pivot/pivotfield/filterbydate/)(PivotFilterType, DateTime, DateTime) | يفلتر حسب قيم التاريخ لحقل المحور الصف أو العمود. |
| [FilterByLabel](../../aspose.cells.pivot/pivotfield/filterbylabel/)(PivotFilterType, string, string) | تصفية حسب التسميات لحقل pivot للصف أو العمود. |
| [FilterByValue](../../aspose.cells.pivot/pivotfield/filterbyvalue/)(int, PivotFilterType, double, double) | تصفية حسب القيم لحقل pivot للبيانات. |
| [FilterTop10](../../aspose.cells.pivot/pivotfield/filtertop10/)(int, PivotFilterType, bool, int) | تصفية حسب القيم لحقل pivot للبيانات. |
| [GetCalculatedFieldFormula](../../aspose.cells.pivot/pivotfield/getcalculatedfieldformula/)() | (**Obsolete.**) احصل على سلسلة الصيغة للحقل المحسوب المحدد. |
| [GetFilters](../../aspose.cells.pivot/pivotfield/getfilters/)() | يحصل على جميع عوامل تصفية المحور المطبقة لهذا الحقل المحوري. |
| [GetFormula](../../aspose.cells.pivot/pivotfield/getformula/)() | يحصل على صيغة الحقل المحسوب. يعمل فقط مع الحقل المحسوب. |
| [GetMaxValue](../../aspose.cells.pivot/pivotfield/getmaxvalue/)() | يحصل على القيمة القصوى لهذا الحقل. |
| [GetMinValue](../../aspose.cells.pivot/pivotfield/getminvalue/)() | يحصل على القيمة القصوى لهذا الحقل. |
| [GetPivotFilterByType](../../aspose.cells.pivot/pivotfield/getpivotfilterbytype/)(PivotFilterType) | يحصل على عامل تصفية المحور للحقل المحوري حسب النوع |
| [GetPivotFilters](../../aspose.cells.pivot/pivotfield/getpivotfilters/)() | (**Obsolete.**) يحصل على عوامل تصفية المحور للحقل المحوري |
| [GetSubtotals](../../aspose.cells.pivot/pivotfield/getsubtotals/)(PivotFieldSubtotalType) | يشير إلى ما إذا كان يجب إظهار المجموع الفرعي المحدد لهذا الحقل المحوري. |
| [Group](../../aspose.cells.pivot/pivotfield/group/#group)() | تجميع الحقل تلقائيًا. |
| [Group](../../aspose.cells.pivot/pivotfield/group/#group_1)(PivotFieldGroupOptions) | يقوم بتجميع الحقل المحوري مع الخيارات. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby)(CustomPiovtFieldGroupItem[], bool) | (**Obsolete.**) تجميع مخصص للحقل. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_1)(DiscreteGroupItem[], bool) | (**Obsolete.**) تجميع مخصص للحقل. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_7)(double, bool) | (**Obsolete.**) تجميع الحقل تلقائيًا بفاصل |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_6)(PivotGroupByType[], double, bool) | (**Obsolete.**) تجميع الحقل تلقائيًا مع الداخلي |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_4)(double, double, double, bool) | (**Obsolete.**) تجميع الملف حسب الرقم. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_5)(DateTime, DateTime, PivotGroupByType[], double, bool) | (**Obsolete.**) تجميع الملف حسب أنواع تجميع التاريخ. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_2)(bool, double, bool, double, double, bool) | (**Obsolete.**) تجميع الملف حسب الرقم. |
| [GroupBy](../../aspose.cells.pivot/pivotfield/groupby/#groupby_3)(bool, DateTime, bool, DateTime, PivotGroupByType[], double, bool) | (**Obsolete.**) تجميع الملف حسب أنواع تجميع التاريخ. |
| [HideAllDetails](../../aspose.cells.pivot/pivotfield/hidealldetails/)() | يخفي جميع تفاصيل كل عنصر محوري. |
| [HideDetail](../../aspose.cells.pivot/pivotfield/hidedetail/)(bool) | (**Obsolete.**) يحدد ما إذا كانت تفاصيل جميع عناصر PivotItems في حقل محوري مخفية. أي طي/توسيع هذا الحقل. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem/#hideitem)(int, bool) | (**Obsolete.**) يحدد ما إذا كان عنصر PivotItem المحدد في حقل بيانات مخفيًا. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem/#hideitem_1)(string, bool) | (**Obsolete.**) يحدد ما إذا كان عنصر PivotItem المحدد في حقل بيانات مخفيًا. |
| [HideItemDetail](../../aspose.cells.pivot/pivotfield/hideitemdetail/)(int, bool) | (**Obsolete.**) يحدد ما إذا كان تفاصيل عنصر PivotItem المحدد في حقل محوري مخفية. |
| [InitPivotItems](../../aspose.cells.pivot/pivotfield/initpivotitems/)() | (**Obsolete.**) تهيئة عناصر المحور للحقل المحوري |
| [IsHiddenItem](../../aspose.cells.pivot/pivotfield/ishiddenitem/)(int) | (**Obsolete.**) يشير إلى ما إذا كان عنصر PivotItem المحدد مخفيًا. |
| [IsHiddenItemDetail](../../aspose.cells.pivot/pivotfield/ishiddenitemdetail/)(int) | (**Obsolete.**) يشير إلى ما إذا كان يجب إخفاء تفاصيل عنصر PivotItem المحدد. |
| [SetSubtotals](../../aspose.cells.pivot/pivotfield/setsubtotals/)(PivotFieldSubtotalType, bool) | يحدد كيفية تجميع المجموع الفرعي للحقل المحدد. |
| [ShowAllDetails](../../aspose.cells.pivot/pivotfield/showalldetails/)() | إظهار جميع تفاصيل كل عنصر محوري. |
| [ShowValuesAs](../../aspose.cells.pivot/pivotfield/showvaluesas/#showvaluesas_1)(PivotShowValuesAsType, int, int) | يحدد حساب \"إظهار القيم كـ\" لهذا الحقل المحوري. |
| [ShowValuesAs](../../aspose.cells.pivot/pivotfield/showvaluesas/#showvaluesas_2)(PivotShowValuesAsType, string, string) | يضبط حساب \"إظهار القيم كـ\" لهذا حقل البيانات. |
| [ShowValuesAs](../../aspose.cells.pivot/pivotfield/showvaluesas/#showvaluesas)(PivotFieldDataDisplayFormat, int, PivotItemPositionType, int) | (**Obsolete.**) يعرض قيم حقل البيانات بصيغة عرض مختلفة عندما يكون حساب ShowDataAs قيد الاستخدام. |
| [SortBy](../../aspose.cells.pivot/pivotfield/sortby/#sortby)(SortOrder) | يقوم بفرز هذا الحقل المحوري. |
| [SortBy](../../aspose.cells.pivot/pivotfield/sortby/#sortby_1)(SortOrder, int) | (**Obsolete.**) يقوم بفرز هذا الحقل المحوري. |
| [SortBy](../../aspose.cells.pivot/pivotfield/sortby/#sortby_3)(SortOrder, int, string) | يقوم بفرز هذا الحقل المحوري. |
| [SortBy](../../aspose.cells.pivot/pivotfield/sortby/#sortby_2)(SortOrder, int, PivotLineType, string) | (**Obsolete.**) يقوم بفرز هذا الحقل المحوري. |
| [Top10AutoShow](../../aspose.cells.pivot/pivotfield/top10autoshow/)(bool, bool, int, int) | يضبط إعدادات Top10 AutoShow لهذا الحقل المحوري. |
| [Ungroup](../../aspose.cells.pivot/pivotfield/ungroup/)() | إلغاء تجميع الحقل المحوري. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldDemo
    {
        public static void PivotFieldExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // إضافة بعض البيانات إلى ورقة العمل
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";

            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // أضف جدولًا محوريًا إلى ورقة العمل
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // إضافة حقول إلى الجدول المحوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "year");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "amount");

            // تعيين نمط جدول pivot
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // الوصول إلى حقل الصف
            PivotField rowField = pivotTable.RowFields[0];

            // تعيين خصائص PivotField
            rowField.DisplayName = "Custom Display Name";
            rowField.IsAutoSubtotals = false;
            rowField.DragToColumn = true;
            rowField.DragToHide = true;
            rowField.DragToRow = true;
            rowField.DragToPage = true;
            rowField.DragToData = true;
            rowField.IsMultipleItemSelectionAllowed = true;
            rowField.IsRepeatItemLabels = true;
            rowField.IsIncludeNewItemsInFilter = true;
            rowField.IsInsertPageBreaksBetweenItems = true;
            rowField.ShowAllItems = true;
            rowField.NonAutoSortDefault = true;
            rowField.IsAutoSort = true;
            rowField.IsAscendSort = true;
            rowField.AutoSortField = -1;
            rowField.IsAutoShow = true;
            rowField.IsAscendShow = true;
            rowField.AutoShowCount = 5;
            rowField.AutoShowField = -1;
            rowField.Function = ConsolidationFunction.Sum;
            rowField.ShowValuesAs(PivotFieldDataDisplayFormat.PercentageOfTotal, 0, PivotItemPositionType.Next, 0);
            rowField.CurrentPageItem = 1;
            rowField.Number = 0;
            rowField.InsertBlankRow = true;
            rowField.ShowSubtotalAtTop = true;
            rowField.ShowInOutlineForm = true;
            rowField.NumberFormat = "0.00";
            rowField.ShowCompact = true;

            // تحديث وحساب بيانات جدول المحور
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // احفظ المصنف
            workbook.Save("PivotFieldExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


