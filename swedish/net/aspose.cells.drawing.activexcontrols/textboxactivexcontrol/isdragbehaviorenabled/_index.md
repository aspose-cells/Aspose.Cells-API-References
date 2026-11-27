---
title: "TextBoxActiveXControl.IsDragBehaviorEnabled"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxActiveXControl egenskap. Anger om dra-och-släpp är aktiverat för kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/isdragbehaviorenabled/
---
## TextBoxActiveXControl.IsDragBehaviorEnabled property

Indikerar om dra och släpp är aktiverat för kontrollen.

```csharp
public bool IsDragBehaviorEnabled { get; set; }
```

### Exempel

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

### Se även

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


