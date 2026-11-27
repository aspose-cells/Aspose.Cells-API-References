---
title: "ActiveXControlBase.Width"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ActiveXControlBase-egenskap. Hämtar och anger kontrollens bredd i enheten punkter"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/width/
---
## ActiveXControlBase.Width property

Hämtar och anger kontrollens bredd i enheter av punkter.

```csharp
public virtual double Width { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 5, 0, 100, 20);
            ActiveXControlBase control = (ActiveXControlBase)shape.ActiveXControl;

            // Demonstrera användning av Width-egenskapen
            Console.WriteLine("Original width: " + control.Width);
            control.Width = 150;
            Console.WriteLine("Modified width: " + control.Width);

            workbook.Save("ActiveXControlWidthDemo.xlsx");
        }
    }
}
```

### Se även

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


