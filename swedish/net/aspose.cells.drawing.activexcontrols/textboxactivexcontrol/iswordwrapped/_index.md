---
title: "TextBoxActiveXControl.IsWordWrapped"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxActiveXControl-egenskap. Anger om innehållet i kontrollen automatiskt radbryts i slutet av en rad"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/iswordwrapped/
---
## TextBoxActiveXControl.IsWordWrapped property

Anger om innehållet i kontrollen automatiskt radbryts i slutet av en rad.

```csharp
public bool IsWordWrapped { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIsWordWrappedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en TextBox ActiveX-kontroll med alla nödvändiga parametrar
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox,
                1, 1, 200, 100, 0, 0);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Ange någon text som skulle ha nytta av radbrytning
            textBox.Text = "This is a long text that should demonstrate word wrapping functionality in the TextBox ActiveX control.";

            // Kontrollera och ange egenskapen IsWordWrapped
            if (!textBox.IsWordWrapped)
            {
                textBox.IsWordWrapped = true;
                Console.WriteLine("Word wrapping has been enabled for the TextBox.");
            }

            // Spara arbetsboken
            workbook.Save("TextBoxWordWrapDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


