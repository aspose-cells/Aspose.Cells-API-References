---
title: "AutoFitterOptions.AutoFitMergedCellsType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AutoFitterOptions. تحصل وتضبط نوع ضبط ارتفاع الصف تلقائيًا للخلايا المدمجة"
type: docs
url: /ar/net/aspose.cells/autofitteroptions/autofitmergedcellstype/
---
## AutoFitterOptions.AutoFitMergedCellsType property

يحصل ويضبط نوع ضبط ارتفاع الصف تلقائيًا للخلايا المدمجة.

```csharp
public AutoFitMergedCellsType AutoFitMergedCellsType { get; set; }
```

### ملاحظات

يُفترض في Excel تجاهل الخلايا المدمجة عند ضبط ارتفاع الصف، لذا يعمل Aspose.Cells وفقًا للإعداد الافتراضي لـ MS Excel. يرجى تعيين هذا النوع لتغيير طريقة ضبط ارتفاع الصف تلقائيًا للخلايا المدمجة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyAutoFitMergedCellsTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين بيانات عينة ودمج الخلايا
            worksheet.Cells["A1"].PutValue("This is a sample text for merged cells auto-fit demonstration");
            worksheet.Cells.Merge(0, 0, 3, 2); // Merge A1:B3

            // ضبط الصفوف تلقائيًا باستخدام AutoFitMergedCellsType.EachLine
            worksheet.AutoFitRows(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph
            });

            // ضبط الأعمدة تلقائيًا باستخدام AutoFitMergedCellsType.EachLine
            worksheet.AutoFitColumns(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph
            });

            // احفظ المصنف
            workbook.Save("AutoFitMergedCellsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [AutoFitMergedCellsType](../../autofitmergedcellstype/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


