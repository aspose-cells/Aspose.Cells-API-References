---
title: "MsoFillFormat.ForeColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFillFormat‑egenskap. Hämtar och anger fyllningens förgrundsfärg"
type: docs
url: /sv/net/aspose.cells.drawing/msofillformat/forecolor/
---
## MsoFillFormat.ForeColor property

Hämtar och anger fyllningens förgrundsfärg.

```csharp
public Color ForeColor { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatPropertyForeColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangel med alla nödvändiga parametrar
            var rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 150, 200);

            // Hämta fyllningsformatet
            MsoFillFormat fillFormat = rectangle.FillFormat;

            // Ange och demonstrera ForeColor‑egenskapen
            fillFormat.ForeColor = System.Drawing.Color.Red;
            Console.WriteLine("ForeColor set to: " + fillFormat.ForeColor);

            // Ändra ForeColor
            fillFormat.ForeColor = System.Drawing.Color.FromArgb(0, 128, 255);
            Console.WriteLine("ForeColor changed to: " + fillFormat.ForeColor);

            // Spara arbetsboken
            workbook.Save("MsoFillFormatForeColorDemo.xlsx");
        }
    }
}
```

### Se även

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


