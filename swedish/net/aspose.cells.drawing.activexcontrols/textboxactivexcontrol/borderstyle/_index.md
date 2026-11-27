---
title: "TextBoxActiveXControl.BorderStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxActiveXControl egenskap. Hämtar och anger typen av ram som används av kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/borderstyle/
---
## TextBoxActiveXControl.BorderStyle property

Hämtar och anger typen av ram som används av kontrollen.

```csharp
public ControlBorderType BorderStyle { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyBorderStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ActiveX TextBox-kontroll
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 1, 1, 1, 100, 100, 0);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;

            // Ställ in BorderStyle-egenskapen
            textBox.BorderStyle = ControlBorderType.Single;

            // Spara arbetsboken
            workbook.Save("TextBoxActiveXControlBorderStyleDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ControlBorderType](../../controlbordertype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


