---
title: "MsoFillFormat.SetOneColorGradient"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoFillFormat-Methode. Setzt die angegebene Füllung auf einen Einfarbverlauf"
type: docs
url: /de/net/aspose.cells.drawing/msofillformat/setonecolorgradient/
---
## MsoFillFormat.SetOneColorGradient method

Setzt die angegebene Füllung auf einen Einfarbverlauf.

```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Farbe | Farbe | Eine Gradientfarbe. |
| Grad | Double | Der Grad des Farbverlaufs. Kann ein Wert von 0.0 (dunkel) bis 1.0 (hell) sein. |
| Stil | GradientStyleType | Gradient-Schattierungsstil. |
| Variante | Int32 | Die Gradientvariante. Kann einen Wert von 1 bis 4 haben, der einer der vier Varianten auf der Registerkarte Gradient im Dialogfeld Fill Effects entspricht. Wenn style GradientStyle.FromCenter ist, kann das Variant-Argument nur 1 oder 2 sein. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatMethodSetOneColorGradientWithColorDoubleGradientStyleTypeInDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 50, 50);
            MsoFillFormat fillFormat = shape.FillFormat;

            // Einfarbverlauf mit angegebenen Parametern festlegen
            fillFormat.SetOneColorGradient(Color.Red, 0.5, GradientStyleType.DiagonalUp, 2);

            workbook.Save("GradientFillExample.xlsx");
        }
    }
}
```

### Siehe auch

* enum [GradientStyleType](../../gradientstyletype/)
* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


