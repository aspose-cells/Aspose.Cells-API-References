---
title: "LabelActiveXControl.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LabelActiveXControl-egenskap. Hämtar typen av ActiveX-kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/type/
---
## LabelActiveXControl.Type property

Hämtar typen av ActiveX-kontrollen.

```csharp
public override ControlType Type { get; }
```

### Exempel

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

### Se även

* enum [ControlType](../../controltype/)
* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


