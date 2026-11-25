---
title: "GradientFill.FillType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà GradientFill. Restituisce il tipo di riempimento gradiente"
type: docs
url: /it/net/aspose.cells.drawing/gradientfill/filltype/
---
## GradientFill.FillType property

Ottiene il tipo di riempimento a gradiente.

```csharp
public GradientFillType FillType { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillPropertyFillTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una forma con riempimento gradiente
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            FillFormat fillFormat = shape.Fill;
            fillFormat.FillType = FillType.Gradient;
            
            // Imposta le proprietà del gradiente
            GradientFill gradientFill = fillFormat.GradientFill;
            gradientFill.SetTwoColorGradient(System.Drawing.Color.Red, System.Drawing.Color.Blue, GradientStyleType.Horizontal, 1);
            
            // Visualizza il tipo di riempimento gradiente
            Console.WriteLine("Gradient Fill Type: " + gradientFill.FillType);
            
            // Passa a gradiente radiale
            gradientFill.SetGradient(GradientFillType.Radial, 45, GradientDirectionType.FromCenter);
            Console.WriteLine("Updated Gradient Fill Type: " + gradientFill.FillType);
            
            // Salva la cartella di lavoro
            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [GradientFillType](../../gradientfilltype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


