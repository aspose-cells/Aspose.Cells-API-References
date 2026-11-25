---
title: "Shape.RotationAngle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene e imposta la rotazione della forma"
type: docs
url: /it/net/aspose.cells.drawing/shape/rotationangle/
---
## Shape.RotationAngle property

Ottiene e imposta la rotazione della shape.

```csharp
public double RotationAngle { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyRotationAngleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 100, 200, 0, 0);

            // Imposta l'angolo di rotazione a 60 gradi
            shape.RotationAngle = 60;
            Console.WriteLine("Shape rotation angle set to: " + shape.RotationAngle);

            // Ottieni l'angolo di rotazione corrente
            double currentAngle = shape.RotationAngle;
            Console.WriteLine("Current shape rotation angle: " + currentAngle);

            // Salva la cartella di lavoro
            workbook.Save("ShapeRotationDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


