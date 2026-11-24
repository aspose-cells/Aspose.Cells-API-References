---
title: "TextBoxActiveXControl.TabKeyBehavior"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextBoxActiveXControl-Eigenschaft. Gibt an, ob Tabulatorzeichen im Text des Steuerelements erlaubt sind"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/tabkeybehavior/
---
## TextBoxActiveXControl.TabKeyBehavior property

Gibt an, ob Tabulatorzeichen im Text des Steuerelements erlaubt sind.

```csharp
public bool TabKeyBehavior { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyTabKeyBehaviorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein TextBox ActiveX-Steuerelement hinzu und erhalten Sie dessen ActiveXControl-Eigenschaft
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 100, 50);
            var textBoxControl = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Demonstrieren Sie die TabKeyBehavior-Eigenschaft
            Console.WriteLine("Initial TabKeyBehavior: " + textBoxControl.TabKeyBehavior);
            
            // Aktivieren Sie TabKeyBehavior
            if (!textBoxControl.TabKeyBehavior)
            {
                textBoxControl.TabKeyBehavior = true;
                Console.WriteLine("TabKeyBehavior after setting to true: " + textBoxControl.TabKeyBehavior);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("TextBoxActiveXControlTabKeyBehaviorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


