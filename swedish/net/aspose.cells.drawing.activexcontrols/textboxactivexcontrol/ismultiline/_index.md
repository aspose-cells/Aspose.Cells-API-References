---
title: "TextBoxActiveXControl.IsMultiLine"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxActiveXControl-egenskap. Anger om kontrollen kan visa mer än en rad text"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/ismultiline/
---
## TextBoxActiveXControl.IsMultiLine property

Indikerar om kontrollen kan visa mer än en textrad.

```csharp
public bool IsMultiLine { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en TextBox ActiveX-kontroll
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 
                1, 1, 200, 100, 0, 0);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Demonstrera egenskapen IsMultiLine
            if (!textBox.IsMultiLine)
            {
                textBox.IsMultiLine = true;
                textBox.Text = "This is a multi-line text box.\nSecond line of text.";
            }

            // Spara arbetsboken
            workbook.Save("TextBoxActiveXControlIsMultiLineDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


