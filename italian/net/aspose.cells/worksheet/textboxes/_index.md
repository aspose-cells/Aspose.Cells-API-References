---
title: "Worksheet.TextBoxes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Ottiene una raccolta di TextBox"
type: docs
url: /it/net/aspose.cells/worksheet/textboxes/
---
## Worksheet.TextBoxes property

Ottiene una raccolta di [`TextBox`](../../../aspose.cells.drawing/textbox/).

```csharp
public TextBoxCollection TextBoxes { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro
            int tID = ws.TextBoxes.Add(1, 1, 500, 1000);
            Aspose.Cells.Drawing.TextBox textBox = ws.TextBoxes[tID];

            // Imposta il testo e formatta le sue parti
            textBox.Text = "Red text 1. Plain text 1. Red text 2. Plain text 2.";
            textBox.Characters(0, 10).Font.Color = Color.Red;
            textBox.Characters(26, 10).Font.Color = Color.DarkRed;

            // Salva la cartella di lavoro
            wb.Save("TextBoxExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextBoxCollection](../../../aspose.cells.drawing/textboxcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


