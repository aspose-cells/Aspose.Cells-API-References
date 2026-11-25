---
title: "PatternFill.BackTransparency"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PatternFill. Ottiene o imposta la trasparenza del colore di sfondo"
type: docs
url: /it/net/aspose.cells.drawing/patternfill/backtransparency/
---
## PatternFill.BackTransparency property

Ottiene o imposta la trasparenza del colore di sfondo.

```csharp
public double BackTransparency { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyBackTransparencyDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare al foglio di lavoro
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);

            // Ottieni l'istanza PatternFill esistente dalla forma e configura le proprietà
            shape.Fill.FillType = FillType.Pattern;
            PatternFill patternFill = shape.Fill.PatternFill;
            patternFill.Pattern = FillPattern.Solid;
            patternFill.BackgroundColor = Color.Blue;

            // Visualizza il valore iniziale di BackTransparency
            Console.WriteLine("Current BackTransparency value: " + patternFill.BackTransparency);

            // Imposta un nuovo valore di BackTransparency (trasparenza del 50%)
            patternFill.BackTransparency = 0.5;

            // Salva la cartella di lavoro modificata
            workbook.Save("PatternFillBackTransparencyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


