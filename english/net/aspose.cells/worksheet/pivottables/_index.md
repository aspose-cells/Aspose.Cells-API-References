---
title: Worksheet.PivotTables
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets all pivot tables in this worksheet
type: docs
url: /net/aspose.cells/worksheet/pivottables/
---
## Worksheet.PivotTables property

Gets all pivot tables in this worksheet.

```csharp
public PivotTableCollection PivotTables { get; }
```

### Examples

```csharp
// Called: PivotTableCollection pivotTables = worksheet.PivotTables;
public static void Property_PivotTables()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells[0, 0].Value = &quot;Fruit&quot;;
            worksheet.Cells[0, 1].Value = &quot;Year&quot;;
            worksheet.Cells[0, 2].Value = &quot;Amount&quot;;
            worksheet.Cells[1, 0].Value = &quot;Apple&quot;;
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 0].Value = &quot;Banana&quot;;
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 0].Value = &quot;Cherry&quot;;
            worksheet.Cells[3, 1].Value = 2021;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 0].Value = &quot;Date&quot;;
            worksheet.Cells[4, 1].Value = 2021;
            worksheet.Cells[4, 2].Value = 80;

            // Add a pivot table to the worksheet
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add(&quot;=Sheet1!A1:C5&quot;, &quot;E3&quot;, &quot;PivotTable1&quot;);
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Set the pivot table style type
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Save the workbook
            workbook.Save(&quot;PivotTableStyleTypeExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [PivotTableCollection](../../../aspose.cells.pivot/pivottablecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


