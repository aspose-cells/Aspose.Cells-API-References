---
title: ListObject.EndRow
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets the end row of the range
type: docs
url: /net/aspose.cells.tables/listobject/endrow/
---
## ListObject.EndRow property

Gets the end row of the range.

```csharp
public int EndRow { get; }
```

### Examples

```csharp
// Called: worksheet.Cells[lo.EndRow, lo.StartColumn + 3].PutValue(&amp;quot;A&amp;quot;);
[Test]
        public void Property_EndRow()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET43286.xlsx&quot;);
            Worksheet worksheet = workbook.Worksheets[0];
            ListObject lo = worksheet.ListObjects[1];
            lo.PutCellValue((lo.EndRow - lo.StartRow), (lo.StartColumn - lo.StartColumn), 1); // Initialize the Table Formulas 
            worksheet.Cells[lo.EndRow, lo.StartColumn + 1].PutValue(2); // Write values to data row of empty table. 
            worksheet.Cells[lo.EndRow, lo.StartColumn + 3].PutValue(&quot;A&quot;);

            //lo.Resize(lo.StartRow, lo.StartColumn, lo.EndRow + 1, lo.EndColumn, true);
            lo.PutCellValue((lo.EndRow - lo.StartRow) + 1, (lo.StartColumn - lo.StartColumn), 10); // Write data to second row of table 
            worksheet.Cells[lo.EndRow, lo.StartColumn + 1].PutValue(20);
            worksheet.Cells[lo.EndRow, lo.StartColumn + 3].PutValue(&quot;B&quot;);

            //// Get Table 24. This table has a row that was added with the Excel UI. 
            //// Call the Resize method to add a new row. This time the VLookup formula is initialized corretly 
            lo = worksheet.ListObjects[2];
            lo.Resize(lo.StartRow, lo.StartColumn, lo.EndRow + 1, lo.EndColumn, true);
            lo.PutCellValue((lo.EndRow - lo.StartRow) + 1, (lo.StartColumn - lo.StartColumn), 100); // Write data to second row of table 
            worksheet.Cells[lo.EndRow, lo.StartColumn + 1].PutValue(200);
            worksheet.Cells[lo.EndRow, lo.StartColumn + 3].PutValue(&quot;C&quot;);
            workbook.CalculateFormula();
            Assert.AreEqual(&quot;A Description&quot;, worksheet.Cells[&quot;F5&quot;].StringValue);
        }
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


