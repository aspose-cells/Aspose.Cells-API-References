---
title: "CheckBoxActiveXControl.IsWordWrapped"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CheckBoxActiveXControl-Eigenschaft. Gibt an, ob der Inhalt des Steuerelements am Zeilenende automatisch umbrochen wird"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/iswordwrapped/
---
## CheckBoxActiveXControl.IsWordWrapped property

Gibt an, ob der Inhalt des Steuerelements am Zeilenende automatisch umbrochen wird.

```csharp
public bool IsWordWrapped { get; set; }
```

### Beispiele

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

### Siehe auch

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


