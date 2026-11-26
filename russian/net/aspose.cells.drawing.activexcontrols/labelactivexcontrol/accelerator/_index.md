---
title: "LabelActiveXControl.Accelerator"
second_title: "Справочник API Aspose.Cells для .NET"
description: "LabelActiveXControl property. Получает и задает клавишу‑ускоритель для элемента управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/accelerator/
---
## LabelActiveXControl.Accelerator property

Получает и задает клавишу ускорителя для элемента управления.

```csharp
public char Accelerator { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class LabelActiveXControlPropertyAcceleratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 5, 0, 1, 1, 100, 20);
            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            label.Caption = "Press Alt+H";
            label.Accelerator = 'H';
            label.IsVisible = true;

            Console.WriteLine("Label Caption: " + label.Caption);
            Console.WriteLine("Label Accelerator: " + label.Accelerator);

            workbook.Save("LabelActiveXControlAcceleratorDemo.xlsx");
        }
    }
}
```

### См. также

* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


