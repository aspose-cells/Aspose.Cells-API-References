---
title: "ListBoxActiveXControl.BorderOleColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListBoxActiveXControl egenskap. Hämtar och sätter bakgrundens ole-färg"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/borderolecolor/
---
## ListBoxActiveXControl.BorderOleColor property

Hämtar och anger ole-färgen för bakgrunden.

```csharp
public int BorderOleColor { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyBorderOleColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 1, 0, 0, 200, 100);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;
            
            listBox.BorderOleColor = -2147483642;
            
            workbook.Save("ListBoxBorderOleColorDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Se även

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


