---
title: "PivotTable.DisplayImmediateItems"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om objekt i rad- och kolumnområdena är synliga när dataområdet i PivotTable är tomt. Standardvärdet är true"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/displayimmediateitems/
---
## PivotTable.DisplayImmediateItems property

Anger om objekt i rad‑ och kolumnområdena är synliga när dataområdet i pivottabellen är tomt. Standardvärdet är sant.

```csharp
public bool DisplayImmediateItems { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDisplayImmediateItemsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Skapa pivottabell
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Lägg till fält i pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Demonstrera DisplayImmediateItems-egenskapen
            Console.WriteLine("Initial DisplayImmediateItems value: " + pivotTable.DisplayImmediateItems);
            
            // Ändra egenskapsvärdet
            pivotTable.DisplayImmediateItems = false;
            Console.WriteLine("After setting to false: " + pivotTable.DisplayImmediateItems);

            // Spara arbetsboken
            workbook.Save("PivotTableDisplayImmediateItemsDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


