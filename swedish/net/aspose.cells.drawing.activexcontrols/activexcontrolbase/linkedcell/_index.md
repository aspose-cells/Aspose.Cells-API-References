---
title: "ActiveXControlBase.LinkedCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ActiveXControlBase-egenskap. Hämtar och anger den länkade cellen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/
---
## ActiveXControlBase.LinkedCell property

Hämtar och anger den länkade cellen.

```csharp
public string LinkedCell { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyLinkedCellDemo
    {
        public static void Run()
        {
            // Initiera en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till en SpinButtonActiveXControl i det första kalkylbladet
            Aspose.Cells.Drawing.Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 
                10, 10, 100, 30, 100, 30);
            Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl spinButton = 
                (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;

            // Konfigurera spin‑knappens egenskaper
            spinButton.Min = 0;
            spinButton.Max = 100;
            spinButton.Position = 50;
            spinButton.SmallChange = 1;

            // Länka kontrollen till cell A1
            spinButton.LinkedCell = "A1";

            // Ställ in cell A1:s värde så att det matchar startpositionen
            workbook.Worksheets[0].Cells["A1"].PutValue(spinButton.Position);

            // Spara arbetsboken
            workbook.Save("LinkedCellDemo.xlsx");
        }
    }
}
```

### Se även

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


