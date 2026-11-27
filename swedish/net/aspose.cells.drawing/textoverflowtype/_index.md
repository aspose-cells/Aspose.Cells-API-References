---
title: "Enum TextOverflowType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.TextOverflowType‑enum. Representerar hur texten överflödar vertikalt eller horisontellt"
type: docs
url: /sv/net/aspose.cells.drawing/textoverflowtype/
---
## TextOverflowType enumeration

Representerar hur texten överflödar vertikalt eller horisontellt.

```csharp
public enum TextOverflowType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Clip | `0` | Var uppmärksam på övre och nedre barriärer. Ge ingen indikation på att det finns text som inte är synlig. |
| Ellipsis | `1` | Var uppmärksam på övre och nedre barriärer. Använd en ellips för att ange att det finns text som inte är synlig. Endast för vertikalt överflöde. |
| Overflow | `2` | Överflöda texten och ignorera övre och nedre barriärer. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DrawingClassTextOverflowTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Lägg till en textruta i diagrammet
            TextBox textBox = chart.Shapes.AddTextBoxInChart(10, 10, 200, 50);

            // Ställ in textrutans egenskaper
            textBox.TextBody.TextAlignment.AutoSize = false;
            textBox.Text = "This is a long text that will demonstrate text overflow handling";
            
            // Ställ in typ av textöverspill
            textBox.TextVerticalOverflow = TextOverflowType.Clip;

            // Spara arbetsboken
            workbook.Save("TextOverflowTypeDemo_out.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


