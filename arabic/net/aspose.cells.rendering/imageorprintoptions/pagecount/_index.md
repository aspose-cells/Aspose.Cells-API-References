---
title: "ImageOrPrintOptions.PageCount"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. تحصل أو تضبط عدد الصفحات التي سيتم حفظها"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/pagecount/
---
## ImageOrPrintOptions.PageCount property

يحصل أو يضبط عدد الصفحات التي سيتم حفظها.

```csharp
public int PageCount { get; set; }
```

### ملاحظات

القيمة الافتراضية هي System.Int32.MaxValue مما يعني أن جميع الصفحات سيتم عرضها.

### أمثلة

```csharp
using System;
using System.IO;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyPageCountDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Page 1 Data");
            worksheet.Cells["A2"].PutValue("Sample Content");
            worksheet.Cells["A3"].PutValue("Demo for PageCount");
            
            // حدد منطقة الطباعة وإعداد الصفحة
            worksheet.PageSetup.PrintArea = "A1:A3";
            worksheet.PageSetup.LeftMargin = 0;
            worksheet.PageSetup.RightMargin = 0;
            worksheet.PageSetup.TopMargin = 0;
            worksheet.PageSetup.BottomMargin = 0;

            // إنشاء خيارات الصورة أو الطباعة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png; // Fully qualified namespace AsposeCellsExamples = 1; // Demonstrating PageCount property
            options.OnlyArea = true;

            // تحويل ورقة العمل إلى صورة
            SheetRender renderer = new SheetRender(worksheet, options);
            using (MemoryStream stream = new MemoryStream())
            {
                renderer.ToImage(0, stream);
                
                // احفظ الصورة إلى ملف
                string outputPath = "output.png";
                File.WriteAllBytes(outputPath, stream.ToArray());
                Console.WriteLine($"Output saved to: {outputPath}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


