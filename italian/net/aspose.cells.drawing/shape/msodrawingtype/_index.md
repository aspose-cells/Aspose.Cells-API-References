---
title: "Shape.MsoDrawingType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene il tipo di disegno"
type: docs
url: /it/net/aspose.cells.drawing/shape/msodrawingtype/
---
## Shape.MsoDrawingType property

Ottiene il tipo di disegno.

```csharp
public MsoDrawingType MsoDrawingType { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyMsoDrawingTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare (parametri corretti)
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);
            
            // Ottieni e visualizza il MsoDrawingType della forma
            MsoDrawingType drawingType = rectangle.MsoDrawingType;
            Console.WriteLine("Shape MsoDrawingType: " + drawingType.ToString());

            // Aggiungi una forma di linea (parametri corretti)
            Shape line = worksheet.Shapes.AddLine(3, 0, 3, 100, 150, 1);
            
            // Ottieni e visualizza il MsoDrawingType della linea
            drawingType = line.MsoDrawingType;
            Console.WriteLine("Line MsoDrawingType: " + drawingType.ToString());
        }
    }
}
```

### Vedi anche

* enum [MsoDrawingType](../../msodrawingtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


