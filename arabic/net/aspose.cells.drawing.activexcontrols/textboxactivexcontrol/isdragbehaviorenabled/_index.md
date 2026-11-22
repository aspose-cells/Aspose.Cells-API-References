---
title: "TextBoxActiveXControl.IsDragBehaviorEnabled"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextBoxActiveXControl. تشير إلى ما إذا كان سحب وإفلات مفعّلاً للعنصر"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/isdragbehaviorenabled/
---
## TextBoxActiveXControl.IsDragBehaviorEnabled property

يشير إلى ما إذا كان السحب والإفلات مفعّلاً للعنصر.

```csharp
public bool IsDragBehaviorEnabled { get; set; }
```

### أمثلة

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

### انظر أيضًا

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


