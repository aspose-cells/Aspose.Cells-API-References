---
title: "FillFormat.GradientColor2"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FillFormat-Eigenschaft. Gibt die zweite Farbverlauffarbe für die angegebene Füllung zurück."
type: docs
url: /de/net/aspose.cells.drawing/fillformat/gradientcolor2/
---
## FillFormat.GradientColor2 property

Gibt die Farbverlauffarbe 2 für die angegebene Füllung zurück.

```csharp
public Color GradientColor2 { get; }
```

### Hinweise

Nur wenn der Farbverlauftyp GradientColorType.TwoColors ist, ist diese Eigenschaft sinnvoll.

### Beispiele

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
            
            // Erstelle ein Rechteck-Shape mit zweifarbigem Farbverlauf
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 200);
            FillFormat fill = rectangle.Fill;
            
            fill.SetTwoColorGradient(Color.Red, Color.Blue, GradientStyleType.Horizontal, 2);

            // Überprüfe die Farbverlauf-Eigenschaften
            Console.WriteLine("GradientColor2: " + fill.GradientColor2);
        }
    }
}
```

### Siehe auch

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


