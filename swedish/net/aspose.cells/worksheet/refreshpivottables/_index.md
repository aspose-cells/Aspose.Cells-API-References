---
title: "Worksheet.RefreshPivotTables"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-metod. Uppdaterar alla PivotTables i detta Worksheet"
type: docs
url: /sv/net/aspose.cells/worksheet/refreshpivottables/
---
## RefreshPivotTables() {#refreshpivottables_1}

Uppdaterar alla PivotTables i detta kalkylblad.

```csharp
public void RefreshPivotTables()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRefreshPivotTablesDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑fil som innehåller pivottabeller
            Workbook workbook = new Workbook("example.xlsx");
            
            // Hämta det första worksheet som innehåller pivottabeller
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Uppdatera alla pivottabeller i worksheet
            worksheet.RefreshPivotTables();
            
            // Spara den uppdaterade workbook
            workbook.Save("RefreshedPivotTables.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RefreshPivotTables(PivotTableRefreshOption) {#refreshpivottables}

Uppdaterar alla PivotTables i detta kalkylblad.

```csharp
public bool RefreshPivotTables(PivotTableRefreshOption option)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| alternativ | PivotTableRefreshOption | Alternativet för att uppdatera datakällan för pivottabell. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class WorksheetMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;

            // Skapa en pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            worksheet.RefreshPivotTables();

            int preCount = pivotTable.RowFields[0].PivotItems.Count;


            // Ändra källdata
            worksheet.Cells["A2"].Value = "test2";
            worksheet.Cells["A3"].Value = "test3";

            // Skapa uppdateringsalternativ
            PivotTableRefreshOption options = new PivotTableRefreshOption
            {
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All // Fixed: Changed ReserveAll to All
            };
            worksheet.RefreshPivotTables(options);
            int nowCount = pivotTable.RowFields[0].PivotItems.Count;
            Console.WriteLine(nowCount > preCount);
                        

            // Spara resultatet
            workbook.Save("WorksheetMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTableRefreshOption](../../../aspose.cells.pivot/pivottablerefreshoption/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


