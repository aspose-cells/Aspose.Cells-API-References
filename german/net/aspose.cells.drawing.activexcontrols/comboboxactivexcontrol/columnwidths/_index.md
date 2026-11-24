---
title: "ComboBoxActiveXControl.ColumnWidths"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ComboBoxActiveXControl-Eigenschaft. Gibt die Breite der Spalte zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/columnwidths/
---
## ComboBoxActiveXControl.ColumnWidths property

Liest und schreibt die Breite der Spalte.

```csharp
public double ColumnWidths { get; set; }
```

### Beispiele

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
            
            // Spaltenbreiten festlegen (unter Verwendung eines Double-Werts für die Breite einer einzelnen Spalte)
            comboBox.ColumnWidths = 100;

            // Listeneinträge über ListFillRange festlegen
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

### Siehe auch

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


