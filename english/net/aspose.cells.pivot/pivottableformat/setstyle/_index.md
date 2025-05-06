---
title: PivotTableFormat.SetStyle
second_title: Aspose.Cells for .NET API Reference
description: PivotTableFormat method. Sets the style of the pivot area
type: docs
url: /net/aspose.cells.pivot/pivottableformat/setstyle/
---
## PivotTableFormat.SetStyle method

Sets the style of the pivot area.

```csharp
public void SetStyle(Style style)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style |  |

### Examples

```csharp
// Called: newFormat.SetStyle(style);
public static void Method_Style_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells[0, 0].Value = &quot;Fruit&quot;;
            worksheet.Cells[0, 1].Value = &quot;Year&quot;;
            worksheet.Cells[0, 2].Value = &quot;Amount&quot;;
            worksheet.Cells[1, 0].Value = &quot;Apple&quot;;
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 0].Value = &quot;Banana&quot;;
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 0].Value = &quot;Apple&quot;;
            worksheet.Cells[3, 1].Value = 2021;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 0].Value = &quot;Banana&quot;;
            worksheet.Cells[4, 1].Value = 2021;
            worksheet.Cells[4, 2].Value = 80;

            // Add a pivot table to the worksheet
            int pivotIndex = worksheet.PivotTables.Add(&quot;=Sheet1!A1:C5&quot;, &quot;E5&quot;, &quot;PivotTable1&quot;);
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Access the PivotTableFormatCollection
            PivotTableFormatCollection formatCollection = pivotTable.PivotFormats;

            // Add a format to the collection
            int formatIndex = formatCollection.Add();
            PivotTableFormat pivotFormat = formatCollection[formatIndex];

            // Define the format area
            PivotTableFormat newFormat = formatCollection.FormatArea(PivotFieldType.Row, 0, PivotFieldSubtotalType.None, PivotTableSelectionType.DataAndLabel, false, false, new Style());

            // Set the style for the format
            Style style = new Style();
            style.BackgroundColor = Color.LightBlue;
            newFormat.SetStyle(style);

            // Save the workbook
            workbook.Save(&quot;PivotTableFormatCollectionExample.xlsx&quot;);
        }
```

### See Also

* class [Style](../../../aspose.cells/style/)
* class [PivotTableFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


