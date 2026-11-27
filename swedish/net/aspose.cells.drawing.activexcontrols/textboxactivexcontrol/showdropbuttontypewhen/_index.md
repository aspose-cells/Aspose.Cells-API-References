---
title: "TextBoxActiveXControl.ShowDropButtonTypeWhen"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxActiveXControl egenskap. Anger symbolen som visas på rullknappen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/showdropbuttontypewhen/
---
## TextBoxActiveXControl.ShowDropButtonTypeWhen property

Anger symbolen som visas på nedrullningsknappen

```csharp
public ShowDropButtonType ShowDropButtonTypeWhen { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyShowDropButtonTypeWhenDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ActiveX TextBox-kontroll
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.TextBox, 
                1, 1, 1, 1, 100, 50);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;

            // Ställ in egenskapen ShowDropButtonTypeWhen
            textBox.ShowDropButtonTypeWhen = ShowDropButtonType.Focus;

            // Spara arbetsboken
            workbook.Save("TextBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ShowDropButtonType](../../showdropbuttontype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


