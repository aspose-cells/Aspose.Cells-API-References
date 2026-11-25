---
title: "Shape.SoftEdges"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene e imposta il raggio della sfocatura da applicare ai bordi in unità di punti"
type: docs
url: /it/net/aspose.cells.drawing/shape/softedges/
---
## Shape.SoftEdges property

Ottiene e imposta il raggio di sfocatura da applicare ai bordi, in unità di punti.

```csharp
public double SoftEdges { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertySoftEdgesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare con i parametri corretti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Imposta l'effetto bordi morbidi con raggio di 5 punti (0.5d = 5 punti)
            shape.SoftEdges = 0.5d;

            // Salva la cartella di lavoro
            workbook.Save("SoftEdgesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


