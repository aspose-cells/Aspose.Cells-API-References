---
title: "ActiveXControl.IsEnabled"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ActiveXControl-egenskap. Anger om kontrollen kan ta emot fokus och svara på användargenererade händelser"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/
---
## ActiveXControl.IsEnabled property

Anger om kontrollen kan ta emot fokus och svara på användargenererade händelser.

```csharp
public bool IsEnabled { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyIsEnabledDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 0, 1, 0, 1, 100, 50);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;
            checkBox.IsEnabled = true;
            checkBox.GroupName = "Sheet1";
            checkBox.Alignment = ControlCaptionAlignmentType.Right;
            checkBox.IsWordWrapped = true;
            checkBox.Value = CheckValueType.UnChecked;

            Console.WriteLine("IsEnabled state: " + checkBox.IsEnabled);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


