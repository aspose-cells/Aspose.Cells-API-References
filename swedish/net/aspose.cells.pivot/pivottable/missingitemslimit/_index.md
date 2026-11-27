---
title: "PivotTable.MissingItemsLimit"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger ett booleskt värde som visar om fälten i en PivotTable kan ha flera filter inställda på dem"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/missingitemslimit/
---
## PivotTable.MissingItemsLimit property

Anger ett booleskt värde som visar om fälten i en PivotTable kan ha flera filter inställda på dem.

```csharp
[Obsolete("Use PivotCache.MissingItemsLimit propery  instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotMissingItemLimitType MissingItemsLimit { get; set; }
```

### Anmärkningar

OBS: Den här egenskapen är nu föråldrad. Använd istället egenskapen PivotCache.MissingItemsLimit. Den här metoden kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyMissingItemsLimitDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Exempeldata
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B4"].Value = 30;

            // Skapa en pivottabell och hämta instansen
            int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:B4", "E3");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Konfigurera pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Value
            
            // Demonstrera egenskapen MissingItemsLimit
            pivotTable.MissingItemsLimit = PivotMissingItemLimitType.Max;
            
            // Uppdatera data
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            workbook.Save("PivotTableMissingItemsLimitDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PivotMissingItemLimitType](../../pivotmissingitemlimittype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


