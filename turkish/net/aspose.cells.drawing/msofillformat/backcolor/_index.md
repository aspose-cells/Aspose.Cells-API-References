---
title: "MsoFillFormat.BackColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoFillFormat özelliği. Dosyanın arka plan rengini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/msofillformat/backcolor/
---
## MsoFillFormat.BackColor property

Dosyanın arka rengini alır ve ayarlar.

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
    public class MsoFillFormatPropertyBackColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);
            MsoFillFormat fillFormat = arcShape.FillFormat;

            fillFormat.ForeColor = Color.Blue;
            fillFormat.BackColor = Color.LightBlue;
            fillFormat.Transparency = 0.5;

            Console.WriteLine("BackColor set to: " + fillFormat.BackColor.Name);

            workbook.Save("MsoFillFormatBackColorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


