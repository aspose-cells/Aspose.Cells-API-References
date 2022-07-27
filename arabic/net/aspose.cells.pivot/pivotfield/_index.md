---
title: PivotField
second_title: Aspose.Cells لمرجع .NET API
description: يمثل حقلاً في تقرير PivotTable .
type: docs
weight: 4530
url: /ar/net/aspose.cells.pivot/pivotfield/
---
## PivotField class

يمثل حقلاً في تقرير PivotTable .

```csharp
public class PivotField
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [AutoShowCount](../../aspose.cells.pivot/pivotfield/autoshowcount) { get; set; } | يمثل عدد العناصر العلوية أو السفلية التي تظهر تلقائيًا في حقل PivotTable المحدد. |
| [AutoShowField](../../aspose.cells.pivot/pivotfield/autoshowfield) { get; set; } | يمثل فهرس حقل العرض التلقائي. -1 تعني PivotField نفسها. يجب أن يكون فهرس حقول البيانات. |
| [AutoSortField](../../aspose.cells.pivot/pivotfield/autosortfield) { get; set; } | يمثل فهرس حقل الفرز التلقائي. -1 تعني PivotField نفسها ، والبعض الآخر يعني موضع حقول البيانات. |
| [BaseFieldIndex](../../aspose.cells.pivot/pivotfield/basefieldindex) { get; set; } | يمثل الحقل الأساسي لحساب مخصص. |
| [BaseIndex](../../aspose.cells.pivot/pivotfield/baseindex) { get; set; } | يمثل فهرس PivotField في PivotField الأساسية. |
| [BaseItemIndex](../../aspose.cells.pivot/pivotfield/baseitemindex) { get; set; } | يمثل العنصر في الحقل الأساسي لحساب مخصص . صالح فقط لحقول البيانات. |
| [BaseItemPosition](../../aspose.cells.pivot/pivotfield/baseitemposition) { get; set; } | يمثل العنصر في الحقل الأساسي لحساب مخصص . صالح فقط لحقول البيانات. نظرًا لأن PivotItemPosition.Custom للقراءة فقط ، إذا كنت بحاجة إلى تعيين PivotItemPosition.Custom ، يرجى تعيين PivotField.BaseItemIndex السمة. |
| [CurrentPageItem](../../aspose.cells.pivot/pivotfield/currentpageitem) { get; set; } | يمثل عنصر الصفحة الحالي المعروض لحقل الصفحة (صالح فقط لحقول الصفحة). |
| [DataDisplayFormat](../../aspose.cells.pivot/pivotfield/datadisplayformat) { get; set; } | يمثل كيفية عرض القيم الموجودة في حقل البيانات. |
| [DisplayName](../../aspose.cells.pivot/pivotfield/displayname) { get; set; } | يمثل اسم عرض PivotField . |
| [DragToColumn](../../aspose.cells.pivot/pivotfield/dragtocolumn) { get; set; } | يشير إلى ما إذا كان الحقل المحدد يمكن سحبه إلى موضع العمود. القيمة الافتراضية هي true . |
| [DragToData](../../aspose.cells.pivot/pivotfield/dragtodata) { get; set; } | يشير إلى إمكانية سحب الحقل المحدد إلى موضع البيانات. القيمة الافتراضية صحيحة. |
| [DragToHide](../../aspose.cells.pivot/pivotfield/dragtohide) { get; set; } | يشير إلى إمكانية سحب الحقل المحدد إلى موضع الإخفاء. القيمة الافتراضية هي true . |
| [DragToPage](../../aspose.cells.pivot/pivotfield/dragtopage) { get; set; } | يشير إلى إمكانية سحب الحقل المحدد إلى موضع الصفحة. القيمة الافتراضية صحيحة. |
| [DragToRow](../../aspose.cells.pivot/pivotfield/dragtorow) { get; set; } | يشير إلى إمكانية سحب الحقل المحدد إلى موضع الصف . القيمة الافتراضية هي "true". |
| [Function](../../aspose.cells.pivot/pivotfield/function) { get; set; } | يمثل الوظيفة المستخدمة لتلخيص حقل بيانات PivotTable. |
| [InsertBlankRow](../../aspose.cells.pivot/pivotfield/insertblankrow) { get; set; } | يشير إلى ما إذا كان يتم إدخال سطر فارغ بعد كل عنصر. |
| [IsAscendShow](../../aspose.cells.pivot/pivotfield/isascendshow) { get; set; } | يشير إلى ما إذا كان حقل PivotTable المحدد يتم عرضه تلقائيًا بشكل تصاعدي. |
| [IsAscendSort](../../aspose.cells.pivot/pivotfield/isascendsort) { get; set; } | يشير إلى ما إذا كان حقل PivotTable المحدد يتم فرزه تلقائيًا تصاعديًا. |
| [IsAutoShow](../../aspose.cells.pivot/pivotfield/isautoshow) { get; set; } | يشير إلى ما إذا كان حقل PivotTable المحدد معروضًا تلقائيًا ، وصالح فقط لـ Excel 2003. |
| [IsAutoSort](../../aspose.cells.pivot/pivotfield/isautosort) { get; set; } | يشير إلى ما إذا كان سيتم فرز حقل PivotTable المحدد تلقائيًا. |
| [IsAutoSubtotals](../../aspose.cells.pivot/pivotfield/isautosubtotals) { get; set; } | يشير إلى ما إذا كان الحقل المحدد يعرض الإجماليات الفرعية التلقائية. الافتراضي هو الصحيح. |
| [IsCalculatedField](../../aspose.cells.pivot/pivotfield/iscalculatedfield) { get; } | يشير إلى ما إذا كان حقل PivotTable المحدد محسوبًا أم لا. |
| [IsIncludeNewItemsInFilter](../../aspose.cells.pivot/pivotfield/isincludenewitemsinfilter) { get; set; } | يشير إلى ما إذا كان الحقل يمكن أن يتضمن عناصر جديدة في filter اليدوي القيمة الافتراضية هي false. |
| [IsInsertPageBreaksBetweenItems](../../aspose.cells.pivot/pivotfield/isinsertpagebreaksbetweenitems) { get; set; } | يشير إلى ما إذا كان الحقل يمكنه إدراج فواصل صفحات بين items إدراج فاصل صفحة بعد كل item القيمة الافتراضية هي false. |
| [IsMultipleItemSelectionAllowed](../../aspose.cells.pivot/pivotfield/ismultipleitemselectionallowed) { get; set; } | يشير إلى ما إذا كان الحقل يمكن أن يحتوي على عدة عناصر محددة في حقل الصفحة القيمة الافتراضية هي "خطأ". |
| [IsRepeatItemLabels](../../aspose.cells.pivot/pivotfield/isrepeatitemlabels) { get; set; } | يشير إلى ما إذا كان الحقل يمكنه تكرار تسميات العناصر القيمة الافتراضية هي false. |
| [ItemCount](../../aspose.cells.pivot/pivotfield/itemcount) { get; } | الحصول على عدد العناصر الأساسية لهذا الحقل المحوري. |
| [Items](../../aspose.cells.pivot/pivotfield/items) { get; } | الحصول على كافة العناصر الأساسية ؛ |
| [Name](../../aspose.cells.pivot/pivotfield/name) { get; } | يمثل اسم PivotField . |
| [Number](../../aspose.cells.pivot/pivotfield/number) { get; set; } | يمثل تنسيق العرض المضمن للأرقام والتواريخ. |
| [NumberFormat](../../aspose.cells.pivot/pivotfield/numberformat) { get; set; } | يمثل تنسيق العرض المخصص للأرقام والتواريخ. |
| [OriginalItems](../../aspose.cells.pivot/pivotfield/originalitems) { get; } | احصل على العناصر الأساسية الأصلية ؛ |
| [PivotItems](../../aspose.cells.pivot/pivotfield/pivotitems) { get; } | الحصول على العناصر المحورية للحقل المحوري |
| [Position](../../aspose.cells.pivot/pivotfield/position) { get; } | يمثل فهرس PivotField في PivotFields. |
| [Range](../../aspose.cells.pivot/pivotfield/range) { get; } | الحصول على نطاق المجموعة للحقل المحوري |
| [ShowAllItems](../../aspose.cells.pivot/pivotfield/showallitems) { get; set; } | يشير إلى ما إذا كانت كافة العناصر في تقرير PivotTable معروضة أم لا ، حتى إذا لم تكن تحتوي على بيانات موجزة. إظهار العناصر التي لا تحتوي على بيانات القيمة الافتراضية خاطئة. |
| [ShowCompact](../../aspose.cells.pivot/pivotfield/showcompact) { get; set; } | يشير إلى ما إذا كان عرض التسميات من الحقل التالي في نفس العمود في طريقة عرض Pivot Table |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivotfield/showinoutlineform) { get; set; } | يشير إلى ما إذا كان تخطيط هذا الحقل في نموذج المخطط التفصيلي في طريقة عرض Pivot Table |
| [ShowSubtotalAtTop](../../aspose.cells.pivot/pivotfield/showsubtotalattop) { get; set; } | عندما يكون ShowInOutlineForm صحيحًا ، قم بعرض المجاميع الفرعية أعلى قائمة العناصر بدلاً من عرضها في الأسفل |

## طُرق

| اسم | وصف |
| --- | --- |
| [AddCalculatedItem](../../aspose.cells.pivot/pivotfield/addcalculateditem)(string, string) | أضف عنصرًا محسوبًا إلى الحقل المحوري. |
| [GetCalculatedFieldFormula](../../aspose.cells.pivot/pivotfield/getcalculatedfieldformula)() | احصل على سلسلة الصيغة للحقل المحسوب المحدد . |
| [GetPivotFilterByType](../../aspose.cells.pivot/pivotfield/getpivotfilterbytype)(PivotFilterType) | يحصل على عامل التصفية المحوري للحقل المحوري حسب النوع |
| [GetPivotFilters](../../aspose.cells.pivot/pivotfield/getpivotfilters)() | الحصول على عوامل التصفية المحورية للحقل المحوري |
| [GetSubtotals](../../aspose.cells.pivot/pivotfield/getsubtotals)(PivotFieldSubtotalType) | تحديد ما إذا كان الحقل المحدد يعرض هذه المجاميع الفرعية. |
| [HideDetail](../../aspose.cells.pivot/pivotfield/hidedetail)(bool) | يحدد ما إذا كانت العناصر المحورية في الحقل المحوري هي تفاصيل مخفية. وهذا يعني طي / توسيع هذا الحقل . |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem#hideitem)(int, bool) | تعيين ما إذا كان PivotItem المحدد في حقل بيانات مخفيًا. |
| [HideItem](../../aspose.cells.pivot/pivotfield/hideitem#hideitem_1)(string, bool) | تعيين ما إذا كان PivotItem المحدد في حقل بيانات مخفيًا. |
| [HideItemDetail](../../aspose.cells.pivot/pivotfield/hideitemdetail)(int, bool) | تعيين ما إذا كان PivotItem المحدد في حقل محوري هو تفاصيل مخفية. |
| [InitPivotItems](../../aspose.cells.pivot/pivotfield/initpivotitems)() | بدء العناصر المحورية للحقل المحوري |
| [IsHiddenItem](../../aspose.cells.pivot/pivotfield/ishiddenitem)(int) | يشير إلى ما إذا كان PivotItem المحدد مخفيًا. |
| [IsHiddenItemDetail](../../aspose.cells.pivot/pivotfield/ishiddenitemdetail)(int) | يشير إلى ما إذا كان PivotItem المحدد هو تفاصيل مخفية. |
| [SetSubtotals](../../aspose.cells.pivot/pivotfield/setsubtotals)(PivotFieldSubtotalType, bool) | يحدد ما إذا كان الحقل المحدد يعرض هذه المجاميع الفرعية. |

### أمثلة

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
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

PivotTableCollection pivots = sheet.PivotTables;

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

// تغيير سمات PivotField
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

pivot.RefreshData();
pivot.CalculateData();

// قم بعملك

book.Save("out.xlsx");

[Visual Basic]

Dim book As Workbook = New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells

cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables
Dim pivotIndex As Int32 = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable")
Dim pivot As PivotTable = pivots(pivotIndex)
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
Pivot.AddFieldToArea(PivotFieldType.Column, "year")
Pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10

'Change PivotField's attributes
Dim rowField As PivotField = pivot.RowFields(0)
rowField.DisplayName = "custom display name"

pivot.RefreshData()
pivot.CalculateData()

book.Save("out_vb.xlsx")
```

### أنظر أيضا

* مساحة الاسم [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
