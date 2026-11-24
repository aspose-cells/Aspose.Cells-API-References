---
title: "TextBoxActiveXControl.MaxLength"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextBoxActiveXControl-Eigenschaft. Gibt die maximale Anzahl von Zeichen zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/maxlength/
---
## TextBoxActiveXControl.MaxLength property

Liest und schreibt die maximale Anzahl von Zeichen

```csharp
public int MaxLength { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyMaxLengthDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein TextBox ActiveX-Steuerelement hinzu und erhalten Sie dessen ActiveXControl-Eigenschaft
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 200, 100);
            var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Setzen Sie die MaxLength-Eigenschaft
            if (textBox.MaxLength == 0)
            {
                textBox.MaxLength = 30;
            }

            // Speichere die Arbeitsmappe
            workbook.Save("TextBoxMaxLengthDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


