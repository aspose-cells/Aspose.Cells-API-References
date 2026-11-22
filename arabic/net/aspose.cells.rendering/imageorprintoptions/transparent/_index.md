---
title: "ImageOrPrintOptions.Transparent"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. تشير إلى ما إذا كان خلفية الصورة المُولدة يجب أن تكون شفافة"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/transparent/
---
## ImageOrPrintOptions.Transparent property

يشير إلى ما إذا كان خلفية الصورة المولدة يجب أن تكون شفافة.

```csharp
public bool Transparent { get; set; }
```

### ملاحظات

القيمة الافتراضية هي false. وهذا يعني أن خلفية الصور المُولدة هي بيضاء.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyTransparentDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Transparent Image Demo");
            
            // عيّن خيارات حفظ HTML باستخدام صورة PNG شفافة
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ImageOptions.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.ImageOptions.Transparent = true;
            options.ExportImagesAsBase64 = true;

            // احفظ دفتر العمل باستخدام خيارات الصورة الشفافة
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML with transparent images saved successfully.");
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


