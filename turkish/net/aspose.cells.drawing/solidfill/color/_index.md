---
title: "SolidFill.Color"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SolidFill özelliği. Rengi alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/solidfill/color/
---
## SolidFill.Color property

Alır veya ayarlar Rengi.

```csharp
public Color Color { get; set; }
```

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SolidFillPropertyColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Çalışma sayfasına doğru parametrelerle bir şekil ekleyin
            Shape shape = sheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // Şekil özelliklerini renk ile ayarlayın
            Color fillColor = Color.LightBlue;
            Color textColor = Color.DarkBlue;
            string text = "Solid Fill Demo";

            // Color özelliğinin kullanımını gösterin
            shape.Fill.SolidFill.Color = fillColor;
            shape.LineFormat.ForeColor = fillColor;
            shape.Text = text;
            shape.Font.Color = textColor;

            // Çalışma kitabını kaydedin
            workbook.Save("SolidFillPropertyColorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SolidFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


