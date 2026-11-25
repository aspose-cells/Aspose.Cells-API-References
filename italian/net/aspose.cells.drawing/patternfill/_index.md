---
title: "Classe PatternFill"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.PatternFill. Incapsula l'oggetto che rappresenta il formato di riempimento a pattern."
type: docs
url: /it/net/aspose.cells.drawing/patternfill/
---
## PatternFill class

Incapsula l'oggetto che rappresenta il formato di riempimento a trama

```csharp
public class PatternFill : Fill
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BackgroundCellsColor](../../aspose.cells.drawing/patternfill/backgroundcellscolor/) { get; set; } | Ottiene e imposta l'oggetto di primo piano [`CellsColor`](../../aspose.cells/cellscolor/). |
| [BackgroundColor](../../aspose.cells.drawing/patternfill/backgroundcolor/) { get; set; } | Ottiene o imposta il colore di sfondo dell'[`Area`](../area/). |
| [BackTransparency](../../aspose.cells.drawing/patternfill/backtransparency/) { get; set; } | Ottiene o imposta la trasparenza del colore di sfondo. |
| [ForegroundCellsColor](../../aspose.cells.drawing/patternfill/foregroundcellscolor/) { get; set; } | Ottiene e imposta l'oggetto di primo piano [`CellsColor`](../../aspose.cells/cellscolor/). |
| [ForegroundColor](../../aspose.cells.drawing/patternfill/foregroundcolor/) { get; set; } | Ottiene o imposta il colore di primo piano. |
| [ForeTransparency](../../aspose.cells.drawing/patternfill/foretransparency/) { get; set; } | Ottiene o imposta la trasparenza del colore di primo piano. |
| [Pattern](../../aspose.cells.drawing/patternfill/pattern/) { get; set; } | Ottiene o imposta il tipo di pattern di riempimento |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Ereditato da [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Ottiene il codice hash.(Ereditato da [`Fill`](../fill/).) |

### Esempi

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

            // Crea uno stile per la cella usando il pattern BackgroundType
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.DiagonalStripe;
            style.ForegroundColor = Color.LightBlue;
            style.BackgroundColor = Color.DarkBlue;

            worksheet.Cells["B2"].SetStyle(style);
            worksheet.Cells["B2"].PutValue("PatternFill Demo");

            // Crea forma e configura il suo riempimento a motivo
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

### Vedi anche

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


