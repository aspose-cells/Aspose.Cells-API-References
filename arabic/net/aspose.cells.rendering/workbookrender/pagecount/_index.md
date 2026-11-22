---
title: "WorkbookRender.PageCount"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookRender. تحصل على العدد الإجمالي للصفحات في دفتر العمل"
type: docs
url: /ar/net/aspose.cells.rendering/workbookrender/pagecount/
---
## WorkbookRender.PageCount property

يحصل على إجمالي عدد الصفحات في المصنف.

```csharp
public int PageCount { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookRenderPropertyPageCountDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Page 1 Content");
            
            // إضافة ورقة عمل ثانية
            workbook.Worksheets.Add();
            worksheet = workbook.Worksheets[1];
            worksheet.Cells["A1"].PutValue("Page 2 Content");

            // إنشاء خيارات العرض ومُصوّر دفتر العمل
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true
            };
            
            WorkbookRender renderer = new WorkbookRender(workbook, options);

            // عرض استخدام PageCount
            Console.WriteLine($"Total pages to render: {renderer.PageCount}");
            
            // عرض كل صفحة كصورة
            for (int i = 0; i < renderer.PageCount; i++)
            {
                string outputPath = $"Page_{i}.png";
                renderer.ToImage(i, outputPath);
                Console.WriteLine($"Rendered page {i+1} to {outputPath}");
            }
        }
    }
}
```

### انظر أيضًا

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


