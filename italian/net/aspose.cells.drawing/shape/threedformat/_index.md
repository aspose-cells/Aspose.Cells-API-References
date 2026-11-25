---
title: "Shape.ThreeDFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene e imposta il formato 3D della forma"
type: docs
url: /it/net/aspose.cells.drawing/shape/threedformat/
---
## Shape.ThreeDFormat property

Ottiene e imposta il formato 3D della forma.

```csharp
public ThreeDFormat ThreeDFormat { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyThreeDFormatDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma di esempio con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 100);

            // Accedi e modifica le proprietà del formato 3D
            ThreeDFormat threeDFormat = shape.ThreeDFormat;
            threeDFormat.ExtrusionColor.Color = System.Drawing.Color.Blue;
            threeDFormat.LightAngle = 45;
            threeDFormat.ContourWidth = 2;
            threeDFormat.ContourColor.Color = System.Drawing.Color.Red;

            // Salva la cartella di lavoro
            workbook.Save("ThreeDFormatDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ThreeDFormat](../../threedformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


