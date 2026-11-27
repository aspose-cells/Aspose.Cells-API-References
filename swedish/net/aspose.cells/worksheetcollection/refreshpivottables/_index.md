---
title: "WorksheetCollection.RefreshPivotTables"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-metod. Uppdaterar alla PivotTables i Excel-filen"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/refreshpivottables/
---
## RefreshPivotTables() {#refreshpivottables_1}

Uppdaterar alla PivotTables i Excel‑filen.

```csharp
public void RefreshPivotTables()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRefreshPivotTablesDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa exempeldata för pivottabell
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(3000);

            // Lägg till pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 1);

            // Ändra källdata
            worksheet.Cells["B2"].PutValue(1500);
            worksheet.Cells["B3"].PutValue(2500);

            // Uppdatera alla pivottabeller i arbetsboken
            workbook.Worksheets.RefreshPivotTables();

            // Spara arbetsboken
            workbook.Save("RefreshPivotTablesDemo.xlsx");
        }
    }
}
```

### Se även

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RefreshPivotTables(PivotTableRefreshOption) {#refreshpivottables}

Uppdaterar alla PivotTables i Excel‑filen.

```csharp
public bool RefreshPivotTables(PivotTableRefreshOption option)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| alternativ | PivotTableRefreshOption | Alternativet för att uppdatera datakällan för pivottabellerna. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class WorksheetCollectionMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            cells["A1"].Value = "Category";
            cells["A2"].Value = "Fruit";
            cells["A3"].Value = "Vegetable";
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 1500;
            cells["B3"].Value = 2300;

            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B3", "E5", "SalesPivot");
            PivotTable pivotTable = pivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            PivotTableRefreshOption option = new PivotTableRefreshOption();

            workbook.Worksheets.RefreshPivotTables(option);

            Console.WriteLine(cells["F8"].StringValue);

            cells["B2"].Value = 2000;

            workbook.Worksheets.RefreshPivotTables(option);
            Console.WriteLine(cells["F8"].StringValue);
                       


            workbook.Save("WorksheetCollectionMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTableRefreshOption](../../../aspose.cells.pivot/pivottablerefreshoption/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


