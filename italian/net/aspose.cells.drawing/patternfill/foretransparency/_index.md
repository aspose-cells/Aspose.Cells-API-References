---
title: "PatternFill.ForeTransparency"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PatternFill. Ottiene o imposta la trasparenza del colore di primo piano"
type: docs
url: /it/net/aspose.cells.drawing/patternfill/foretransparency/
---
## PatternFill.ForeTransparency property

Ottiene o imposta la trasparenza del colore di primo piano.

```csharp
public double ForeTransparency { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyForeTransparencyDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare per dimostrare il riempimento a pattern
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            // Imposta il tipo di riempimento su pattern
            shape.Fill.FillType = FillType.Pattern;

            // Ottieni l'istanza di PatternFill
            PatternFill patternFill = shape.Fill.PatternFill;

            // Configura le proprietà di riempimento del pattern
            patternFill.Pattern = FillPattern.Solid;
            patternFill.ForegroundColor = Color.Red;
            patternFill.BackgroundColor = Color.Blue;

            try
            {
                // Visualizza il valore iniziale di ForeTransparency
                Console.WriteLine("Initial ForeTransparency value: " + patternFill.ForeTransparency);

                // Imposta un nuovo valore di ForeTransparency (trasparenza del 50%)
                patternFill.ForeTransparency = 0.5;

                // Visualizza il valore aggiornato di ForeTransparency
                Console.WriteLine("Updated ForeTransparency value: " + patternFill.ForeTransparency);

                // Salva la cartella di lavoro
                workbook.Save("ForeTransparencyDemo.xlsx");
                Console.WriteLine("ForeTransparency demonstration completed successfully.");
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

* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


