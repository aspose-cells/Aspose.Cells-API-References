---
title: "Shape.CreateId"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene e imposta l'ID di creazione per questa forma"
type: docs
url: /it/net/aspose.cells.drawing/shape/createid/
---
## Shape.CreateId property

Ottiene e imposta l'ID di creazione per questa forma.

```csharp
public Guid CreateId { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyCreateIdDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una forma rettangolare
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 200, 150);
            
            // Crea e assegna un nuovo GUID come CreateId
            Guid createId = Guid.NewGuid();
            shape.CreateId = createId;
            
            // Salva la cartella di lavoro
            workbook.Save("ShapeCreateIdDemo.xlsx");
            
            // Ricarica la cartella di lavoro per verificare che il CreateId persista
            Workbook loadedWorkbook = new Workbook("ShapeCreateIdDemo.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Restituisci il CreateId per la verifica
            Console.WriteLine("Original CreateId: " + createId);
            Console.WriteLine("Loaded CreateId: " + loadedShape.CreateId);
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


