---
title: "SheetPrintingPreview.EvaluatedPageCount"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SheetPrintingPreview. تقييم العدد الإجمالي للصفحات في هذه ورقة العمل"
type: docs
url: /ar/net/aspose.cells.rendering/sheetprintingpreview/evaluatedpagecount/
---
## SheetPrintingPreview.EvaluatedPageCount property

تقييم العدد الإجمالي للصفحات في ورقة العمل هذه

```csharp
public int EvaluatedPageCount { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetPrintingPreviewPropertyEvaluatedPageCountDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة إلى ورقة العمل
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }

            ImageOrPrintOptions options = new ImageOrPrintOptions();
            SheetPrintingPreview preview = new SheetPrintingPreview(worksheet, options);
            
            Console.WriteLine("Evaluated Page Count: " + preview.EvaluatedPageCount);
        }
    }
}
```

### انظر أيضًا

* class [SheetPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


