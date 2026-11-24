---
title: "Enum FillType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.FillType Enum. Füllformattyp"
type: docs
url: /de/net/aspose.cells.drawing/filltype/
---
## FillType enumeration

Füllformattyp.

```csharp
public enum FillType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Automatic | `0` | Stellt den automatischen Formatierungstyp dar. |
| None | `1` | Stellt den Formatierungstyp "keine" dar. |
| Solid | `2` | Solides Füllformat. |
| Gradient | `3` | Verlaufs‑Füllformat. |
| Texture | `4` | Texturfüllformat (einschließlich Bildfüllung). |
| Pattern | `5` | Muster‑Füllformat. |
| Group | `6` | Erbt die Fülleigenschaften der Gruppe. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rechteckform hinzufügen
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 150);
            
            // Setze den Typ der Farbverlauffüllung
            rectangle.Fill.FillType = FillType.Gradient;
            rectangle.Fill.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 1);

            // Füge ein Textfeld hinzu
            Shape textBox = worksheet.Shapes.AddTextBox(1, 0, 10, 10, 100, 150);
            textBox.Text = "Gradient Fill Example";
            
            // Lege den Verlauffülltyp für das Textfeld fest
            textBox.Fill.FillType = FillType.Gradient;
            textBox.Fill.SetTwoColorGradient(Color.LightGreen, Color.DarkGreen, GradientStyleType.Vertical, 1);

            // Speichere die Arbeitsmappe
            workbook.Save("FillTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


