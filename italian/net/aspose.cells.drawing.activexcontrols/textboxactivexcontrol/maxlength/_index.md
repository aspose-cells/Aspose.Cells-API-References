---
title: "TextBoxActiveXControl.MaxLength"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxActiveXControl. Ottiene e imposta il numero massimo di caratteri"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/maxlength/
---
## TextBoxActiveXControl.MaxLength property

Ottiene e imposta il numero massimo di caratteri

```csharp
public int MaxLength { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyMaxLengthDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo TextBox ActiveX e ottieni la sua proprietà ActiveXControl
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 200, 100);
            var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Imposta la proprietà MaxLength
            if (textBox.MaxLength == 0)
            {
                textBox.MaxLength = 30;
            }

            // Salva la cartella di lavoro
            workbook.Save("TextBoxMaxLengthDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


