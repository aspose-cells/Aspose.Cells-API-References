---
title: "GradientFill.FillType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GradientFill property. Gibt den Gradient-Fülltyp zurück"
type: docs
url: /de/net/aspose.cells.drawing/gradientfill/filltype/
---
## GradientFill.FillType property

Liest den Verlauf-Fülltyp.

```csharp
public GradientFillType FillType { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Form mit Gradientfüllung
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            FillFormat fillFormat = shape.Fill;
            fillFormat.FillType = FillType.Gradient;
            
            // Gradienteigenschaften festlegen
            GradientFill gradientFill = fillFormat.GradientFill;
            gradientFill.SetTwoColorGradient(System.Drawing.Color.Red, System.Drawing.Color.Blue, GradientStyleType.Horizontal, 1);
            
            // Zeige den Gradient-Fülltyp an
            Console.WriteLine("Gradient Fill Type: " + gradientFill.FillType);
            
            // Wechsel zu radialem Farbverlauf
            gradientFill.SetGradient(GradientFillType.Radial, 45, GradientDirectionType.FromCenter);
            Console.WriteLine("Updated Gradient Fill Type: " + gradientFill.FillType);
            
            // Speichere die Arbeitsmappe
            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [GradientFillType](../../gradientfilltype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


