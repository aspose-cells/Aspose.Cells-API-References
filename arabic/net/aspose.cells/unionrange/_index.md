---
title: "الفئة UnionRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.UnionRange فئة. تمثل نطاق الاتحاد"
type: docs
url: /ar/net/aspose.cells/unionrange/
---
## UnionRange class

يمثل نطاق الاتحاد.

```csharp
public class UnionRange : IEnumerable
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CellCount](../../aspose.cells/unionrange/cellcount/) { get; } | يحصل على عدد جميع الخلايا في النطاق. |
| [ColumnCount](../../aspose.cells/unionrange/columncount/) { get; } | يحصل على عدد الصفوف في النطاق. |
| [FirstColumn](../../aspose.cells/unionrange/firstcolumn/) { get; } | يحصل على فهرس العمود الأول في النطاق. |
| [FirstRow](../../aspose.cells/unionrange/firstrow/) { get; } | يحصل على فهرس الصف الأول في النطاق. |
| [HasRange](../../aspose.cells/unionrange/hasrange/) { get; } | يشير إلى ما إذا كان لهذا نطاق. |
| [Hyperlinks](../../aspose.cells/unionrange/hyperlinks/) { get; } | يحصل على جميع الروابط التشعبية في النطاق. |
| [Name](../../aspose.cells/unionrange/name/) { get; set; } | يحصل أو يضبط اسم النطاق. |
| [RangeCount](../../aspose.cells/unionrange/rangecount/) { get; } | يحصل على عدد النطاقات. |
| [Ranges](../../aspose.cells/unionrange/ranges/) { get; } | يحصل على جميع نطاقات الاتحاد. |
| [RefersTo](../../aspose.cells/unionrange/refersto/) { get; } | يحصل على ما يشير إليه النطاق. |
| [RowCount](../../aspose.cells/unionrange/rowcount/) { get; } | يحصل على عدد الصفوف في النطاق. |
| [Value](../../aspose.cells/unionrange/value/) { get; set; } | يحصل على قيم النطاق ويضبطها. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [ApplyStyle](../../aspose.cells/unionrange/applystyle/)(Style, StyleFlag) | يطبق التنسيقات على نطاق كامل. |
| [Copy](../../aspose.cells/unionrange/copy/)(UnionRange, PasteOptions) | نسخ النطاق باستخدام خيارات اللصق الخاصة. |
| [GetEnumerator](../../aspose.cells/unionrange/getenumerator/)() | يحصل على المُعدِّد للخلية في هذا Range. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect)(Range[]) | يتقاطع مع نطاق آخر. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect_2)(string) | يتقاطع مع نطاق آخر. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect_1)(UnionRange) | يتقاطع مع نطاق آخر. |
| [Merge](../../aspose.cells/unionrange/merge/)() | يجمع نطاقًا من الخلايا في خلية واحدة. |
| [PutValue](../../aspose.cells/unionrange/putvalue/)(string, bool, bool) | يضع قيمة في النطاق، إذا كان مناسبًا سيتم تحويل القيمة إلى نوع بيانات آخر وسيتم إعادة ضبط تنسيق الرقم للخلية. |
| [SetOutlineBorders](../../aspose.cells/unionrange/setoutlineborders/#setoutlineborders)(CellBorderType, Color) | يضبط الحدود الخارجية حول نطاق من الخلايا بنفس نمط الحد واللون. |
| [SetOutlineBorders](../../aspose.cells/unionrange/setoutlineborders/#setoutlineborders_1)(CellBorderType[], Color[]) | يضبط حدود الخط الخارجي حول نطاق من الخلايا. |
| [SetStyle](../../aspose.cells/unionrange/setstyle/)(Style) | يضبط نمط النطاق. |
| [Union](../../aspose.cells/unionrange/union/#union)(Range[]) | اتحاد النطاقات. |
| [Union](../../aspose.cells/unionrange/union/#union_2)(string) | اتحاد نطاق آخر. |
| [Union](../../aspose.cells/unionrange/union/#union_1)(UnionRange) | اتحاد نطاق آخر. |
| [UnMerge](../../aspose.cells/unionrange/unmerge/)() | يفك دمج الخلايا المدمجة في هذا النطاق. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassUnionRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء نطاق اتحاد باستخدام API الصحيح
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A10,C1:C10", 0);
            
            // تعيين قيمة للنطاق الاتحاد بالكامل
            unionRange.Value = "Test";
            
            // تطبيق النمط على نطاق الاتحاد
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            unionRange.ApplyStyle(style, new StyleFlag { All = true });
            
            // احفظ المصنف
            workbook.Save("UnionRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


