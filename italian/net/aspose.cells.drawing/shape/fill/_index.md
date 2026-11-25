---
title: "Shape.Fill"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Restituisce un oggetto FillFormat che contiene le proprietà di formattazione di riempimento per la forma specificata"
type: docs
url: /it/net/aspose.cells.drawing/shape/fill/
---
## Shape.Fill property

Restituisce un oggetto [`FillFormat`](../fillformat/) che contiene le proprietà di formattazione di riempimento per la forma specificata.

```csharp
public FillFormat Fill { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyFillDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare con i parametri corretti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Ottieni il formato di riempimento della forma
            FillFormat fillFmt = shape.Fill;

            // Imposta un riempimento solido con colore.
            fillFmt.SolidFill.Color = System.Drawing.Color.Red;

            // Imposta la trasparenza
            fillFmt.Transparency = 0.5;

            // Salva la cartella di lavoro
            workbook.Save("ShapeFillDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FillFormat](../../fillformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


