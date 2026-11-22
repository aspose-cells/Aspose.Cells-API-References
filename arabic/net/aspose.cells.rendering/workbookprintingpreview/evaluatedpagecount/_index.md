---
title: "WorkbookPrintingPreview.EvaluatedPageCount"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookPrintingPreview. تقييم إجمالي عدد الصفحات في هذا دفتر العمل"
type: docs
url: /ar/net/aspose.cells.rendering/workbookprintingpreview/evaluatedpagecount/
---
## WorkbookPrintingPreview.EvaluatedPageCount property

تقييم العدد الإجمالي للصفحات في هذا المصنف

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
    public class WorkbookPrintingPreviewPropertyEvaluatedPageCountDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة إلى ورقة العمل
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].PutValue("Row " + (i + 1));
            }

            // إنشاء خيارات معاينة الطباعة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // إنشاء معاينة طباعة دفتر العمل
            WorkbookPrintingPreview printingPreview = new WorkbookPrintingPreview(workbook, options);
            
            // احصل على عدد الصفحات المقيم وعرضه
            Console.WriteLine("Evaluated Page Count: " + printingPreview.EvaluatedPageCount);
        }
    }
}
```

### انظر أيضًا

* class [WorkbookPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


