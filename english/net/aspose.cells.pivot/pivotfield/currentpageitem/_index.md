---
title: PivotField.CurrentPageItem
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represents the current selected page item of the page field to filter data. Only valid for page fields
type: docs
url: /net/aspose.cells.pivot/pivotfield/currentpageitem/
---
## PivotField.CurrentPageItem property

Represents the current selected page item of the page field to filter data. Only valid for page fields.

```csharp
public short CurrentPageItem { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyCurrentPageItemDemo
    {
        public static void Run()
        {
            // Create a workbook with sample data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data for pivot table
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Apple";
            worksheet.Cells["A5"].Value = "Orange";
            
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["B4"].Value = "North";
            worksheet.Cells["B5"].Value = "East";
            
            worksheet.Cells["C1"].Value = "Sales";
            worksheet.Cells["C2"].Value = 1000;
            worksheet.Cells["C3"].Value = 2000;
            worksheet.Cells["C4"].Value = 1500;
            worksheet.Cells["C5"].Value = 3000;

            // Create pivot table
            int index = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Add fields
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.AddFieldToArea(PivotFieldType.Page, "Product");
            
            // Refresh data
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Get page fields
            PivotFieldCollection pageFields = pivotTable.PageFields;
            
            // Display current page items
            Console.WriteLine("Initial CurrentPageItem: " + pageFields[0].CurrentPageItem);
            
            // Change current page item
            pageFields[0].CurrentPageItem = 1; // Change to Banana
            Console.WriteLine("After Change CurrentPageItem: " + pageFields[0].CurrentPageItem);
            
            // Save the workbook
            workbook.Save("PivotFieldCurrentPageItemDemo.xlsx");
        }
    }
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


