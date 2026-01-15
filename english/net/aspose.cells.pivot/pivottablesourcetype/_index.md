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
    using System;

    public class PivotClassPivotTableSourceTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Add sample data to the worksheet
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["A2"].PutValue("A");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["A3"].PutValue("B");
                worksheet.Cells["B3"].PutValue(20);
                worksheet.Cells["A4"].PutValue("C");
                worksheet.Cells["B4"].PutValue(30);

                // Create a pivot table collection
                PivotTableCollection pivotTables = worksheet.PivotTables;

                // Add a pivot table using Sheet as the source type
                int index = pivotTables.Add("=A1:B4", "D3", "SheetPivotTable");
                PivotTable pivotTable = pivotTables[index];

                // Display the source type
                Console.WriteLine("Pivot Table Source Type: " + pivotTable.SourceType);

                // Demonstrate different source types
                Console.WriteLine("Available PivotTableSourceType values:");
                Console.WriteLine("Sheet: " + PivotTableSourceType.Sheet);
                Console.WriteLine("External: " + PivotTableSourceType.External);
                Console.WriteLine("Consolidation: " + PivotTableSourceType.Consolidation);
                Console.WriteLine("Scenario: " + PivotTableSourceType.Scenario);
                Console.WriteLine("Unknown: " + PivotTableSourceType.Unknown);

                // Save the workbook
                workbook.Save("PivotTableSourceTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PivotTableSourceType: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


