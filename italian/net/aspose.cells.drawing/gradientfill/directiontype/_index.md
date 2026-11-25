---
title: "GradientFill.DirectionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà GradientFill. Ottiene il tipo di direzione del gradiente"
type: docs
url: /it/net/aspose.cells.drawing/gradientfill/directiontype/
---
## GradientFill.DirectionType property

Ottiene il tipo di direzione del gradiente.

```csharp
public GradientDirectionType DirectionType { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillPropertyDirectionTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una forma per dimostrare il riempimento gradiente
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 5, 5);

            // Imposta le proprietà del riempimento gradiente
            FillFormat fillFormat = shape.Fill;
            fillFormat.SetTwoColorGradient(System.Drawing.Color.Blue, System.Drawing.Color.LightBlue, GradientStyleType.DiagonalDown, 1);
            fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);

            // Restituisci il tipo di direzione del gradiente
            Console.WriteLine("Gradient Direction Type: " + fillFormat.GradientFill.DirectionType);

            // Salva la cartella di lavoro
            workbook.Save("GradientDirectionTypeExample.xlsx");
        }
    }
}
```

### Vedi anche

* enum [GradientDirectionType](../../gradientdirectiontype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


