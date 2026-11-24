---
title: "TextBoxActiveXControl.IsMultiLine"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextBoxActiveXControl-Eigenschaft. Gibt an, ob das Steuerelement mehr als eine Textzeile anzeigen kann"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/ismultiline/
---
## TextBoxActiveXControl.IsMultiLine property

Gibt an, ob das Steuerelement mehr als eine Textzeile anzeigen kann.

```csharp
public bool IsMultiLine { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein TextBox‑ActiveX‑Steuerelement hinzufügen
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 
                1, 1, 200, 100, 0, 0);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Demonstrieren Sie die IsMultiLine-Eigenschaft
            if (!textBox.IsMultiLine)
            {
                textBox.IsMultiLine = true;
                textBox.Text = "This is a multi-line text box.\nSecond line of text.";
            }

            // Speichere die Arbeitsmappe
            workbook.Save("TextBoxActiveXControlIsMultiLineDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


