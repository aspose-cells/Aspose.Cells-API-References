---
title: "RadioButtonActiveXControl.GroupName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RadioButtonActiveXControl Eigenschaft. Liest und setzt den Namen der Gruppe"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/groupname/
---
## RadioButtonActiveXControl.GroupName property

Liest und setzt den Namen der Gruppe.

```csharp
public string GroupName { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RadioButtonActiveXControlPropertyGroupNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Zwei RadioButton ActiveX-Steuerelemente hinzufügen
            var shape1 = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton, 1, 0, 1, 0, 100, 30);
            var radio1 = (Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl)shape1.ActiveXControl;
            
            var shape2 = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton, 1, 0, 1, 50, 100, 30);
            var radio2 = (Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl)shape2.ActiveXControl;

            // Setzen Sie denselben Gruppennamen, damit sie sich gegenseitig ausschließen
            radio1.GroupName = "RadioGroup1";
            radio2.GroupName = "RadioGroup1";

            // Beschriftungen festlegen
            radio1.Caption = "Option 1";
            radio2.Caption = "Option 2";

            // Speichere die Arbeitsmappe
            workbook.Save("RadioButtonGroupDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [RadioButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


