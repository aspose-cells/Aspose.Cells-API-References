---
title: PivotTable.GetSource
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Get the data source of this pivottable
type: docs
url: /net/aspose.cells.pivot/pivottable/getsource/
---
## GetSource() {#getsource}

Get the data source of this pivottable.

```csharp
public string[] GetSource()
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetSourceDemo
    {
        public static void Run()
        {
            // Create a workbook with sample data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data for pivot table
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Create pivot table
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Get and display the source data range
            string[] sourceData = pivotTable.GetSource();
            Console.WriteLine("Pivot Table Source: " + sourceData[0]);
            
            // Change the data source
            pivotTable.ChangeDataSource(new[] { "A1:B4" });
            
            // Verify the changed source
            sourceData = pivotTable.GetSource();
            Console.WriteLine("Updated Pivot Table Source: " + sourceData[0]);
        }
    }
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GetSource(bool) {#getsource_1}

Get the data source of this pivottable.

```csharp
public string[] GetSource(bool isOriginal)
```

| Parameter | Type | Description |
| --- | --- | --- |
| isOriginal | Boolean | Indicates whether to return original or display data source. |

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetSourceWithBooleanDemo
    {
        public static void Run()
        {
            // Create a workbook from source Excel file
            Workbook workbook = new Workbook("example.xlsx");
            
            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Access the first pivot table
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Get source data with local path (true)
            string[] localSource = pivotTable.GetSource(true);
            Console.WriteLine("Local path source: " + localSource[0]);
            
            // Get source data with full path (false)
            string[] fullSource = pivotTable.GetSource(false);
            Console.WriteLine("Full path source: " + fullSource[0]);
            
            // Save the workbook
            workbook.Save("output.xlsx");
        }
    }
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


