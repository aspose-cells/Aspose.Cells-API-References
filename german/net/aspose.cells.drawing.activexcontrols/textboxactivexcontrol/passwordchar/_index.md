---
title: "TextBoxActiveXControl.PasswordChar"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextBoxActiveXControl-Eigenschaft. Gibt ein Zeichen zurück und legt es fest, das anstelle der eingegebenen Zeichen angezeigt wird"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/passwordchar/
---
## TextBoxActiveXControl.PasswordChar property

Liest und setzt ein Zeichen, das anstelle der eingegebenen Zeichen angezeigt wird.

```csharp
public char PasswordChar { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyPasswordCharDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein TextBox ActiveX Control hinzu und erhalten Sie dessen Form
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 0, 1, 1, 100, 50);
            
            // Holen Sie das TextBoxActiveXControl aus der Form
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBoxControl = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Setzen Sie die PasswordChar-Eigenschaft
            textBoxControl.PasswordChar = '*';

            // Setzen Sie einen Text, um die Passwortmaskierung zu demonstrieren
            textBoxControl.Text = "password123";

            // Speichere die Arbeitsmappe
            workbook.Save("TextBoxActiveXControlPasswordCharDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


