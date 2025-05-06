---
title: PivotArea.IsOutline
second_title: Aspose.Cells for .NET API Reference
description: PivotArea property. Indicates whether the rule refers to an area that is in outline mode
type: docs
url: /net/aspose.cells.pivot/pivotarea/isoutline/
---
## PivotArea.IsOutline property

Indicates whether the rule refers to an area that is in outline mode.

```csharp
public bool IsOutline { get; set; }
```

### Examples

```csharp
// Called: pivotArea.IsOutline = false;
public static void Property_IsOutline()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data for the PivotTable
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Category&quot;);
            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Sales&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;A&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(100);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;B&quot;);
            worksheet.Cells[&quot;B3&quot;].PutValue(150);
            worksheet.Cells[&quot;A4&quot;].PutValue(&quot;A&quot;);
            worksheet.Cells[&quot;B4&quot;].PutValue(200);
            worksheet.Cells[&quot;A5&quot;].PutValue(&quot;B&quot;);
            worksheet.Cells[&quot;B5&quot;].PutValue(250);

            // Create a PivotTable
            int pivotIndex = worksheet.PivotTables.Add(&quot;A1:B5&quot;, &quot;D1&quot;, &quot;PivotTable1&quot;);
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add fields to the PivotTable
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Create a PivotArea and set its properties
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.OnlyData = false;
            pivotArea.OnlyLabel = true;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;
            pivotArea.IsOutline = false;

            // Select the area with specific selection type
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);

            // Save the workbook
            workbook.Save(&quot;PivotTableSelectionTypeExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


