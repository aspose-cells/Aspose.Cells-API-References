---
title: "CheckBoxActiveXControl.Value"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CheckBoxActiveXControl-Eigenschaft. Gibt an, ob das Steuerelement aktiviert ist oder nicht"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/value/
---
## CheckBoxActiveXControl.Value property

Gibt an, ob das Steuerelement aktiviert ist oder nicht.

```csharp
public CheckValueType Value { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyValueDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein CheckBox‑ActiveX‑Steuerelement zum Arbeitsblatt hinzu
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.CheckBox, 5, 0, 5, 0, 100, 20);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Setzen Sie grundlegende Eigenschaften einschließlich Value
            checkBox.Caption = "Check Me";
            checkBox.Value = CheckValueType.Checked; // Demonstrating Value property usage

            // Speichere die Arbeitsmappe
            workbook.Save("CheckBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [CheckValueType](../../../aspose.cells.drawing/checkvaluetype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


