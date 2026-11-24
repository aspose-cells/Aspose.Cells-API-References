---
title: "Worksheet.TextBoxes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt eine TextBox-Sammlung zurück"
type: docs
url: /de/net/aspose.cells/worksheet/textboxes/
---
## Worksheet.TextBoxes property

Gibt eine [`TextBox`](../../../aspose.cells.drawing/textbox/) Sammlung zurück.

```csharp
public TextBoxCollection TextBoxes { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Füge ein Textfeld zum Arbeitsblatt hinzu
            int tID = ws.TextBoxes.Add(1, 1, 500, 1000);
            Aspose.Cells.Drawing.TextBox textBox = ws.TextBoxes[tID];

            // Legen Sie Text fest und formatieren Sie Teile davon
            textBox.Text = "Red text 1. Plain text 1. Red text 2. Plain text 2.";
            textBox.Characters(0, 10).Font.Color = Color.Red;
            textBox.Characters(26, 10).Font.Color = Color.DarkRed;

            // Speichere die Arbeitsmappe
            wb.Save("TextBoxExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextBoxCollection](../../../aspose.cells.drawing/textboxcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


