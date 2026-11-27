---
title: "PivotTable.EnableFieldList"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om fältlistan för PivotTable är tillgänglig i Excel-vyn"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/enablefieldlist/
---
## PivotTable.EnableFieldList property

Anger om fältlistan för pivottabellen är tillgänglig i Excels vy.

```csharp
public bool EnableFieldList { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyEnableFieldListDemo
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

            // Ställ in EnableFieldList-egenskapen
            pivotTable.EnableFieldList = false;

            // Spara arbetsboken
            workbook.Save("PivotTable_EnableFieldList_Demo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


