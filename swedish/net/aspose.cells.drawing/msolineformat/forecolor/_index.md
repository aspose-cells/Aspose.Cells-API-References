---
title: "MsoLineFormat.ForeColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoLineFormat egenskap. Hämtar och anger färgen på kantlinjens förgrund"
type: docs
url: /sv/net/aspose.cells.drawing/msolineformat/forecolor/
---
## MsoLineFormat.ForeColor property

Hämtar och anger kantlinjens förgrundsfärg.

```csharp
public Color ForeColor { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyForeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 200, 100);
            
            // Ange radformatsegenskaper inklusive ForeColor
            textBox.LineFormat.ForeColor = Color.Red;
            textBox.LineFormat.Style = MsoLineStyle.Single;
            textBox.LineFormat.IsVisible = true;
            textBox.LineFormat.Weight = 2;

            workbook.Save("MsoLineFormatForeColorDemo.xlsx", SaveFormat.Xlsx);
            
            // Verifiera den sparade färgen
            Workbook loadedWorkbook = new Workbook("MsoLineFormatForeColorDemo.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            Console.WriteLine("Line ForeColor: " + loadedShape.LineFormat.ForeColor.ToString());
        }
    }
}
```

### Se även

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


