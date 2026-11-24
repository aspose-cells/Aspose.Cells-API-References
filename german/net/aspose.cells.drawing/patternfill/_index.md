---
title: "Klasse PatternFill"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.PatternFill Klasse. Kapselt das Objekt, das das Musterfüllformat darstellt"
type: docs
url: /de/net/aspose.cells.drawing/patternfill/
---
## PatternFill class

Kapselt das Objekt, das das Musterfüllformat darstellt

```csharp
public class PatternFill : Fill
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BackgroundCellsColor](../../aspose.cells.drawing/patternfill/backgroundcellscolor/) { get; set; } | Liest und setzt das Vordergrund‑[`CellsColor`](../../aspose.cells/cellscolor/)‑Objekt. |
| [BackgroundColor](../../aspose.cells.drawing/patternfill/backgroundcolor/) { get; set; } | Liest oder setzt die Hintergrundfarbe des [`Area`](../area/). |
| [BackTransparency](../../aspose.cells.drawing/patternfill/backtransparency/) { get; set; } | Liest oder setzt die Transparenz der Hintergrundfarbe. |
| [ForegroundCellsColor](../../aspose.cells.drawing/patternfill/foregroundcellscolor/) { get; set; } | Liest und setzt das Vordergrund‑[`CellsColor`](../../aspose.cells/cellscolor/)‑Objekt. |
| [ForegroundColor](../../aspose.cells.drawing/patternfill/foregroundcolor/) { get; set; } | Liest oder setzt die Vordergrundfarbe. |
| [ForeTransparency](../../aspose.cells.drawing/patternfill/foretransparency/) { get; set; } | Liest oder setzt die Transparenz der Vordergrundfarbe. |
| [Pattern](../../aspose.cells.drawing/patternfill/pattern/) { get; set; } | Liest oder setzt den Füllmuster‑Typ |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Geerbt von [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Liest den Hash‑Code. (Geerbt von [`Fill`](../fill/).) |

### Beispiele

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

            // Erstelle Stil für die Zelle mit dem BackgroundType‑Muster
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.DiagonalStripe;
            style.ForegroundColor = Color.LightBlue;
            style.BackgroundColor = Color.DarkBlue;

            worksheet.Cells["B2"].SetStyle(style);
            worksheet.Cells["B2"].PutValue("PatternFill Demo");

            // Erstelle Form und konfiguriere deren Musterfüllung
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

### Siehe auch

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


