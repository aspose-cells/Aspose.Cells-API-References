---
title: "Klass CellsColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CellsColor-klass. Representerar alla färgtyper"
type: docs
url: /sv/net/aspose.cells/cellscolor/
---
## CellsColor class

Representerar alla typer av färg.

```csharp
public class CellsColor
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Argb](../../aspose.cells/cellscolor/argb/) { get; set; } | Hämtar och sätter färgen från ett 32-bitars ARGB-värde. |
| [Color](../../aspose.cells/cellscolor/color/) { get; set; } | Hämtar och sätter RGB-färgen. |
| [ColorIndex](../../aspose.cells/cellscolor/colorindex/) { get; set; } | Hämtar och sätter färgindexet i färgpaletten. Gäller endast för indexerad färg. |
| [IsShapeColor](../../aspose.cells/cellscolor/isshapecolor/) { get; set; } | Hämtar och sätter färgen som ska tillämpas på cell eller form. |
| [ThemeColor](../../aspose.cells/cellscolor/themecolor/) { get; set; } | Hämtar temafärgen. Gäller endast för temafärgstyp. |
| [Transparency](../../aspose.cells/cellscolor/transparency/) { get; set; } | Hämtar och sätter transparens som ett värde från 0,0 (opak) till 1,0 (klar). |
| [Type](../../aspose.cells/cellscolor/type/) { get; } | Färgtypen. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [SetTintOfShapeColor](../../aspose.cells/cellscolor/settintofshapecolor/)(double) | Ställ in nyansen för formens färg |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsColorDemo
    {
        public static void CellsColorExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa ett cellområde
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "A10");

            // Skapa en CellsColor-instans
            CellsColor cellsColor = workbook.CreateCellsColor();

            // Ställ in egenskaper för CellsColor
            cellsColor.IsShapeColor = false;
            cellsColor.Color = Color.Red;
            cellsColor.ColorIndex = 5;
            cellsColor.Argb = Color.Blue.ToArgb();
            cellsColor.Transparency = 0.5;

            // Applicera CellsColor på området
            Style style = workbook.CreateStyle();
            style.ForegroundColor = cellsColor.Color;
            style.Pattern = BackgroundType.Solid;
            range.ApplyStyle(style, new StyleFlag { CellShading = true });

            // Spara arbetsboken
            workbook.Save("CellsColorExample.xlsx");
            workbook.Save("CellsColorExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


