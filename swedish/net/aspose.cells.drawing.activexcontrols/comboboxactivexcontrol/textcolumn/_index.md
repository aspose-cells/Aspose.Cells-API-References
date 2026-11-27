---
title: "ComboBoxActiveXControl.TextColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ComboBoxActiveXControl-egenskap. Representerar kolumnen i en ComboBox eller ListBox som ska visas för användaren"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/textcolumn/
---
## ComboBoxActiveXControl.TextColumn property

Representerar kolumnen i en ComboBox eller ListBox som ska visas för användaren.

```csharp
public int TextColumn { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyTextColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ComboBox ActiveX control med alla nödvändiga parametrar
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 
                10, 10, 150, 30, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Ställ in egenskaper för combo box
            comboBox.ColumnCount = 2;
            comboBox.ListRows = 5;
            
            // Lägg till objekt med ListFillRange (alternativ till AddItem)
            worksheet.Cells["A1"].PutValue("Item1");
            worksheet.Cells["B1"].PutValue("Description1");
            worksheet.Cells["A2"].PutValue("Item2");
            worksheet.Cells["B2"].PutValue("Description2");
            worksheet.Cells["A3"].PutValue("Item3");
            worksheet.Cells["B3"].PutValue("Description3");
            comboBox.ListFillRange = "A1:B3";

            // Demonstrera TextColumn-egenskapen
            comboBox.TextColumn = 2; // Display second column (descriptions) as text
            comboBox.BoundColumn = 1; // But bind to first column (items)

            // Spara arbetsboken
            workbook.Save("ComboBoxTextColumnDemo.xlsx");
        }
    }
}
```

### Se även

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


