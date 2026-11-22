---
title: "FillFormat.GradientColor2"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FillFormat. تُرجع لون التدرج 2 للملء المحدد"
type: docs
url: /ar/net/aspose.cells.drawing/fillformat/gradientcolor2/
---
## FillFormat.GradientColor2 property

يرجع اللون المتدرج 2 للتعبئة المحددة.

```csharp
public Color GradientColor2 { get; }
```

### ملاحظات

فقط عندما يكون نوع لون التدرج هو GradientColorType.TwoColors، تكون هذه الخاصية ذات معنى.

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientColor2Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء شكل مستطيل بملء تدرج لوني ثنائي اللون
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 200);
            FillFormat fill = rectangle.Fill;
            
            fill.SetTwoColorGradient(Color.Red, Color.Blue, GradientStyleType.Horizontal, 2);

            // تحقق من خصائص لون التدرج
            Console.WriteLine("GradientColor2: " + fill.GradientColor2);
        }
    }
}
```

### انظر أيضًا

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


