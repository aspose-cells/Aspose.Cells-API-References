---
title: Class PivotTableCalculateOption
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Pivot.PivotTableCalculateOption class. Rerepsents the options of calculating data of the pivot table
type: docs
url: /net/aspose.cells.pivot/pivottablecalculateoption/
---
## PivotTableCalculateOption class

Rerepsents the options of calculating data of the pivot table.

```csharp
public class PivotTableCalculateOption
```

## Constructors

| Name | Description |
| --- | --- |
| [PivotTableCalculateOption](pivottablecalculateoption/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [RefreshCharts](../../aspose.cells.pivot/pivottablecalculateoption/refreshcharts/) { get; set; } | Indicates whether refreshing charts are based on this pivot table. |
| [RefreshData](../../aspose.cells.pivot/pivottablecalculateoption/refreshdata/) { get; set; } | Indicates whether refreshing data source of the pivottable. |
| [ReserveMissingPivotItemType](../../aspose.cells.pivot/pivottablecalculateoption/reservemissingpivotitemtype/) { get; set; } | Represents how to reserve missing pivot items. |

### Examples

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionDemo
    {
        public static void PivotTableCalculateOptionExample()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some data for the pivot table
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["B3"].PutValue(30);
            sheet.Cells["A4"].PutValue("Fruit");
            sheet.Cells["B4"].PutValue(70);
            sheet.Cells["A5"].PutValue("Vegetable");
            sheet.Cells["B5"].PutValue(40);

            // Add a pivot table to the worksheet
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Configure the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // Create a PivotTableCalculateOption object
            PivotTableCalculateOption calculateOption = new PivotTableCalculateOption
            {
                RefreshData = true,
                RefreshCharts = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Calculate the pivot table data with the specified options
            pivotTable.CalculateData(calculateOption);

            // Save the workbook
            workbook.Save("PivotTableCalculateOptionExample.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


