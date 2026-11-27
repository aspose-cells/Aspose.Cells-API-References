---
title: "ListBoxActiveXControl.IntegralHeight"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListBoxActiveXControl egenskap. Anger om kontrollen endast visar hela textrader utan att visa några ofullständiga rader"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/integralheight/
---
## ListBoxActiveXControl.IntegralHeight property

Indikerar om kontrollen endast visar hela textrader utan att visa några partiella rader.

```csharp
public bool IntegralHeight { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyIntegralHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox,
                10,  // left
                10,  // top
                200, // width
                100, // height
                0,   // imageWidth (required parameter)
                0    // imageHeight (required parameter)
            );
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Demonstrera IntegralHeight-egenskapen
            listBox.IntegralHeight = true;
            Console.WriteLine("ListBox IntegralHeight set to: " + listBox.IntegralHeight);

            // Lägg till exempelobjekt
            listBox.ListFillRange = "A1:A3";
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Orange");

            workbook.Save("ListBoxIntegralHeightDemo.xlsx");
        }
    }
}
```

### Se även

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


