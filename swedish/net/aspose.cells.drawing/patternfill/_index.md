---
title: "Klass PatternFill"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.PatternFill-klass. Inkapslar objektet som representerar mönsterfyllningsformat"
type: docs
url: /sv/net/aspose.cells.drawing/patternfill/
---
## PatternFill class

Inkapslar objektet som representerar mönsterfyllningsformat

```csharp
public class PatternFill : Fill
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BackgroundCellsColor](../../aspose.cells.drawing/patternfill/backgroundcellscolor/) { get; set; } | Hämtar och anger förgrundsobjektet [`CellsColor`](../../aspose.cells/cellscolor/). |
| [BackgroundColor](../../aspose.cells.drawing/patternfill/backgroundcolor/) { get; set; } | Hämtar eller anger bakgrundsfärgen för [`Area`](../area/). |
| [BackTransparency](../../aspose.cells.drawing/patternfill/backtransparency/) { get; set; } | Hämtar eller anger transparensen för bakgrundsfärgen. |
| [ForegroundCellsColor](../../aspose.cells.drawing/patternfill/foregroundcellscolor/) { get; set; } | Hämtar och anger förgrundsobjektet [`CellsColor`](../../aspose.cells/cellscolor/). |
| [ForegroundColor](../../aspose.cells.drawing/patternfill/foregroundcolor/) { get; set; } | Hämtar eller anger förgrundsfärgen. |
| [ForeTransparency](../../aspose.cells.drawing/patternfill/foretransparency/) { get; set; } | Hämtar eller anger transparensen för förgrundsfärgen. |
| [Pattern](../../aspose.cells.drawing/patternfill/pattern/) { get; set; } | Hämtar eller anger fyllningsmönster-typen |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Arv från [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Hämtar hashkoden.(Arv från [`Fill`](../fill/).) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassPatternFillDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa stil för cellen med BackgroundType-mönster
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.DiagonalStripe;
            style.ForegroundColor = Color.LightBlue;
            style.BackgroundColor = Color.DarkBlue;

            worksheet.Cells["B2"].SetStyle(style);
            worksheet.Cells["B2"].PutValue("PatternFill Demo");

            // Skapa form och konfigurera dess mönsterfyllning
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 200, 100);
            shape.Fill.FillType = FillType.Pattern;
            
            PatternFill shapePatternFill = shape.Fill.PatternFill;
            shapePatternFill.Pattern = FillPattern.DiagonalBrick;
            shapePatternFill.ForegroundColor = Color.LightBlue;
            shapePatternFill.BackgroundColor = Color.DarkBlue;
            shapePatternFill.ForeTransparency = 0.2;
            shapePatternFill.BackTransparency = 0.3;

            CellsColor cellsColor = workbook.CreateCellsColor();
            cellsColor.Color = Color.Gold;
            shapePatternFill.ForegroundCellsColor = cellsColor;

            workbook.Save("PatternFillDemo.xlsx");
        }
    }
}
```

### Se även

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


