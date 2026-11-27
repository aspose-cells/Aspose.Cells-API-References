---
title: "TextBoxActiveXControl.MaxLength"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxActiveXControl-egenskap. Hämtar och anger det maximala antalet tecken"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/maxlength/
---
## TextBoxActiveXControl.MaxLength property

Hämtar och anger det maximala antalet tecken

```csharp
public int MaxLength { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyMaxLengthDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en TextBox ActiveX Control och hämta dess ActiveXControl-egenskap
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 1, 1, 200, 100);
            var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Ställ in MaxLength-egenskapen
            if (textBox.MaxLength == 0)
            {
                textBox.MaxLength = 30;
            }

            // Spara arbetsboken
            workbook.Save("TextBoxMaxLengthDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


