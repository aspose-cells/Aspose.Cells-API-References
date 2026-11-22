---
title: "الفئة Range"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Range. تغلف الكائن الذي يمثل نطاقًا من الخلايا داخل جدول بيانات"
type: docs
url: /ar/net/aspose.cells/range/
---
## Range class

يحتوي على الكائن الذي يمثل نطاقًا من الخلايا داخل جدول البيانات.

```csharp
public class Range : IEnumerable
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [Range](range/#constructor)(CellArea, Cells) | منشئ الفئة. |
| [Range](range/#constructor_1)(int, int, int, int, Cells) | منشئ الفئة. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Address](../../aspose.cells/range/address/) { get; } | يحصل على عنوان النطاق. |
| [ColumnCount](../../aspose.cells/range/columncount/) { get; } | يحصل على عدد الأعمدة في النطاق. |
| [ColumnWidth](../../aspose.cells/range/columnwidth/) { get; set; } | يضبط أو يحصل على عرض العمود لهذا النطاق |
| [CurrentRegion](../../aspose.cells/range/currentregion/) { get; } | يرجع كائن Range يمثل المنطقة الحالية. المنطقة الحالية هي نطاق محاط بأي تركيبة من الصفوف الفارغة والأعمدة الفارغة. |
| [EntireColumn](../../aspose.cells/range/entirecolumn/) { get; } | يحصل على كائن Range يمثل العمود بالكامل (أو الأعمدة) الذي يحتوي على النطاق المحدد. |
| [EntireRow](../../aspose.cells/range/entirerow/) { get; } | يحصل على كائن Range يمثل الصف بالكامل (أو الصفوف) الذي يحتوي على النطاق المحدد. |
| [FirstColumn](../../aspose.cells/range/firstcolumn/) { get; } | يحصل على فهرس العمود الأول في النطاق. |
| [FirstRow](../../aspose.cells/range/firstrow/) { get; } | يحصل على فهرس الصف الأول في النطاق. |
| [Height](../../aspose.cells/range/height/) { get; } | يحصل على عرض النطاق بالنقاط. |
| [Hyperlinks](../../aspose.cells/range/hyperlinks/) { get; } | يحصل على جميع الروابط التشعبية في النطاق. |
| [Item](../../aspose.cells/range/item/) { get; } | يحصل على كائن [`Cell`](../cell/) في هذا النطاق. |
| [Left](../../aspose.cells/range/left/) { get; } | يحصل على المسافة، بالنقاط، من الحافة اليسرى للعمود A إلى الحافة اليسرى للنطاق. |
| [Name](../../aspose.cells/range/name/) { get; set; } | يحصل أو يضبط اسم النطاق. |
| [RefersTo](../../aspose.cells/range/refersto/) { get; } | يحصل على ما يشير إليه النطاق. |
| [RowCount](../../aspose.cells/range/rowcount/) { get; } | يحصل على عدد الصفوف في النطاق. |
| [RowHeight](../../aspose.cells/range/rowheight/) { get; set; } | يضبط أو يحصل على ارتفاع الصفوف في هذا النطاق |
| [Top](../../aspose.cells/range/top/) { get; } | يحصل على المسافة، بالنقاط، من الحافة العلوية للصف 1 إلى الحافة العلوية للنطاق. |
| [Value](../../aspose.cells/range/value/) { get; set; } | يحصل ويضبط قيمة النطاق. |
| [Width](../../aspose.cells/range/width/) { get; } | يحصل على عرض النطاق بالنقاط. |
| [Worksheet](../../aspose.cells/range/worksheet/) { get; } | يحصل على كائن [`Worksheet`](./worksheet/) الذي يحتوي على هذا النطاق. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [AddHyperlink](../../aspose.cells/range/addhyperlink/)(string, string, string) | يضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا. |
| [ApplyStyle](../../aspose.cells/range/applystyle/)(Style, StyleFlag) | يطبق التنسيقات على نطاق كامل. |
| [AutoFill](../../aspose.cells/range/autofill/#autofill)(Range) | ملء النطاق الهدف تلقائيًا. |
| [AutoFill](../../aspose.cells/range/autofill/#autofill_1)(Range, AutoFillType) | ملء النطاق الهدف تلقائيًا. |
| [Clear](../../aspose.cells/range/clear/)() | يمسح هذا النطاق. |
| [ClearComments](../../aspose.cells/range/clearcomments/)() | يمسح تعليقات هذا النطاق. |
| [ClearContents](../../aspose.cells/range/clearcontents/)() | يمسح محتويات هذا النطاق. |
| [ClearFormats](../../aspose.cells/range/clearformats/)() | يمسح تنسيقات هذا النطاق. |
| [ClearHyperlinks](../../aspose.cells/range/clearhyperlinks/)(bool) | يزيل الروابط التشعبية فقط. |
| [Copy](../../aspose.cells/range/copy/#copy)(Range) | ينسخ البيانات (بما في ذلك الصيغ)، التنسيق، كائنات الرسم إلخ من نطاق مصدر. |
| [Copy](../../aspose.cells/range/copy/#copy_1)(Range, PasteOptions) | نسخ النطاق باستخدام خيارات اللصق الخاصة. |
| [CopyData](../../aspose.cells/range/copydata/)(Range) | ينسخ بيانات الخلية (بما في ذلك الصيغ) من نطاق مصدر. |
| [CopyStyle](../../aspose.cells/range/copystyle/)(Range) | ينسخ إعدادات النمط من نطاق مصدر. |
| [CopyValue](../../aspose.cells/range/copyvalue/)(Range) | ينسخ قيمة الخلية من نطاق مصدر. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable/#exportdatatable)() | يصدّر البيانات في هذا النطاق إلى كائن DataTable. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable/#exportdatatable_1)(ExportTableOptions) | يصدّر البيانات في هذا النطاق إلى كائن DataTable. |
| [ExportDataTableAsString](../../aspose.cells/range/exportdatatableasstring/)() | يصدّر البيانات في هذا النطاق إلى كائن DataTable. |
| [GetCellOrNull](../../aspose.cells/range/getcellornull/)(int, int) | يحصل على كائن [`Cell`](../cell/) أو null في هذا النطاق. |
| [GetEnumerator](../../aspose.cells/range/getenumerator/)() | يحصل على المُعدِّد للخلية في هذا Range. |
| [GetOffset](../../aspose.cells/range/getoffset/)(int, int) | يحصل على نطاق `Range` بالإزاحة. |
| [Intersect](../../aspose.cells/range/intersect/)(Range) | يرجع كائن `Range` يمثل تقاطع مستطيل لنطاقين. |
| [IsBlank](../../aspose.cells/range/isblank/)() | يشير إلى ما إذا كان النطاق يحتوي على قيم. |
| [IsIntersect](../../aspose.cells/range/isintersect/)(Range) | يشير إلى ما إذا كان النطاق متقاطعًا. |
| [Merge](../../aspose.cells/range/merge/)() | يجمع نطاقًا من الخلايا في خلية واحدة. |
| [MoveTo](../../aspose.cells/range/moveto/)(int, int) | انقل النطاق الحالي إلى النطاق الوجهة. |
| [PutValue](../../aspose.cells/range/putvalue/)(string, bool, bool) | يضع قيمة في النطاق، إذا كان مناسبًا سيتم تحويل القيمة إلى نوع بيانات آخر وسيتم إعادة ضبط تنسيق الرقم للخلية. |
| [SetInsideBorders](../../aspose.cells/range/setinsideborders/)(BorderType, CellBorderType, CellsColor) | حدد الحدود الداخلية للنطاق. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder/#setoutlineborder)(BorderType, CellBorderType, CellsColor) | يضبط حدًا خارجيًا حول نطاق من الخلايا. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder/#setoutlineborder_1)(BorderType, CellBorderType, Color) | يضبط حدًا خارجيًا حول نطاق من الخلايا. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders)(CellBorderType, CellsColor) | يضبط الحدود الخارجية حول نطاق من الخلايا بنفس نمط الحد واللون. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders_1)(CellBorderType, Color) | يضبط الحدود الخارجية حول نطاق من الخلايا بنفس نمط الحد واللون. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders_2)(CellBorderType[], Color[]) | يضبط حدود الخط الخارجي حول نطاق من الخلايا. |
| [SetStyle](../../aspose.cells/range/setstyle/#setstyle)(Style) | يضبط نمط النطاق. |
| [SetStyle](../../aspose.cells/range/setstyle/#setstyle_1)(Style, bool) | تطبيق نمط الخلية. |
| [ToHtml](../../aspose.cells/range/tohtml/)(HtmlSaveOptions) | تحويل النطاق إلى html. |
| [ToImage](../../aspose.cells/range/toimage/)(ImageOrPrintOptions) | يقوم بتحويل النطاق إلى صورة. |
| [ToJson](../../aspose.cells/range/tojson/)(JsonSaveOptions) | تحويل النطاق إلى قيمة JSON. |
| override [ToString](../../aspose.cells/range/tostring/)() | يعيد سلسلة تمثل كائن النطاق الحالي. |
| [Transpose](../../aspose.cells/range/transpose/)() | نقل (تدوير) البيانات من الصفوف إلى الأعمدة أو العكس. |
| [Union](../../aspose.cells/range/union/)(Range) | (**Obsolete.**) يرجع اتحاد نطاقين. |
| [UnionRang](../../aspose.cells/range/unionrang/)(Range) | (**Obsolete.**) يرجع نتيجة اتحاد نطاقين. |
| [UnionRanges](../../aspose.cells/range/unionranges/)(Range[]) | يرجع نتيجة اتحاد نطاقين. |
| [UnMerge](../../aspose.cells/range/unmerge/)() | يفك دمج الخلايا المدمجة في هذا النطاق. |

### ملاحظات

تشير فئة Range إلى منطقة من جدول بيانات Excel. باستخدامها، يمكنك تنسيق وتعيين قيمة النطاق. ويمكنك أيضًا نسخ نطاق Excel بسهولة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange("A1", "D3");
            range.Value = "Hello";
            workbook.Save("book1.xlsm");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


