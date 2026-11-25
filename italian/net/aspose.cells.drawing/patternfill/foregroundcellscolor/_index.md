---
title: "PatternFill.ForegroundCellsColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PatternFill. Ottiene e imposta l'oggetto CellsColor di primo piano"
type: docs
url: /it/net/aspose.cells.drawing/patternfill/foregroundcellscolor/
---
## PatternFill.ForegroundCellsColor property

Ottiene e imposta l'oggetto [`CellsColor`](../../../aspose.cells/cellscolor/) di primo piano.

```csharp
public CellsColor ForegroundCellsColor { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyForegroundCellsColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare per dimostrare il riempimento a pattern
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            try
            {
                // Imposta il tipo di riempimento su pattern
                shape.Fill.FillType = FillType.Pattern;

                // Ottieni l'istanza di PatternFill
                PatternFill patternFill = shape.Fill.PatternFill;

                // Imposta il tipo di pattern e i colori
                patternFill.Pattern = FillPattern.WideDownwardDiagonal;
                patternFill.ForegroundColor = Color.Red;
                patternFill.BackgroundColor = Color.Yellow;

                // Crea un oggetto CellsColor per il primo piano utilizzando la proprietà Color
                // Poiché CellsColor non ha un costruttore pubblico, utilizzeremo il ForegroundCellsColor esistente
                // e modifica direttamente le sue proprietà
                patternFill.ForegroundCellsColor.Color = Color.Blue;
                patternFill.ForegroundCellsColor.Argb = Color.Blue.ToArgb();

                // Visualizza le proprietà di ForegroundCellsColor
                Console.WriteLine("ForegroundCellsColor Type: " + patternFill.ForegroundCellsColor.Type);
                Console.WriteLine("ForegroundCellsColor Color: " + patternFill.ForegroundCellsColor.Color);
                Console.WriteLine("ForegroundCellsColor ARGB: " + patternFill.ForegroundCellsColor.Argb);

                // Salva la cartella di lavoro
                workbook.Save("ForegroundCellsColorDemo.xlsx");
                Console.WriteLine("ForegroundCellsColor demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


