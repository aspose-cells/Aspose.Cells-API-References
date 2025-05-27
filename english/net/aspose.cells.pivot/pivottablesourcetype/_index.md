---
title: Enum PivotTableSourceType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Pivot.PivotTableSourceType enum. Represents data source type of the pivot table
type: docs
url: /net/aspose.cells.pivot/pivottablesourcetype/
---
## PivotTableSourceType enumeration

Represents data source type of the pivot table.

```csharp
public enum PivotTableSourceType : byte
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Sheet | `1` | Specifies that the source data is a range. |
| External | `2` | Specifies that external source data is used. |
| Consolidation | `4` | Specifies that multiple consolidation ranges are used as the source data. |
| Scenario | `8` | The source data is populated from a temporary internal structure. |
| Unknown | `9` | Unknown data source. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;

    public class PivotClassPivotTableSourceTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Populate sample data
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Vegetable";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1500;
            worksheet.Cells["B3"].Value = 1200;

            // Create pivot table using worksheet data source
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B3", "E5", "SalesReport", true);
            
            PivotTable pivotTable = pivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            if (pivotTable.DataFields.Count > 0)
            {
                PivotField dataField = pivotTable.DataFields[0];
                dataField.DisplayName = "Total Sales";
                dataField.Function = ConsolidationFunction.Sum;
            }

            pivotTable.RefreshData();
            pivotTable.CalculateData();

            workbook.Save("PivotTableSourceTypeDemo.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


