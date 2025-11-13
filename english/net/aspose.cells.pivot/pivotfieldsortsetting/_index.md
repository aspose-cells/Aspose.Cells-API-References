---
title: Class PivotFieldSortSetting
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Pivot.PivotFieldSortSetting class. Represents the setting for sorting pivot fields
type: docs
url: /net/aspose.cells.pivot/pivotfieldsortsetting/
---
## PivotFieldSortSetting class

Represents the setting for sorting pivot fields.

```csharp
public class PivotFieldSortSetting
```

## Properties

| Name | Description |
| --- | --- |
| [Cell](../../aspose.cells.pivot/pivotfieldsortsetting/cell/) { get; } | Sorts by the values in which row or column. |
| [FieldIndex](../../aspose.cells.pivot/pivotfieldsortsetting/fieldindex/) { get; } | Represents the index of the field sorted by. -1 means sorting the PivotField by the labels,others means sorting by the data field. |
| [IsSimpleSort](../../aspose.cells.pivot/pivotfieldsortsetting/issimplesort/) { get; } | Indicates whether a simple data sort operation will be applied. |
| [IsSortByLabels](../../aspose.cells.pivot/pivotfieldsortsetting/issortbylabels/) { get; } | Indicates whether to sort the field by itself or data field. |
| [LineTypeSortedBy](../../aspose.cells.pivot/pivotfieldsortsetting/linetypesortedby/) { get; } | The pivot line type sorted by. |
| [SortType](../../aspose.cells.pivot/pivotfieldsortsetting/sorttype/) { get; } | Represents the [`SortOrder`](../../aspose.cells/sortorder/). |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotFieldSortSettingDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for pivot table
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B2"].PutValue("East");
            worksheet.Cells["B3"].PutValue("West");
            worksheet.Cells["B4"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["C3"].PutValue(2000);
            worksheet.Cells["C4"].PutValue(3000);

            // Create a pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Get pivot field sort setting from the pivot table
            // Note: This assumes the pivot table has sorting settings we can access
            // Since we can't create a new PivotFieldSortSetting directly
            PivotFieldSortSetting sortSetting = pivotTable.RowFields[0].SortSetting;
            
            // Display properties (read-only)
            Console.WriteLine("SortType: " + sortSetting.SortType);
            Console.WriteLine("IsSortByLabels: " + sortSetting.IsSortByLabels);
            Console.WriteLine("FieldIndex: " + sortSetting.FieldIndex);
            Console.WriteLine("LineTypeSortedBy: " + sortSetting.LineTypeSortedBy);
            Console.WriteLine("IsSimpleSort: " + sortSetting.IsSimpleSort);
            Console.WriteLine("Cell: " + sortSetting.Cell);

            // Apply sorting to pivot table (actual sorting would be done through pivot table methods)
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Save the result
            workbook.Save("PivotFieldSortSettingDemo.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


