---
title: ListObject.Comment
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets and sets the comment of the table
type: docs
url: /net/aspose.cells.tables/listobject/comment/
---
## ListObject.Comment property

Gets and sets the comment of the table.

```csharp
public string Comment { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].ListObjects[1].Comment, "sdfsdfsdfsdf");
[Test]
        public void Property_Comment()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet43364.xlsx");

            // Get Table 2. This is an empty table. 
            // When the new row is initialized with 'PutCellValue', the VLookup formula is not initialized correctly 
            Worksheet worksheet = workbook.Worksheets[0];
            ListObject lo = worksheet.ListObjects[1];
            lo.Comment = "sdfsdfsdfsdf";
            lo.PutCellValue((lo.EndRow - lo.StartRow), (lo.StartColumn - lo.StartColumn), 1); // Initialize the Table Formulas 
            worksheet.Cells[lo.EndRow, lo.StartColumn + 1].PutValue(2); // Write values to data row of empty table. 
            worksheet.Cells[lo.EndRow, lo.StartColumn + 3].PutValue("A");

            lo.Resize(lo.StartRow, lo.StartColumn, lo.EndRow + 1, lo.EndColumn, true);
            worksheet.Cells[lo.EndRow, lo.StartColumn].PutValue(10); // Write data to second row of table 
            worksheet.Cells[lo.EndRow, lo.StartColumn + 1].PutValue(20);
            worksheet.Cells[lo.EndRow, lo.StartColumn + 3].PutValue("B");

            // Get Table 24. This table has a row that was added with the Excel UI. 
            // Call the Resize method to add a new row. This time the VLookup formula is initialized corretly 
            lo = worksheet.ListObjects[2];
            lo.Resize(lo.StartRow, lo.StartColumn, lo.EndRow + 1, lo.EndColumn, true);
            worksheet.Cells[lo.EndRow, lo.StartColumn].PutValue(100); // Write data to second row of table 
            worksheet.Cells[lo.EndRow, lo.StartColumn + 1].PutValue(200);
            worksheet.Cells[lo.EndRow, lo.StartColumn + 3].PutValue("C");

            Assert.AreEqual(worksheet.Cells["D6"].Formula, "=SUM($B6,$C6)");
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            Assert.AreEqual(workbook.Worksheets[0].ListObjects[1].Comment, "sdfsdfsdfsdf");
        }
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


