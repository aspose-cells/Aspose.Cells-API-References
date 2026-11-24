---
title: "TextBoxActiveXControl.EnterFieldBehavior"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextBoxActiveXControl-Eigenschaft. Gibt das Auswahlverhalten beim Betreten des Steuerelements an. True bedeutet, dass die Auswahl seit dem letzten Aktivieren des Steuerelements unverändert bleibt. False bedeutet, dass beim Betreten des Steuerelements der gesamte Text ausgewählt wird."
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/enterfieldbehavior/
---
## TextBoxActiveXControl.EnterFieldBehavior property

Gibt das Auswahlverhalten beim Betreten des Steuerelements an. True gibt an, dass die Auswahl unverändert bleibt seit dem letzten Mal, als das Steuerelement aktiv war. False gibt an, dass beim Betreten des Steuerelements der gesamte Text im Steuerelement ausgewählt wird.

```csharp
public bool EnterFieldBehavior { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyEnterFieldBehaviorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein TextBox ActiveX-Steuerelement mit korrekten Parametern hinzu
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 
                1, 1, 1, 1, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Demonstrieren Sie die EnterFieldBehavior-Eigenschaft
            Console.WriteLine("Initial EnterFieldBehavior: " + textBox.EnterFieldBehavior);
            
            // Schalten Sie die EnterFieldBehavior-Eigenschaft um
            textBox.EnterFieldBehavior = !textBox.EnterFieldBehavior;
            Console.WriteLine("Toggled EnterFieldBehavior: " + textBox.EnterFieldBehavior);

            // Setzen Sie EnterFieldBehavior explizit auf true
            textBox.EnterFieldBehavior = true;
            Console.WriteLine("Final EnterFieldBehavior: " + textBox.EnterFieldBehavior);
        }
    }
}
```

### Siehe auch

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


