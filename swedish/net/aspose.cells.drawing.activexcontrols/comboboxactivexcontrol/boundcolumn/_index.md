---
title: "ComboBoxActiveXControl.BoundColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ComboBoxActiveXControl property. Representerar hur Value property bestäms för en ComboBox eller ListBox när MultiSelect-egenskapens värde är fmMultiSelectSingle"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/boundcolumn/
---
## ComboBoxActiveXControl.BoundColumn property

Representerar hur Value-egenskapen bestäms för en ComboBox eller ListBox när MultiSelect-egenskapens värde är (fmMultiSelectSingle).

```csharp
public int BoundColumn { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyBoundColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B4"].PutValue("Banana");

            // Lägg till en ComboBox ActiveX-kontroll
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 5, 0, 1, 0, 150, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Konfigurera ComboBox
            comboBox.ListFillRange = "A1:B4";
            comboBox.ColumnCount = 2;
            comboBox.BoundColumn = 0; // Bind to the ID column (column index 0)
            comboBox.TextColumn = 1; // Display the Name column (column index 1)

            // Spara arbetsboken
            workbook.Save("ComboBoxBoundColumnDemo.xlsx");

            Console.WriteLine("ComboBox BoundColumn set to: " + comboBox.BoundColumn);
        }
    }
}
```

### Se även

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


