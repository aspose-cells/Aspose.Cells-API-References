---
title: "TextBoxActiveXControl.Text"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextBoxActiveXControl-Eigenschaft. Ruft den Text des Steuerelements ab und legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/text/
---
## TextBoxActiveXControl.Text property

Liest und setzt den Text des Steuerelements.

```csharp
public string Text { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyTextDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie ein TextBox ActiveX-Steuerelement zum Arbeitsblatt hinzu
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 200, 100);
            
            // Holen Sie das ActiveX-Steuerelement und setzen Sie dessen Text
            var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;
            textBox.Text = "This is a test.";
            
            // Speichere die Arbeitsmappe
            workbook.Save("TextBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


