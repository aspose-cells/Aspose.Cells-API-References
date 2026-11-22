---
title: "TextureFill.ImageData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextureFill. تحصل وتضبط بيانات الصورة للتعبئة"
type: docs
url: /ar/net/aspose.cells.drawing/texturefill/imagedata/
---
## TextureFill.ImageData property

يحصل ويضبط بيانات الصورة للتعبئة.

```csharp
public byte[] ImageData { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TextureFillPropertyImageDataDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 15, 15);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نوع تعبئة النسيج
            chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;

            // تحميل بيانات الصورة
            byte[] imageData = File.ReadAllBytes("texture.png");

            // تعيين بيانات الصورة لتعبئة النسيج
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;

            // احفظ المصنف
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


