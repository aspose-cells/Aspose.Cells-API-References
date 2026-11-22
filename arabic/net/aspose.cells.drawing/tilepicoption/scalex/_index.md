---
title: "TilePicOption.ScaleX"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TilePicOption. تحصل أو تعين مقياس X لتبليط الصورة"
type: docs
url: /ar/net/aspose.cells.drawing/tilepicoption/scalex/
---
## TilePicOption.ScaleX property

يحصل أو يضبط مقياس X لصورة البلاط.

```csharp
public double ScaleX { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TilePicOptionPropertyScaleXDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات عينة وأنشئ مخططًا
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // عيّن تعبئة نسيجية باستخدام صورة
            string imagePath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "texture.png");
            byte[] imageData = File.ReadAllBytes(imagePath);
            
            chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = new TilePicOption();
            
            // إظهار خاصية ScaleX
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleX = 50; // 50% horizontal scaling
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleY = 75; // 75% vertical scaling

            // احفظ المصنف
            workbook.Save(Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "ScaleXDemo.xlsx"));
        }
    }
}
```

### انظر أيضًا

* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


