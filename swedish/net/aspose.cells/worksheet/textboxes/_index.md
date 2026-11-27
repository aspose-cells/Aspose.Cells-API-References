---
title: "Worksheet.TextBoxes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Hämtar en TextBox-samling"
type: docs
url: /sv/net/aspose.cells/worksheet/textboxes/
---
## Worksheet.TextBoxes property

Hämtar en [`TextBox`](../../../aspose.cells.drawing/textbox/) samling.

```csharp
public TextBoxCollection TextBoxes { get; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTextBoxesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Lägg till en textruta i kalkylbladet
            int tID = ws.TextBoxes.Add(1, 1, 500, 1000);
            Aspose.Cells.Drawing.TextBox textBox = ws.TextBoxes[tID];

            // Ange text och formatera delar av den
            textBox.Text = "Red text 1. Plain text 1. Red text 2. Plain text 2.";
            textBox.Characters(0, 10).Font.Color = Color.Red;
            textBox.Characters(26, 10).Font.Color = Color.DarkRed;

            // Spara arbetsboken
            wb.Save("TextBoxExample.xlsx");
        }
    }
}
```

### Se även

* class [TextBoxCollection](../../../aspose.cells.drawing/textboxcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


