---
title: "PivotTable.IsSelected"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable‑egenskap. Anger om denna pivottabell är markerad"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/isselected/
---
## PivotTable.IsSelected property

Anger om denna PivotTable är markerad.

```csharp
public bool IsSelected { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIsSelectedDemo
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
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];

            // Initialt är IsSelected falskt
            Console.WriteLine("PivotTable IsSelected initially: " + pivotTable.IsSelected);

            // Markera pivottabellen
            pivotTable.IsSelected = true;
            Console.WriteLine("PivotTable IsSelected after setting to true: " + pivotTable.IsSelected);

            // Avmarkera pivottabellen
            pivotTable.IsSelected = false;
            Console.WriteLine("PivotTable IsSelected after setting to false: " + pivotTable.IsSelected);
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


