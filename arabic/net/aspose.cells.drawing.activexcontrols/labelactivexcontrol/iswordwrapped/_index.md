---
title: "LabelActiveXControl.IsWordWrapped"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LabelActiveXControl. تشير إلى ما إذا كان محتوى العنصر يلتف تلقائيًا في نهاية السطر"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/iswordwrapped/
---
## LabelActiveXControl.IsWordWrapped property

يشير إلى ما إذا كان محتوى العنصر يلتف تلقائيًا في نهاية السطر.

```csharp
public bool IsWordWrapped { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LabelActiveXControlPropertyIsWordWrappedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.Label, 5, 0, 1, 1, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.LabelActiveXControl label = (Aspose.Cells.Drawing.ActiveXControls.LabelActiveXControl)shape.ActiveXControl;

            label.Caption = "This is a long text that will demonstrate word wrapping when IsWordWrapped is set to true";
            label.IsWordWrapped = true;
            label.IsAutoSize = true;

            Console.WriteLine("Label IsWordWrapped: " + label.IsWordWrapped);
            Console.WriteLine("Label Caption: " + label.Caption);

            workbook.Save("LabelActiveXControlIsWordWrappedDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


