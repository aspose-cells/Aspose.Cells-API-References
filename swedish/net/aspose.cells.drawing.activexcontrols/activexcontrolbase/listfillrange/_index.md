---
title: "ActiveXControlBase.ListFillRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ActiveXControlBase-egenskap. Hämtar och anger listfyllnadsintervallet"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/
---
## ActiveXControlBase.ListFillRange property

Hämtar och anger listfyllningsområdet.

```csharp
public string ListFillRange { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyListFillRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för ListFillRange
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Item " + i);
            }

            // Lägg till en ComboBoxActiveXControl
            Shape shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox,
                1, 0, 100, 50, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Ange ListFillRange för att fylla i kombinationsrutan
            comboBox.ListFillRange = "A2:A10";

            // Spara arbetsboken
            workbook.Save("ActiveXControlListFillRangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


