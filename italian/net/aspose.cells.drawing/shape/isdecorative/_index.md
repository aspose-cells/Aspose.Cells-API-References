---
title: "Shape.IsDecorative"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Indica se l'oggetto è decorativo"
type: docs
url: /it/net/aspose.cells.drawing/shape/isdecorative/
---
## Shape.IsDecorative property

Indica se l'oggetto è decorativo.

```csharp
public bool IsDecorative { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsDecorativeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una forma rettangolare
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
            
            // Imposta la forma come decorativa
            shape.IsDecorative = true;
            
            // Salva la cartella di lavoro
            string outputPath = "ShapeIsDecorativeDemo.xlsx";
            workbook.Save(outputPath);
            
            // Ricarica la cartella di lavoro per verificare la proprietà
            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Restituisci il risultato
            Console.WriteLine("Shape IsDecorative property: " + loadedShape.IsDecorative);
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


