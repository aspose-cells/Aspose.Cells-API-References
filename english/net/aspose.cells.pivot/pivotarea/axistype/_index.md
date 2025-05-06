---
title: PivotArea.AxisType
second_title: Aspose.Cells for .NET API Reference
description: PivotArea property. Gets and sets the region of the PivotTable to which this rule applies
type: docs
url: /net/aspose.cells.pivot/pivotarea/axistype/
---
## PivotArea.AxisType property

Gets and sets the region of the PivotTable to which this rule applies.

```csharp
public PivotFieldType AxisType { get; set; }
```

### Examples

```csharp
// Called: pivotArea.AxisType = PivotFieldType.Row;
public static void Property_AxisType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells[0, 0].Value = &quot;Fruit&quot;;
            worksheet.Cells[1, 0].Value = &quot;Apple&quot;;
            worksheet.Cells[2, 0].Value = &quot;Banana&quot;;
            worksheet.Cells[3, 0].Value = &quot;Cherry&quot;;
            worksheet.Cells[0, 1].Value = &quot;Year&quot;;
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2021;
            worksheet.Cells[3, 1].Value = 2022;
            worksheet.Cells[0, 2].Value = &quot;Amount&quot;;
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;

            // Add a pivot table to the worksheet
            int pivotIndex = worksheet.PivotTables.Add(&quot;=Sheet1!A1:C4&quot;, &quot;E5&quot;, &quot;PivotTable1&quot;);
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Create a PivotArea instance
            PivotArea pivotArea = new PivotArea(pivotTable);

            // Set properties of the PivotArea
            pivotArea.OnlyData = true;
            pivotArea.OnlyLabel = false;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.IsOutline = false;

            // Use the Select method to select a specific area
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.DataAndLabel);

            // Save the workbook
            workbook.Save(&quot;PivotAreaExample.xlsx&quot;);
        }
```

### See Also

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


