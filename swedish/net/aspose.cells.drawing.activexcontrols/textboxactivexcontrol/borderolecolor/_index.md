---
title: "TextBoxActiveXControl.BorderOleColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxActiveXControl-egenskap. Hämtar och anger OLE-färgen för bakgrunden"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/borderolecolor/
---
## TextBoxActiveXControl.BorderOleColor property

Hämtar och anger ole-färgen för bakgrunden.

```csharp
public int BorderOleColor { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyBorderOleColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ActiveX TextBox-kontroll och hämta dess ActiveXControl-egenskap
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 100, 100, 100, 100);
            var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Ange egenskapen BorderOleColor (Excels standardfärgsystem 12 eller grön)
            textBox.BorderOleColor = unchecked((int)0x80000012);

            // Spara arbetsboken
            workbook.Save("TextBoxActiveXControlBorderOleColorDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


