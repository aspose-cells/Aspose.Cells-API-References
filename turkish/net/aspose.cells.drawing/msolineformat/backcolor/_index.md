---
title: "MsoLineFormat.BackColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoLineFormat özelliği. Kenar çizgi arka plan rengini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/msolineformat/backcolor/
---
## MsoLineFormat.BackColor property

Kenarlık çizgi arka plan rengini alır ve ayarlar.

```csharp
public Color BackColor { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyBackColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir çizgi şekli ekleyin
            Shape line = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);

            // Çizgi özelliklerini ayarlayın
            line.LineFormat.ForeColor = Color.Red;
            line.LineFormat.BackColor = Color.Yellow; // Demonstrating BackColor usage
            line.LineFormat.DashStyle = MsoLineDashStyle.Solid;
            line.LineFormat.Weight = 2.0;

            // Çalışma kitabını kaydedin
            workbook.Save("LineFormatBackColorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


