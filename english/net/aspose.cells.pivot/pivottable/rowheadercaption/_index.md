---
title: PivotTable.RowHeaderCaption
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets and sets custom caption of the Row Header in this PivotTable
type: docs
url: /net/aspose.cells.pivot/pivottable/rowheadercaption/
---
## PivotTable.RowHeaderCaption property

Gets and sets custom caption of the Row Header in this PivotTable.

```csharp
public string RowHeaderCaption { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRowHeaderCaptionDemo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook workbook = new Workbook();
            
            // Add data worksheet
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // Add sample data
            var cells = dataSheet.Cells;
            cells["A1"].PutValue("State");
            cells["B1"].PutValue("City");
            cells["C1"].PutValue("Population");
            
            cells["A2"].PutValue("TN");
            cells["B2"].PutValue("Chennai");
            cells["C2"].PutValue("50");
            
            cells["A3"].PutValue("KL");
            cells["B3"].PutValue("Cochin");
            cells["C3"].PutValue("70");
            
            // Add pivot table worksheet
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Add pivot table and get its index
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Data!A1:C3", 
                "A3", 
                "PivotTable");
            
            // Get the pivot table instance
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            
            // Configure pivot table
            pivotTable.RowHeaderCaption = "State"; // Demonstrating RowHeaderCaption property
            pivotTable.AddFieldToArea(PivotFieldType.Row, "State");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Population");
            
            // Save the workbook
            workbook.Save("PivotTableWithRowHeaderCaption.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


