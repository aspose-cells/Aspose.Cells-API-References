---
title: "Shape.HeightCM"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Rappresenta l'altezza della forma in unità di centimetri"
type: docs
url: /it/net/aspose.cells.drawing/shape/heightcm/
---
## Shape.HeightCM property

Rappresenta l'altezza della forma, in unità di centimetri.

```csharp
public double HeightCM { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightCMDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Imposta l'altezza in centimetri
            shape.HeightCM = 3;
            Console.WriteLine("Shape height: " + shape.HeightCM + " cm");

            // Modifica l'altezza se è 3 cm
            if (shape.HeightCM == 3)
            {
                shape.HeightCM = 1;
                Console.WriteLine("Modified shape height: " + shape.HeightCM + " cm");
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


