---
title: "FillFormat.GradientColor2"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FillFormat. Restituisce il colore gradiente 2 per il riempimento specificato"
type: docs
url: /it/net/aspose.cells.drawing/fillformat/gradientcolor2/
---
## FillFormat.GradientColor2 property

Restituisce il colore gradiente 2 per il riempimento specificato.

```csharp
public Color GradientColor2 { get; }
```

### Osservazioni

Solo quando il tipo di colore gradiente è GradientColorType.TwoColors, questa proprietà ha senso.

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientColor2Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea una forma rettangolare con riempimento a gradiente a due colori
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 200);
            FillFormat fill = rectangle.Fill;
            
            fill.SetTwoColorGradient(Color.Red, Color.Blue, GradientStyleType.Horizontal, 2);

            // Verifica le proprietà del colore gradiente
            Console.WriteLine("GradientColor2: " + fill.GradientColor2);
        }
    }
}
```

### Vedi anche

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


