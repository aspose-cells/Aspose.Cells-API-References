---
title: "ToggleButtonActiveXControl.Value"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ToggleButtonActiveXControl-Eigenschaft. Gibt an, ob das Steuerelement aktiviert ist oder nicht"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/value/
---
## ToggleButtonActiveXControl.Value property

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
    public class ToggleButtonActiveXControlPropertyValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein ToggleButton‑ActiveX‑Steuerelement hinzu
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 1, 100, 30);
            ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // Setzen Sie den Anfangswert auf Nicht aktiviert
            toggleButton.Value = CheckValueType.UnChecked;

            // Überprüfen und schalten Sie den Wert um, wenn er Nicht aktiviert ist
            if (toggleButton.Value == CheckValueType.UnChecked)
            {
                toggleButton.Value = CheckValueType.Checked;
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ToggleButtonDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [CheckValueType](../../../aspose.cells.drawing/checkvaluetype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


