---
title: "ImageOrPrintOptions.OnlyArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. إذا كانت هذه الخاصية true سيتم إخراج منطقة واحدة ولن يتم تطبيق أي مقياس"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/onlyarea/
---
## ImageOrPrintOptions.OnlyArea property

إذا كانت هذه الخاصية صحيحة، سيتم إخراج منطقة واحدة، ولن يؤثر أي مقياس.

```csharp
public bool OnlyArea { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyOnlyAreaDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // حدد خيارات الصورة باستخدام خاصية OnlyArea
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnlyArea = true; // Only render the used area

            // تحويل ورقة العمل إلى صورة
            SheetRender sr = new SheetRender(worksheet, options);
            using (MemoryStream ms = new MemoryStream())
            {
                sr.ToImage(0, ms);
                Console.WriteLine("Worksheet rendered to image with OnlyArea=true");
            }
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


