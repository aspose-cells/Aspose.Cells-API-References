---
title: "TextBoxActiveXControl.IsDragBehaviorEnabled"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextBoxActiveXControl-Eigenschaft. Gibt an, ob Ziehen und Ablegen für das Steuerelement aktiviert ist"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/isdragbehaviorenabled/
---
## TextBoxActiveXControl.IsDragBehaviorEnabled property

Gibt an, ob Ziehen und Ablegen für das Steuerelement aktiviert ist.

```csharp
public bool IsDragBehaviorEnabled { get; set; }
```

### Beispiele

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIsDragBehaviorEnabledDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 1, 0, 1, 0, 100, 22);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;

            if (!textBox.IsDragBehaviorEnabled)
            {
                textBox.IsDragBehaviorEnabled = true;
            }

            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


