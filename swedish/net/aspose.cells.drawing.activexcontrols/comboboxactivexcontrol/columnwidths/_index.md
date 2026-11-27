---
title: "ComboBoxActiveXControl.ColumnWidths"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ComboBoxActiveXControl-egenskap. Hämtar och anger bredden på kolumnen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/columnwidths/
---
## ComboBoxActiveXControl.ColumnWidths property

Hämtar och anger bredden på kolumnen.

```csharp
public double ColumnWidths { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyColumnWidthsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox,
                5, 0, 100, 20, 100, 20);
            
            var comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            comboBox.ColumnCount = 3;
            comboBox.ListRows = 5;
            
            // Ställ in kolumnbredder (använd dubbelvärde för enskild kolumnbredd)
            comboBox.ColumnWidths = 100;

            // Ställ in listobjekt via ListFillRange
            worksheet.Cells["A1"].PutValue("Product\tPrice\tStock");
            worksheet.Cells["A2"].PutValue("Laptop\t$999\t50");
            worksheet.Cells["A3"].PutValue("Phone\t$699\t120");
            worksheet.Cells["A4"].PutValue("Tablet\t$399\t75");
            comboBox.ListFillRange = "A1:A4";

            workbook.Save("ComboBoxColumnWidthsDemo.xlsx");
        }
    }
}
```

### Se även

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


