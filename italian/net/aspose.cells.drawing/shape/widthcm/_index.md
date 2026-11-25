---
title: "Shape.WidthCM"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Rappresenta la larghezza della forma nell'unità di centimetri"
type: docs
url: /it/net/aspose.cells.drawing/shape/widthcm/
---
## Shape.WidthCM property

Rappresenta la larghezza della forma, in unità di centimetri.

```csharp
public double WidthCM { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthCMDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 100, 100);

            // Imposta la larghezza in centimetri
            shape.WidthCM = 3.5;
            Console.WriteLine("Shape width set to: " + shape.WidthCM + " cm");

            // Modifica la larghezza se corrisponde a una condizione
            if (shape.WidthCM == 3.5)
            {
                shape.WidthCM = 2.0;
                Console.WriteLine("Shape width changed to: " + shape.WidthCM + " cm");
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


