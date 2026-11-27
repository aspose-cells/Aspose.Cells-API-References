---
title: "Enum FillType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.FillType-enum. Fyllformatstyp"
type: docs
url: /sv/net/aspose.cells.drawing/filltype/
---
## FillType enumeration

Fyllningsformattyp.

```csharp
public enum FillType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Automatic | `0` | Representerar automatisk formateringstyp. |
| None | `1` | Representerar ingen formateringstyp. |
| Solid | `2` | Solid fyllformat. |
| Gradient | `3` | Gradientfyllningsformat. |
| Texture | `4` | Texturfyllformat(inkluderar bildfyllning). |
| Pattern | `5` | Mönsterfyllningsformat. |
| Group | `6` | Ärv fyllnadsegenskaperna från gruppen. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassFillTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 150);
            
            // Ställ in gradientfyllningstyp
            rectangle.Fill.FillType = FillType.Gradient;
            rectangle.Fill.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 1);

            // Lägg till en textruta
            Shape textBox = worksheet.Shapes.AddTextBox(1, 0, 10, 10, 100, 150);
            textBox.Text = "Gradient Fill Example";
            
            // Ange gradientfyllnadstyp för textrutan
            textBox.Fill.FillType = FillType.Gradient;
            textBox.Fill.SetTwoColorGradient(Color.LightGreen, Color.DarkGreen, GradientStyleType.Vertical, 1);

            // Spara arbetsboken
            workbook.Save("FillTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


