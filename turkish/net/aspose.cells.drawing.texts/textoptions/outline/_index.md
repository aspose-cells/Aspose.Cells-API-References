---
title: "TextOptions.Outline"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextOptions özelliği. Metnin ana hat biçimini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textoptions/outline/
---
## TextOptions.Outline property

Metnin anahat biçimini temsil eder.

```csharp
public LineFormat Outline { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyOutlineDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Metin içeren bir şekil ekleyin
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);
            shape.Text = "Sample Text";

            // Metin seçeneklerine erişin
            TextOptions textOptions = shape.TextOptions;

            // Ana hat özelliklerini yapılandırın
            LineFormat outline = textOptions.Outline;
            outline.Weight = 2.48; // Set outline weight
            outline.DashStyle = MsoLineDashStyle.Solid; // Set line style
            outline.CompoundType = MsoLineStyle.Single; // Set compound type

            // Çalışma kitabını kaydedin
            workbook.Save("TextOutlineDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [LineFormat](../../../aspose.cells.drawing/lineformat/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


