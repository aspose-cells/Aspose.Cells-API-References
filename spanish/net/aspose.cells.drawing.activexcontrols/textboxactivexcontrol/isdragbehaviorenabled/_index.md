---
title: "TextBoxActiveXControl.IsDragBehaviorEnabled"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxActiveXControl. Indica si arrastrar y soltar está habilitado para el control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/isdragbehaviorenabled/
---
## TextBoxActiveXControl.IsDragBehaviorEnabled property

Indica si arrastrar y soltar está habilitado para el control.

```csharp
public bool IsDragBehaviorEnabled { get; set; }
```

### Ejemplos

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

### Ver también

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


