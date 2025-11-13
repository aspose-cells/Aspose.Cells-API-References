---
title: PivotTable.Format
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Formats selected area of the PivotTable
type: docs
url: /net/aspose.cells.pivot/pivottable/format/
---
## Format(PivotArea, Style) {#format_1}

Formats selected area of the PivotTable.

```csharp
public void Format(PivotArea pivotArea, Style style)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivotArea | PivotArea | The selected pivot view area. |
| style | Style | The formatted setting. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Drawing;

    public class PivotTableMethodFormatWithPivotAreaStyleDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the pivot table
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["A4"].Value = "Truck";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 5000;
            worksheet.Cells["B3"].Value = 12000;
            worksheet.Cells["B4"].Value = 8000;

            // Create a pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D3", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Calculate data to populate the pivot table
            pivotTable.CalculateData();

            // Create a style for formatting
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // Create pivot area for formatting
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.AxisType = PivotFieldType.Data;

            try
            {
                // Apply formatting to the pivot area
                pivotTable.Format(pivotArea, style);
                
                Console.WriteLine("Format method executed successfully with parameters (PivotArea, Style)");
                
                // Save the workbook to show the effect
                workbook.Save("PivotTableFormatWithPivotAreaStyleDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Format method: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [PivotArea](../../pivotarea/)
* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Format(CellArea, Style) {#format}

Formats selected area of the PivotTable.

```csharp
public void Format(CellArea ca, Style style)
```

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The range of the cells. |
| style | Style | The style |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Drawing;

    public class PivotTableMethodFormatWithCellAreaStyleDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the pivot table
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue("South");
            worksheet.Cells["C3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Product C");
            worksheet.Cells["B4"].PutValue("East");
            worksheet.Cells["C4"].PutValue(3000);

            // Create a pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Add row and data fields
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Calculate data and ranges
            pivotTable.CalculateData();
            pivotTable.CalculateRange();

            // Create a style for formatting
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // Define cell area to format (data body range)
            CellArea area = pivotTable.DataBodyRange;

            try
            {
                // Call the Format method with CellArea and Style parameters
                pivotTable.Format(area, style);
                
                Console.WriteLine("PivotTable formatted successfully with parameters (CellArea, Style)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error formatting PivotTable: {ex.Message}");
            }
            
            // Save the result
            workbook.Save("PivotTableFormatWithCellAreaStyleDemo.xlsx");
        }
    }
}
```

### See Also

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Format(int, int, Style) {#format_2}

Formats the cell in the pivottable area

```csharp
public void Format(int row, int column, Style style)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row Index of the cell |
| column | Int32 | Column index of the cell |
| style | Style | Style which is to format the cell |

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodFormatWithInt32Int32StyleDemo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for pivot table
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(150);

            // Add pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Add fields to row area
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Calculate data
            pivotTable.CalculateData();

            // Create a style for formatting
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.LightBlue;
            style.Font.IsBold = true;

            // Format the pivot table header cell (row 2, column 0 in pivot table coordinates)
            pivotTable.Format(2, 0, style);

            // Save the workbook
            workbook.Save("PivotTableFormatDemo.xlsx");
        }
    }
}
```

### See Also

* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


