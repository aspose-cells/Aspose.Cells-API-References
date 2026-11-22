---
title: "TilePicOption.ScaleY"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TilePicOption. تحصل أو تعين مقياس Y لتكرار الصورة"
type: docs
url: /ar/net/aspose.cells.drawing/tilepicoption/scaley/
---
## TilePicOption.ScaleY property

يحصل أو يضبط مقياس Y لصورة البلاط.

```csharp
public double ScaleY { get; set; }
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
    public class TilePicOptionPropertyScaleYDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 15, 15);
            Chart chart = worksheet.Charts[chartIndex];
            
            // عيّن تعبئة نسيجية باستخدام صورة
            chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;
            byte[] imageData = File.ReadAllBytes("example.png");
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;
            
            // قم بتهيئة خيارات التكرار باستخدام ScaleY
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = new TilePicOption();
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleX = 50;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleY = 50;
            
            // احفظ المصنف
            workbook.Save("TilePicOptionScaleYDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


