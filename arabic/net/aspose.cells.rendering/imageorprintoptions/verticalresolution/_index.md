---
title: "ImageOrPrintOptions.VerticalResolution"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. تحصل أو تعيّن الدقة العمودية للصور المولدة بوحدة النقاط في البوصة"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/verticalresolution/
---
## ImageOrPrintOptions.VerticalResolution property

يحصل أو يضبط الدقة العمودية للصور المولدة، بوحدة النقاط في البوصة.

```csharp
public int VerticalResolution { get; set; }
```

### ملاحظات

القيمة الافتراضية هي 96.

ضبط [`HorizontalResolution`](../horizontalresolution/) و `VerticalResolution` يؤثران على عرض وارتفاع الصورة الناتجة بالبكسل.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyVerticalResolutionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات عينة وأنشئ مخططًا
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue(200);
            
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // أنشئ خيارات الصورة بدقة عمودية محددة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png;
            options.VerticalResolution = 300; // Setting vertical resolution to 300 DPI
            options.HorizontalResolution = 300; // For consistency, setting horizontal resolution too

            // احفظ المخطط كصورة بدقة محددة
            chart.ToImage("output_chart.png", options);
            
            Console.WriteLine("Chart saved as image with vertical resolution of 300 DPI.");
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


