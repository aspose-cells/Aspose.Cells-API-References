---
title: PivotTableFormatCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: PivotTableFormatCollection property. Gets the format by the index
type: docs
url: /net/aspose.cells.pivot/pivottableformatcollection/item/
---
## PivotTableFormatCollection indexer

Gets the format by the index.

```csharp
public PivotTableFormat this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Examples

```csharp
// Called: PivotTableFormat pivotFormat = pivotFormats[formatIndex];
public static void Property_Int32_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some sample data
            sheet.Cells[&quot;A1&quot;].PutValue(&quot;Category&quot;);
            sheet.Cells[&quot;A2&quot;].PutValue(&quot;Fruit&quot;);
            sheet.Cells[&quot;A3&quot;].PutValue(&quot;Vegetable&quot;);
            sheet.Cells[&quot;B1&quot;].PutValue(&quot;Amount&quot;);
            sheet.Cells[&quot;B2&quot;].PutValue(50);
            sheet.Cells[&quot;B3&quot;].PutValue(30);

            // Add a pivot table
            int pivotIndex = sheet.PivotTables.Add(&quot;A1:B3&quot;, &quot;E5&quot;, &quot;PivotTable1&quot;);
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // Access the PivotTableFormatCollection
            PivotTableFormatCollection pivotFormats = pivotTable.PivotFormats;

            // Add a new format to the collection
            int formatIndex = pivotFormats.Add();
            PivotTableFormat pivotFormat = pivotFormats[formatIndex];

            // Access the PivotArea of the format
            PivotArea pivotArea = pivotFormat.PivotArea;
            pivotArea.AxisType = PivotFieldType.Data;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;

            // Create a new style
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // Apply the style to the PivotTableFormat
            pivotFormat.SetStyle(style);

            // Save the workbook
            workbook.Save(&quot;PivotTableFormatDemo.xlsx&quot;);
        }
```

### See Also

* class [PivotTableFormat](../../pivottableformat/)
* class [PivotTableFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


