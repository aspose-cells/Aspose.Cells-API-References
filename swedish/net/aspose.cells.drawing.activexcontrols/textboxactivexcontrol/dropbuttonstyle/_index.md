---
title: "TextBoxActiveXControl.DropButtonStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxActiveXControl egenskap. Anger symbolen som visas på rullknappen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/dropbuttonstyle/
---
## TextBoxActiveXControl.DropButtonStyle property

Anger symbolen som visas på nedrullningsknappen

```csharp
public DropButtonStyle DropButtonStyle { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyDropButtonStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en TextBox ActiveX Control
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.TextBox, 1, 1, 100, 50, 100, 50);
            ActiveXControl control = shape.ActiveXControl;
            
            // Kasta till TextBoxActiveXControl för att komma åt TextBox-specifika egenskaper
            TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)control;
            
            // Ställ in DropButtonStyle-egenskapen
            textBoxControl.DropButtonStyle = DropButtonStyle.Arrow;
            
            // Spara arbetsboken
            workbook.Save("TextBoxActiveXControlDropButtonStyleDemo.xlsx");
        }
    }
}
```

### Se även

* enum [DropButtonStyle](../../dropbuttonstyle/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


