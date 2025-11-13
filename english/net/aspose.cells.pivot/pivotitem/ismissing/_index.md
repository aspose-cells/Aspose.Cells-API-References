---
title: PivotItem.IsMissing
second_title: Aspose.Cells for .NET API Reference
description: PivotItem property. Indicates whether the item is removed from the data source
type: docs
url: /net/aspose.cells.pivot/pivotitem/ismissing/
---
## PivotItem.IsMissing property

Indicates whether the item is removed from the data source.

```csharp
public bool IsMissing { get; }
```

### Remarks

True means this value has been removed from the data source.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemPropertyIsMissingDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the pivot table
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Create a pivot table
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Add row field
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");

            // Add data field
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Refresh pivot table data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Get the first pivot item in the first row field
            PivotField rowField = pivotTable.RowFields[0];
            PivotItem pivotItem = rowField.PivotItems[0];

            // Display the IsMissing property value
            Console.WriteLine("IsMissing value for '{0}': {1}", pivotItem.Name, pivotItem.IsMissing);

            // Create a scenario where an item might be missing
            worksheet.Cells["A5"].PutValue("Grape");
            worksheet.Cells["B5"].PutValue(4000);
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Check if the original pivot item is now missing
            Console.WriteLine("After data change - IsMissing value for '{0}': {1}", 
                pivotItem.Name, pivotItem.IsMissing);

            // Save the workbook
            workbook.Save("PivotItemIsMissingDemo.xlsx");
        }
    }
}
```

### See Also

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


