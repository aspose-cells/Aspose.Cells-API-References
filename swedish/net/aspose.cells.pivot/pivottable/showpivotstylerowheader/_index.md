---
title: "PivotTable.ShowPivotStyleRowHeader"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable‑egenskap. Anger om radhuvudet i pivottabellen ska ha stilen tillämpad"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/showpivotstylerowheader/
---
## PivotTable.ShowPivotStyleRowHeader property

Anger om radhuvudet i pivottabellen ska ha stilen tillämpad.

```csharp
public bool ShowPivotStyleRowHeader { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowPivotStyleRowHeaderDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
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

            // Lägg till en pivottabell
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Konfigurera pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Demonstrera egenskapen ShowPivotStyleRowHeader
            pivotTable.ShowPivotStyleRowHeader = true;
            Console.WriteLine("ShowPivotStyleRowHeader is set to: " + pivotTable.ShowPivotStyleRowHeader);

            // Spara arbetsboken
            workbook.Save("PivotTableShowPivotStyleRowHeaderDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


