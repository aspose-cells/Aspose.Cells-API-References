---
title: "TextBoxActiveXControl.HideSelection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxActiveXControl-egenskap. Anger om markerad text i kontrollen visas markerad när kontrollen inte har fokus"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/hideselection/
---
## TextBoxActiveXControl.HideSelection property

Indikerar om markerad text i kontrollen visas markerad när kontrollen inte har fokus.

```csharp
public bool HideSelection { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyHideSelectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ActiveX TextBox-kontroll i kalkylbladet
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 100, 50);
            var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Demonstrera HideSelection property
            Console.WriteLine("Initial HideSelection value: " + textBox.HideSelection);
            
            // Ställ in HideSelection till true om den är false
            if (!textBox.HideSelection)
            {
                textBox.HideSelection = true;
                Console.WriteLine("HideSelection set to: " + textBox.HideSelection);
            }

            // Spara arbetsboken
            workbook.Save("TextBoxActiveXControlHideSelectionDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


