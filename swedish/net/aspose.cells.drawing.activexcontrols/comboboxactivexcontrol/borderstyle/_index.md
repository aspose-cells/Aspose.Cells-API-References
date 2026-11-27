---
title: "ComboBoxActiveXControl.BorderStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ComboBoxActiveXControl-egenskap. Hämtar och anger typen av ram som används av kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/borderstyle/
---
## ComboBoxActiveXControl.BorderStyle property

Hämtar och anger typen av ram som används av kontrollen.

```csharp
public ControlBorderType BorderStyle { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyBorderStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Demonstrera egenskapen BorderStyle
            comboBox.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.Single;
            comboBox.BorderOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Black);

            // Ställ in grundläggande egenskaper för funktionalitet
            comboBox.ListRows = 5;
            comboBox.Value = "Sample Text";

            workbook.Save("ComboBoxBorderStyleDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ControlBorderType](../../controlbordertype/)
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


