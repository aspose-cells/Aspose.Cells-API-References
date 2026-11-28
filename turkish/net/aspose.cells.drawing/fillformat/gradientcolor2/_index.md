---
title: "FillFormat.GradientColor2"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FillFormat özelliği. Belirtilen doldurma için gradient renk 2'yi döndürür"
type: docs
url: /tr/net/aspose.cells.drawing/fillformat/gradientcolor2/
---
## FillFormat.GradientColor2 property

Belirtilen dolgu için gradient renk 2'yi döndürür.

```csharp
public Color GradientColor2 { get; }
```

### Açıklamalar

Yalnızca gradient renk türü GradientColorType.TwoColors olduğunda bu özellik anlamlıdır.

### Örnekler

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
            
            // İki renkli gradient doldurma ile dikdörtgen şekil oluştur
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 200);
            FillFormat fill = rectangle.Fill;
            
            fill.SetTwoColorGradient(Color.Red, Color.Blue, GradientStyleType.Horizontal, 2);

            // Gradient renk özelliklerini doğrula
            Console.WriteLine("GradientColor2: " + fill.GradientColor2);
        }
    }
}
```

### Ayrıca Bakınız

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


