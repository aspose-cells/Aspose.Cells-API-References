---
title: "FillFormat.FillType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FillFormat. Ottiene e imposta il tipo di riempimento."
type: docs
url: /it/net/aspose.cells.drawing/fillformat/filltype/
---
## FillFormat.FillType property

Ottiene e imposta il tipo di riempimento

```csharp
public FillType FillType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyFillTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Imposta un riempimento solido con colore.
            shape.Fill.FillType = FillType.Solid;
            shape.Fill.SolidFill.Color = System.Drawing.Color.Red;

            // Restituisci il tipo di riempimento.
            Console.WriteLine("Shape fill type: " + shape.Fill.FillType);

            // Cambia a riempimento gradiente.
            shape.Fill.FillType = FillType.Gradient;
            Console.WriteLine("Shape fill type changed to: " + shape.Fill.FillType);

            // Salva la cartella di lavoro
            workbook.Save("FillTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [FillType](../../filltype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


