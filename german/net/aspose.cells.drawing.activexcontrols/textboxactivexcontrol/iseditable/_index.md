---
title: "TextBoxActiveXControl.IsEditable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextBoxActiveXControl-Eigenschaft. Gibt an, ob der Benutzer in das Steuerelement tippen kann."
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/iseditable/
---
## TextBoxActiveXControl.IsEditable property

Gibt an, ob der Benutzer in das Steuerelement tippen kann.

```csharp
public bool IsEditable { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIsEditableDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein TextBox‑ActiveX‑Steuerelement hinzufügen
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 
                1, 1, 100, 50, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Demonstrieren Sie die IsEditable-Eigenschaft
            Console.WriteLine("Initial IsEditable: " + textBox.IsEditable);
            
            // Schalten Sie die IsEditable-Eigenschaft um
            textBox.IsEditable = !textBox.IsEditable;
            Console.WriteLine("After toggle IsEditable: " + textBox.IsEditable);

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


