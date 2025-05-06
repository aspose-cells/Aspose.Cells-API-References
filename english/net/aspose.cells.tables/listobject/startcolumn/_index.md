---
title: ListObject.StartColumn
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets the start column of the range
type: docs
url: /net/aspose.cells.tables/listobject/startcolumn/
---
## ListObject.StartColumn property

Gets the start column of the range.

```csharp
public int StartColumn { get; }
```

### Examples

```csharp
// Called: worksheet.Cells[lo.EndRow, lo.StartColumn + 3].PutValue(&amp;quot;B&amp;quot;);
[Test]
        public void Property_StartColumn()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet43364.xlsx&quot;);

            // Get Table 2. This is an empty table. 
            // When the new row is initialized with &apos;PutCellValue&apos;, the VLookup formula is not initialized correctly 
            Worksheet worksheet = workbook.Worksheets[0];
            ListObject lo = worksheet.ListObjects[1];
            lo.Comment = &quot;sdfsdfsdfsdf&quot;;
            lo.PutCellValue((lo.EndRow - lo.StartRow), (lo.StartColumn - lo.StartColumn), 1); // Initialize the Table Formulas 
            worksheet.Cells[lo.EndRow, lo.StartColumn + 1].PutValue(2); // Write values to data row of empty table. 
            worksheet.Cells[lo.EndRow, lo.StartColumn + 3].PutValue(&quot;A&quot;);

            lo.Resize(lo.StartRow, lo.StartColumn, lo.EndRow + 1, lo.EndColumn, true);
            worksheet.Cells[lo.EndRow, lo.StartColumn].PutValue(10); // Write data to second row of table 
            worksheet.Cells[lo.EndRow, lo.StartColumn + 1].PutValue(20);
            worksheet.Cells[lo.EndRow, lo.StartColumn + 3].PutValue(&quot;B&quot;);

            // Get Table 24. This table has a row that was added with the Excel UI. 
            // Call the Resize method to add a new row. This time the VLookup formula is initialized corretly 
            lo = worksheet.ListObjects[2];
            lo.Resize(lo.StartRow, lo.StartColumn, lo.EndRow + 1, lo.EndColumn, true);
            worksheet.Cells[lo.EndRow, lo.StartColumn].PutValue(100); // Write data to second row of table 
            worksheet.Cells[lo.EndRow, lo.StartColumn + 1].PutValue(200);
            worksheet.Cells[lo.EndRow, lo.StartColumn + 3].PutValue(&quot;C&quot;);

            Assert.AreEqual(worksheet.Cells[&quot;D6&quot;].Formula, &quot;=SUM($B6,$C6)&quot;);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            Assert.AreEqual(workbook.Worksheets[0].ListObjects[1].Comment, &quot;sdfsdfsdfsdf&quot;);
        }
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


