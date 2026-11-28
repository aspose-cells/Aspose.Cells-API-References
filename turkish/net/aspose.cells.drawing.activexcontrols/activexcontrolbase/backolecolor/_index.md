---
title: "ActiveXControlBase.BackOleColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ActiveXControlBase özelliği. Arka planın ole rengini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/
---
## ActiveXControlBase.BackOleColor property

Arka planın ole rengini alır ve ayarlar.

```csharp
public virtual int BackOleColor { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyBackOleColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 5, 0, 1, 1, 100, 20);
            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            label.Caption = "BackOleColor Demo";
            label.BackOleColor = 0xFFFF00; // Yellow background
            label.ForeOleColor = 0x0000FF; // Blue text
            label.IsAutoSize = true;

            Console.WriteLine("Label Back Color: " + label.BackOleColor.ToString("X6"));
            
            workbook.Save("BackOleColorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


