---
title: Range
second_title: Aspose.Cells لمرجع .NET API
description: لتغليف الكائن الذي يمثل نطاقًا من الخلايا داخل جدول بيانات.
type: docs
weight: 5030
url: /ar/net/aspose.cells/range/
---
## Range class

لتغليف الكائن الذي يمثل نطاقًا من الخلايا داخل جدول بيانات.

```csharp
public class Range
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [Address](../../aspose.cells/range/address) { get; } | يحصل على عنوان النطاق . |
| [ColumnCount](../../aspose.cells/range/columncount) { get; } | الحصول على عدد الأعمدة في النطاق . |
| [ColumnWidth](../../aspose.cells/range/columnwidth) { get; set; } | تعيين عرض العمود لهذا النطاق أو الحصول عليه |
| [CurrentRegion](../../aspose.cells/range/currentregion) { get; } | إرجاع كائن النطاق الذي يمثل المنطقة الحالية. المنطقة الحالية هي نطاق محدد بأي مجموعة من الصفوف والأعمدة الفارغة. |
| [EntireColumn](../../aspose.cells/range/entirecolumn) { get; } | الحصول على كائن نطاق يمثل العمود (أو الأعمدة) بأكمله الذي يحتوي على النطاق المحدد. |
| [EntireRow](../../aspose.cells/range/entirerow) { get; } | الحصول على كائن نطاق يمثل الصف (أو الصفوف) بأكملها التي تحتوي على النطاق المحدد. |
| [FirstColumn](../../aspose.cells/range/firstcolumn) { get; } | يحصل على فهرس العمود الأول من النطاق. |
| [FirstRow](../../aspose.cells/range/firstrow) { get; } | يحصل على فهرس الصف الأول من النطاق . |
| [Height](../../aspose.cells/range/height) { get; } | الحصول على عرض النطاق بالنقاط. |
| [Hyperlinks](../../aspose.cells/range/hyperlinks) { get; } | يحصل على كل الارتباطات التشعبية في النطاق . |
| [Item](../../aspose.cells/range/item) { get; } | يحصل[`Cell`](../cell) كائن في هذا النطاق. |
| [Left](../../aspose.cells/range/left) { get; } | الحصول على المسافة ، بالنقاط ، من الحافة اليسرى للعمود A إلى الحافة اليسرى للنطاق . |
| [Name](../../aspose.cells/range/name) { get; set; } | الحصول على أو تحديد اسم النطاق . |
| [RefersTo](../../aspose.cells/range/refersto) { get; } | يحصل على النطاق الذي يشير إليه . |
| [RowCount](../../aspose.cells/range/rowcount) { get; } | الحصول على عدد الصفوف في النطاق . |
| [RowHeight](../../aspose.cells/range/rowheight) { get; set; } | تعيين ارتفاع الصفوف أو الحصول عليها في هذا النطاق |
| [Top](../../aspose.cells/range/top) { get; } | الحصول على المسافة ، بالنقاط ، من الحافة العلوية للصف 1 إلى الحافة العلوية للنطاق . |
| [Value](../../aspose.cells/range/value) { get; set; } | الحصول على قيمة النطاق وتعيينها. |
| [Width](../../aspose.cells/range/width) { get; } | الحصول على عرض النطاق بالنقاط. |
| [Worksheet](../../aspose.cells/range/worksheet) { get; } | يحصل على ملف[`Worksheet`](./worksheet) الكائن الذي يحتوي على هذا النطاق. |

## طُرق

| اسم | وصف |
| --- | --- |
| [ApplyStyle](../../aspose.cells/range/applystyle)(Style, StyleFlag) | يطبق التنسيقات على نطاق كامل . |
| [AutoFill](../../aspose.cells/range/autofill#autofill)(Range) | كل ملء النطاق المستهدف. |
| [AutoFill](../../aspose.cells/range/autofill#autofill_1)(Range, AutoFillType) | كل ملء النطاق المستهدف. |
| [Copy](../../aspose.cells/range/copy#copy)(Range) | نسخ البيانات (بما في ذلك الصيغ) والتنسيق والكائنات الرسومية وما إلى ذلك من نطاق مصدر. |
| [Copy](../../aspose.cells/range/copy#copy_1)(Range, PasteOptions) | نسخ النطاق باستخدام خيارات اللصق الخاصة. |
| [CopyData](../../aspose.cells/range/copydata)(Range) | نسخ بيانات الخلية (بما في ذلك الصيغ) من نطاق مصدر . |
| [CopyStyle](../../aspose.cells/range/copystyle)(Range) | نسخ إعدادات النمط من نطاق مصدر . |
| [CopyValue](../../aspose.cells/range/copyvalue)(Range) | ينسخ قيمة الخلية من نطاق مصدر . |
| [ExportDataTable](../../aspose.cells/range/exportdatatable#exportdatatable)() | لتصدير البيانات في هذا النطاق إلى ملفDataTable الكائن . |
| [ExportDataTable](../../aspose.cells/range/exportdatatable#exportdatatable_1)(ExportTableOptions) | لتصدير البيانات في هذا النطاق إلى ملفDataTable الكائن . |
| [ExportDataTableAsString](../../aspose.cells/range/exportdatatableasstring)() | لتصدير البيانات في هذا النطاق إلى ملفDataTable الكائن . |
| [GetCellOrNull](../../aspose.cells/range/getcellornull)(int, int) | يحصل[`Cell`](../cell) كائن أو فارغ في هذا النطاق. |
| [GetEnumerator](../../aspose.cells/range/getenumerator)() | الحصول على العداد للخلايا في هذا النطاق . |
| [GetOffset](../../aspose.cells/range/getoffset)(int, int) | يحصل[`Range`](../range) النطاق عن طريق الإزاحة. |
| [Intersect](../../aspose.cells/range/intersect)(Range) | إرجاع أ[`Range`](../range) يمثل التقاطع المستطيل لنطاقين. |
| [IsIntersect](../../aspose.cells/range/isintersect)(Range) | يشير إلى ما إذا كان النطاق متقاطعًا. |
| [Merge](../../aspose.cells/range/merge)() | دمج نطاق من الخلايا في خلية واحدة. |
| [MoveTo](../../aspose.cells/range/moveto)(int, int) | انقل النطاق الحالي إلى النطاق المصدق . |
| [PutValue](../../aspose.cells/range/putvalue)(string, bool, bool) | يضع قيمة في النطاق ، إذا كان ذلك مناسبًا ، فسيتم تحويل القيمة إلى نوع بيانات آخر وستتم إعادة تعيين تنسيق رقم الخلية. |
| [SetInsideBorders](../../aspose.cells/range/setinsideborders)(BorderType, CellBorderType, CellsColor) | تعيين الحدود الداخلية للنطاق . |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder)(BorderType, CellBorderType, Color) | يعين حدود المخطط حول نطاق من الخلايا. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders#setoutlineborders)(CellBorderType, Color) | تعيين حدود المخطط التفصيلي حول نطاق من الخلايا بنفس نمط ولون الحدود. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders#setoutlineborders_1)(CellBorderType[], Color[]) | تعيين حدود الخط حول نطاق من الخلايا. |
| [SetStyle](../../aspose.cells/range/setstyle)(Style) | يضبط نمط النطاق . |
| override [ToString](../../aspose.cells/range/tostring)() | إرجاع سلسلة تمثل كائن النطاق الحالي. |
| [Union](../../aspose.cells/range/union)(Range) | إرجاع اتحاد نطاقين . |
| [UnMerge](../../aspose.cells/range/unmerge)() | يقوم بإلغاء دمج الخلايا المدمجة من هذا النطاق. |

### أمثلة

```csharp

[C#]

// إنشاء كائن مصنف
Workbook workbook = new Workbook();
// احصل على خلايا ورقة العمل الأولى.
Cells cells = workbook.Worksheets[0].Cells;
// قم بإنشاء نطاق (A1: D3).
Range range = cells.CreateRange("A1", "D3");
// تعيين القيمة إلى النطاق.
range.Value = "Hello";
// احفظ ملف Excel
workbook.Save("book1.xlsm");

 [Visual Basic]

'إنشاء كائن مصنف
Dim workbook As Workbook = New Workbook()
'احصل على خلايا ورقة العمل الأولى.
Dim cells as Cells = workbook.Worksheets[0].Cells
'قم بإنشاء نطاق (A1: D3).
Dim range as Range = cells.CreateRange("A1", "D3")
'اضبط القيمة على النطاق.
range.Value = "Hello"
'احفظ ملف Excel
workbook.Save("book1.xlsm")
```

### أنظر أيضا

* مساحة الاسم [Aspose.Cells](../../aspose.cells)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
