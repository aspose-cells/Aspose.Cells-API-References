---
title: PivotField.FilterByDate
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Filters by date values of row or column pivot field
type: docs
url: /net/aspose.cells.pivot/pivotfield/filterbydate/
---
## PivotField.FilterByDate method

Filters by date values of row or column pivot field.

```csharp
public PivotFilter FilterByDate(PivotFilterType type, DateTime dateTime1, DateTime dateTime2)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | PivotFilterType | The type of filtering data. |
| dateTime1 | DateTime | The date label of filter condition |
| dateTime2 | DateTime | The upper-bound date label of between filter condition |

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodFilterByDateWithPivotFilterTypeDateTimeDateTimDemo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data with dates
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2020, 9, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2020, 10, 20));
            worksheet.Cells["A4"].PutValue(new DateTime(2021, 9, 16));
            worksheet.Cells["A5"].PutValue(new DateTime(2021, 11, 5));

            // Create pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:A5", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Add date field to column area
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Column, 0);
            PivotField pivotField = pivotTable.ColumnFields[fieldIndex];
            
            // Apply date filter (September dates between 2020-2021)
            pivotField.FilterByDate(PivotFilterType.September, new DateTime(2020, 1, 1), new DateTime(2021, 12, 31));
            
            // Refresh and calculate pivot table
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Save results
            workbook.Save("FilterByDateDemo.xlsx");
        }
    }
}
```

### See Also

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


