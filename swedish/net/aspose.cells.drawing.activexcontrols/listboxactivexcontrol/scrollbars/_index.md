---
title: "ListBoxActiveXControl.ScrollBars"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListBoxActiveXControl egenskap. Anger om kontrollen har vertikala rullningslister, horisontella rullningslister, båda eller ingen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/scrollbars/
---
## ListBoxActiveXControl.ScrollBars property

Anger om kontrollen har vertikala rullningslister, horisontella rullningslister, båda eller ingen.

```csharp
public ControlScrollBarType ScrollBars { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyScrollBarsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 1, 0, 1, 0, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBoxControl = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Lägg till några objekt för att göra rullningslisterna synliga
            listBoxControl.ListFillRange = "A1:A20";
            for (int i = 1; i <= 20; i++)
            {
                worksheet.Cells["A" + i].PutValue("Item " + i);
            }

            // Demonstrera ScrollBars‑egenskap
            listBoxControl.ScrollBars = Aspose.Cells.Drawing.ActiveXControls.ControlScrollBarType.BarsBoth;

            workbook.Save("ListBoxScrollBarsDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ControlScrollBarType](../../controlscrollbartype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


