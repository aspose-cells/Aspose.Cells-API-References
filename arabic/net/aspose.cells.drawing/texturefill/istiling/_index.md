---
title: "TextureFill.IsTiling"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextureFill. تشير إلى ما إذا كان يتم تكرار الصورة كملمس"
type: docs
url: /ar/net/aspose.cells.drawing/texturefill/istiling/
---
## TextureFill.IsTiling property

يشير إلى ما إذا كان يتم تكرار الصورة كنقش.

```csharp
public bool IsTiling { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextureFillPropertyIsTilingDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين بيانات المخطط
            chart.NSeries.Add("A1:B3", true);
            
            // تعيين ملء الملمس لمنطقة المخطط
            chart.PlotArea.Area.FillFormat.Texture = TextureType.BlueTissuePaper;
            
            // تعيين خاصية IsTiling
            chart.PlotArea.Area.FillFormat.TextureFill.IsTiling = true;
            
            // تحقق وأخرج قيمة IsTiling
            Console.WriteLine("IsTiling: " + chart.PlotArea.Area.FillFormat.TextureFill.IsTiling);
            
            // احفظ المصنف
            workbook.Save("TextureFillIsTilingDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


