---
title: "TextBoxActiveXControl.IsMultiLine"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxActiveXControl. Indica se il controllo può visualizzare più di una riga di testo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/ismultiline/
---
## TextBoxActiveXControl.IsMultiLine property

Indica se il controllo può visualizzare più di una riga di testo.

```csharp
public bool IsMultiLine { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIsMultiLineDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX TextBox
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 
                1, 1, 200, 100, 0, 0);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Dimostra la proprietà IsMultiLine
            if (!textBox.IsMultiLine)
            {
                textBox.IsMultiLine = true;
                textBox.Text = "This is a multi-line text box.\nSecond line of text.";
            }

            // Salva la cartella di lavoro
            workbook.Save("TextBoxActiveXControlIsMultiLineDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


