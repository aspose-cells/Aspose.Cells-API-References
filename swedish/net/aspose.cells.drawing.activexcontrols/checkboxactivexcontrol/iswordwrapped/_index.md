---
title: "CheckBoxActiveXControl.IsWordWrapped"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CheckBoxActiveXControl egenskap. Anger om kontrollens innehåll automatiskt radbryts vid slutet av en rad"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/iswordwrapped/
---
## CheckBoxActiveXControl.IsWordWrapped property

Anger om innehållet i kontrollen automatiskt radbryts i slutet av en rad.

```csharp
public bool IsWordWrapped { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyIsWordWrappedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 5, 0, 150, 50);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            checkBox.Caption = "This is a long caption that should word wrap when enabled";
            checkBox.IsWordWrapped = true;
            checkBox.IsAutoSize = true;

            workbook.Save("CheckBoxWordWrapDemo.xlsx");
        }
    }
}
```

### Se även

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


