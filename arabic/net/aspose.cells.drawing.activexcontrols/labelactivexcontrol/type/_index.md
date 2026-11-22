---
title: "LabelActiveXControl.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LabelActiveXControl. يحصل على نوع عنصر التحكم ActiveX"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/type/
---
## LabelActiveXControl.Type property

يحصل على نوع عنصر التحكم ActiveX.

```csharp
public override ControlType Type { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class LabelActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape labelShape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 1, 1, 200, 50, 0, 0);
            LabelActiveXControl labelControl = (LabelActiveXControl)labelShape.ActiveXControl;

            labelControl.Caption = "Demo Label";

            Console.WriteLine("Label Control Type: " + labelControl.Type);
            
            workbook.Save("LabelControlDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ControlType](../../controltype/)
* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


