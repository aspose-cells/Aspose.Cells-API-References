---
title: "Shape.Id"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene l'identificatore di questa forma"
type: docs
url: /it/net/aspose.cells.drawing/shape/id/
---
## Shape.Id property

Ottiene l'identificatore di questa forma.

```csharp
public int Id { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIdDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma al foglio di lavoro
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Ottieni e visualizza l'ID della forma
            int id = shape.Id;
            Console.WriteLine("Shape ID: " + id);

            // Modifica le proprietà della forma
            shape.Name = "Rectangle1";
            shape.Text = "Shape with ID: " + id;

            // Salva la cartella di lavoro
            workbook.Save("ShapePropertyIdDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


