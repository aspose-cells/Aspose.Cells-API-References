---
title: "Shape.AutoShapeType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene e imposta il tipo di forma automatica"
type: docs
url: /it/net/aspose.cells.drawing/shape/autoshapetype/
---
## Shape.AutoShapeType property

Ottiene e imposta il tipo di forma automatica.

```csharp
public AutoShapeType AutoShapeType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyAutoShapeTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma al foglio di lavoro con i parametri corretti.
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 1, 1, 100, 150, 0, 0);

            // Verifica e modifica l'AutoShapeType se necessario
            if (shape.AutoShapeType == AutoShapeType.Unknown)
            {
                shape.AutoShapeType = AutoShapeType.Rectangle;
            }

            // Modifica il tipo di forma per dimostrare la proprietà
            shape.AutoShapeType = AutoShapeType.Oval;

            // Salva la cartella di lavoro
            workbook.Save("ShapePropertyAutoShapeTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [AutoShapeType](../../autoshapetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


