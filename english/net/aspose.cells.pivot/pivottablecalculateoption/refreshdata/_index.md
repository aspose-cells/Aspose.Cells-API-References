---
title: PivotTableCalculateOption.RefreshData
second_title: Aspose.Cells for .NET API Reference
description: PivotTableCalculateOption property. Indicates whether refreshing data source of the pivottable
type: docs
url: /net/aspose.cells.pivot/pivottablecalculateoption/refreshdata/
---
## PivotTableCalculateOption.RefreshData property

Indicates whether refreshing data source of the pivottable.

```csharp
public bool RefreshData { get; set; }
```

### Remarks

If it is true, refresh pivot cache from data source,then calculate all pivot tables based same pivot cache.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionPropertyRefreshDataDemo
    {
        public static void Run()
        {
            // Create a workbook from source Excel file
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Setup sample data for pivot table
            var cells = sheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Sales");
            cells["A2"].PutValue("A");
            cells["B2"].PutValue(100);
            cells["A3"].PutValue("B");
            cells["B3"].PutValue(200);
            cells["A4"].PutValue("C");
            cells["B4"].PutValue(300);

            // Create pivot table
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Modify source data
            cells["B2"].PutValue(150); // Change value from 100 to 150

            // Calculate pivot table with RefreshData option
            PivotTableCalculateOption options = new PivotTableCalculateOption();
            options.RefreshData = true;
            pivotTable.CalculateData(options);

            // Output the updated pivot table value
            Console.WriteLine("Updated Pivot Table Value: " + cells["F5"].StringValue);
        }
    }
}
```

### See Also

* class [PivotTableCalculateOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


