---
title: "Shape.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Restituisce il tipo di forma automatica"
type: docs
url: /it/net/aspose.cells.drawing/shape/type/
---
## Shape.Type property

Ottiene il tipo di forma automatica.

```csharp
public AutoShapeType Type { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare con i parametri corretti
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 1, 1, 100, 150, 0, 0);

            // Ottieni e visualizza il tipo di forma
            AutoShapeType autoShapeType = shape.Type;
            Console.WriteLine("Shape Type: " + autoShapeType);

            // Impossibile modificare il tipo di forma poiché la proprietà Type è di sola lettura
            // Invece crea una nuova forma con un tipo diverso
            Shape ovalShape = worksheet.Shapes.AddAutoShape(AutoShapeType.Oval, 1, 1, 100, 150, 0, 0);
            Console.WriteLine("New Shape Type: " + ovalShape.Type);
        }
    }
}
```

### Vedi anche

* enum [AutoShapeType](../../autoshapetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


