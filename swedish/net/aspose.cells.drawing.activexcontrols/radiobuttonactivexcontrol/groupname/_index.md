---
title: "RadioButtonActiveXControl.GroupName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RadioButtonActiveXControl egenskap. Hämtar och anger gruppens namn"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/groupname/
---
## RadioButtonActiveXControl.GroupName property

Hämtar och anger gruppens namn.

```csharp
public string GroupName { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RadioButtonActiveXControlPropertyGroupNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till två RadioButton ActiveX-kontroller
            var shape1 = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton, 1, 0, 1, 0, 100, 30);
            var radio1 = (Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl)shape1.ActiveXControl;
            
            var shape2 = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton, 1, 0, 1, 50, 100, 30);
            var radio2 = (Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl)shape2.ActiveXControl;

            // Ange samma gruppnamn för att göra dem ömsesidigt uteslutande
            radio1.GroupName = "RadioGroup1";
            radio2.GroupName = "RadioGroup1";

            // Ställ in rubriker
            radio1.Caption = "Option 1";
            radio2.Caption = "Option 2";

            // Spara arbetsboken
            workbook.Save("RadioButtonGroupDemo.xlsx");
        }
    }
}
```

### Se även

* class [RadioButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


