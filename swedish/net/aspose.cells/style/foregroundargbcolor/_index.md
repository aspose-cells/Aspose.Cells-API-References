---
title: "Style.ForegroundArgbColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-egenskap. Hämtar och anger förgrundsfärgen med ett 32‑bit ARGB‑värde"
type: docs
url: /sv/net/aspose.cells/style/foregroundargbcolor/
---
## Style.ForegroundArgbColor property

Hämtar och anger förgrundsfärgen med ett 32‑bitars ARGB‑värde.

```csharp
public int ForegroundArgbColor { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyForegroundArgbColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa en stil med specifik förgrundsfärg
            Style style = workbook.CreateStyle();
            style.ForegroundColor = System.Drawing.Color.FromArgb(255, 0, 255, 0); // Green color
            style.Pattern = BackgroundType.Solid;
            
            // Tillämpa stilen på en cell
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            // Hämta och visa förgrundens ARGB‑färgvärde
            int foregroundArgb = cell.GetStyle().ForegroundArgbColor;
            Console.WriteLine("Foreground ARGB Color: " + foregroundArgb);
            
            // Spara arbetsboken
            workbook.Save("ForegroundColorDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


