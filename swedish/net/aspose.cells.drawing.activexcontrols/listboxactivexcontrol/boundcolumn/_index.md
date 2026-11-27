---
title: "ListBoxActiveXControl.BoundColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListBoxActiveXControl egenskap. Representerar hur Value-egenskapen bestäms för en ComboBox eller ListBox när MultiSelect-egenskapens värde är fmMultiSelectSingle"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/boundcolumn/
---
## ListBoxActiveXControl.BoundColumn property

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
    public class ListBoxActiveXControlPropertyBoundColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B4"].PutValue("Banana");

            // Lägg till ListBox ActiveX‑kontroll
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 5, 0, 1, 0, 150, 100);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Konfigurera ListBox‑egenskaper
            listBox.ColumnCount = 2;
            listBox.ListFillRange = "A1:B4";
            
            // Ställ in BoundColumn till 0 (ID-kolumn) - detta blir värdet som returneras när ett objekt väljs
            listBox.BoundColumn = 0;
            
            // Ställ in TextColumn till 1 (Namnkolumn) - detta kommer att visas i listan
            listBox.TextColumn = 1;

            // Spara arbetsboken
            workbook.Save("ListBoxBoundColumnDemo.xlsx");

            Console.WriteLine("ListBox BoundColumn set to: " + listBox.BoundColumn);
        }
    }
}
```

### Se även

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


