---
title: "TextBoxActiveXControl.IsAutoTab"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextBoxActiveXControl-Eigenschaft. Gibt an, ob der Fokus automatisch zum nächsten Steuerelement wechselt, wenn der Benutzer die maximale Zeichenanzahl eingibt"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/isautotab/
---
## TextBoxActiveXControl.IsAutoTab property

Gibt an, ob der Fokus automatisch zum nächsten Steuerelement wechselt, wenn der Benutzer die maximale Zeichenanzahl eingibt.

```csharp
public bool IsAutoTab { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIsAutoTabDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein TextBox-ActiveX-Steuerelement hinzufügen und sein Steuerelement abrufen
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 100, 30, 100, 30);
            var textBoxControl = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Die IsAutoTab-Eigenschaft demonstrieren
            Console.WriteLine("Initial IsAutoTab value: " + textBoxControl.IsAutoTab);
            
            // Setze IsAutoTab auf true, wenn es false ist
            if (!textBoxControl.IsAutoTab)
            {
                textBoxControl.IsAutoTab = true;
                Console.WriteLine("IsAutoTab set to: " + textBoxControl.IsAutoTab);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("TextBoxActiveXControlIsAutoTabDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


