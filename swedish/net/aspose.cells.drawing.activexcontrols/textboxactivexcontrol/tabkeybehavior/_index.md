---
title: "TextBoxActiveXControl.TabKeyBehavior"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxActiveXControl-egenskap. Anger om tabulatortecken är tillåtna i kontrollens text"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/tabkeybehavior/
---
## TextBoxActiveXControl.TabKeyBehavior property

Indikerar om tabbtecken är tillåtna i kontrollens text.

```csharp
public bool TabKeyBehavior { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyTabKeyBehaviorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en TextBox ActiveX Control och hämta dess ActiveXControl-egenskap
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 100, 50);
            var textBoxControl = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Demonstrera egenskapen TabKeyBehavior
            Console.WriteLine("Initial TabKeyBehavior: " + textBoxControl.TabKeyBehavior);
            
            // Aktivera TabKeyBehavior
            if (!textBoxControl.TabKeyBehavior)
            {
                textBoxControl.TabKeyBehavior = true;
                Console.WriteLine("TabKeyBehavior after setting to true: " + textBoxControl.TabKeyBehavior);
            }

            // Spara arbetsboken
            workbook.Save("TextBoxActiveXControlTabKeyBehaviorDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


