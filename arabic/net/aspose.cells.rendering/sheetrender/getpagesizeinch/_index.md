---
title: "SheetRender.GetPageSizeInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SheetRender. احصل على حجم الصفحة بالبوصة للصورة الناتجة"
type: docs
url: /ar/net/aspose.cells.rendering/sheetrender/getpagesizeinch/
---
## SheetRender.GetPageSizeInch method

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
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodGetPageSizeInchWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.PageSetup.PrintArea = "A1:D10";
            worksheet.PageSetup.LeftMargin = 0;
            worksheet.PageSetup.RightMargin = 0;
            worksheet.PageSetup.TopMargin = 0;
            worksheet.PageSetup.BottomMargin = 0;

            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true,
                ImageType = ImageType.Png
            };

            SheetRender sheetRender = new SheetRender(worksheet, options);
            float[] pageSize = sheetRender.GetPageSizeInch(0);
            
            Console.WriteLine($"Page Size (Inches): Width={pageSize[0]}, Height={pageSize[1]}");
        }
    }
}
```

### انظر أيضًا

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


