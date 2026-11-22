---
title: "WorkbookRender.GetPageSizeInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WorkbookRender. احصل على حجم الصفحة بالبوصة لصورة الإخراج"
type: docs
url: /ar/net/aspose.cells.rendering/workbookrender/getpagesizeinch/
---
## WorkbookRender.GetPageSizeInch method

احصل على حجم الصفحة بالبوصة للصورة الناتجة.

```csharp
public float[] GetPageSizeInch(int pageIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس الصفحة | Int32 | فهرس الصفحة يبدأ من الصفر. |

### قيمة الإرجاع

حجم صورة الصفحة، [0] للعرض و[1] للارتفاع

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookRenderMethodGetPageSizeInchWithInt32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["A1"].PutValue("Test page size");
            sheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;

            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            WorkbookRender wr = new WorkbookRender(wb, imgOpt);
            
            float[] pageSize = wr.GetPageSizeInch(0);
            Console.WriteLine($"Page size in inches: {pageSize[0]} x {pageSize[1]}");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


