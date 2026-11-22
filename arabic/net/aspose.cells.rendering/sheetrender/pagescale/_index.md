---
title: "SheetRender.PageScale"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SheetRender. تحصل على مقياس الصفحة المحسوب للورقة. تُعيد المقياس المحدد إذا تم تعيين Zoom. وإلا تُعيد المقياس المحسوب وفقًا لـ FitToPagesWide و FitToPagesTall"
type: docs
url: /ar/net/aspose.cells.rendering/sheetrender/pagescale/
---
## SheetRender.PageScale property

يحصل على مقياس الصفحة المحسوب للورقة. يُعيد المقياس المحدد إذا تم تعيين [`Zoom`](../../../aspose.cells/pagesetup/zoom/). وإلا، يُعيد المقياس المحسوب وفقًا لـ [`FitToPagesWide`](../../../aspose.cells/pagesetup/fittopageswide/) و [`FitToPagesTall`](../../../aspose.cells/pagesetup/fittopagestall/).

```csharp
public double PageScale { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderPropertyPageScaleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue($"Item {i + 1}");
                sheet.Cells[i, 1].PutValue((i + 1) * 10);
            }

            // إنشاء خيارات الصورة أو الطباعة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // إنشاء SheetRender
            SheetRender sheetRender = new SheetRender(sheet, options);
            
            // احصل على مقياس الصفحة المحسوب وعرضه
            double pageScale = sheetRender.PageScale;
            Console.WriteLine($"Calculated Page Scale: {pageScale}");
        }
    }
}
```

### انظر أيضًا

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


