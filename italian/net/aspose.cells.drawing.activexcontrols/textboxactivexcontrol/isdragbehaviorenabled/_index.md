---
title: "TextBoxActiveXControl.IsDragBehaviorEnabled"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxActiveXControl. Indica se il trascinamento e il rilascio sono abilitati per il controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/isdragbehaviorenabled/
---
## TextBoxActiveXControl.IsDragBehaviorEnabled property

Indica se il trascinamento e il rilascio sono abilitati per il controllo.

```csharp
public bool IsDragBehaviorEnabled { get; set; }
```

### Esempi

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

### Vedi anche

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


