---
title: "StyleFlag.LeftBorder"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag-egenskap. Inställningar för vänster kant kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/leftborder/
---
## StyleFlag.LeftBorder property

Inställningar för vänsterkant kommer att tillämpas.

```csharp
public bool LeftBorder { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyLeftBorderDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            var workbook = new Workbook();
            var worksheet = workbook.Worksheets[0];

            // Skapa ett område och applicera vänsterkantstil
            var range = worksheet.Cells.CreateRange(1, 1, 1, 1);
            range.PutValue("Left Border Demo", false, false);

            // Skapa stil och flagga
            var style = workbook.CreateStyle();
            var flag = new StyleFlag();

            // Ställ in vänsterkantsegenskaper
            style.Borders[BorderType.LeftBorder].Color = Color.Green;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thick;
            flag.LeftBorder = true;

            // Applicera stilen med vänsterkantflagga
            range.ApplyStyle(style, flag);

            // Verifiera att vänsterkanten har tillämpats
            var appliedStyle = worksheet.Cells[1, 1].GetStyle();
            Console.WriteLine($"Left border color: {appliedStyle.Borders[BorderType.LeftBorder].Color}");
            Console.WriteLine($"Left border style: {appliedStyle.Borders[BorderType.LeftBorder].LineStyle}");

            // Spara arbetsboken
            workbook.Save("LeftBorderDemo.xlsx");
        }
    }
}
```

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


