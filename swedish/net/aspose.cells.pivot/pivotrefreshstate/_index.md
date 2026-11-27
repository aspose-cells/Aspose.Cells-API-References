---
title: "Enum PivotRefreshState"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotRefreshState enum. Tillståndet för att uppdatera pivottabeller"
type: docs
url: /sv/net/aspose.cells.pivot/pivotrefreshstate/
---
## PivotRefreshState enumeration

Tillståndet för att uppdatera pivottabeller.

```csharp
public enum PivotRefreshState
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Success | `0` | Uppdateringen lyckades |
| UnsupportedExternalDataSource | `1` | Uppdateringen misslyckades eftersom datakällan är extern. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotRefreshStateDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med ett exempel på pivottabell
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Skapa pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Demonstrera PivotRefreshState
            PivotRefreshState refreshState = pivotTable.RefreshData();
            if (refreshState == PivotRefreshState.Success)
            {
                Console.WriteLine("Pivot table refreshed successfully");
            }
            else if (refreshState == PivotRefreshState.UnsupportedExternalDataSource)
            {
                Console.WriteLine("External data source not supported - calculating data instead");
                pivotTable.CalculateData();
            }

            // Spara arbetsboken
            workbook.Save("PivotRefreshStateDemo_out.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


