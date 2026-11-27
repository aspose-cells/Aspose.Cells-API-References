---
title: "PivotItem.IsHidden"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotItem‑egenskap. Hämtar och anger om pivotelementet är dolt"
type: docs
url: /sv/net/aspose.cells.pivot/pivotitem/ishidden/
---
## PivotItem.IsHidden property

Hämtar och anger om pivotobjektet är dolt.

```csharp
public bool IsHidden { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "债券借贷";
            worksheet.Cells["A3"].Value = "股票";
            worksheet.Cells["A4"].Value = "基金";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Skapa pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Åtkomst till pivotfält och element
            PivotField field = pivotTable.RowFields[0];
            
            // Ställ in egenskapen IsHidden för att endast visa \"债券借贷\"
            foreach (PivotItem item in field.PivotItems)
            {
                item.IsHidden = (item.Name != "债券借贷");
            }

            // Uppdatera pivottabell
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("PivotItemIsHiddenDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


