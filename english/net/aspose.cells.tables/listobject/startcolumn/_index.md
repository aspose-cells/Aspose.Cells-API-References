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
// Called: worksheet.Cells[lo.EndRow, lo.StartColumn + 1].PutValue(2); // Write values to data row of empty table.
[Test]
        public void Property_StartColumn()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET43286.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];
            ListObject lo = worksheet.ListObjects[1];
            lo.PutCellValue((lo.EndRow - lo.StartRow), (lo.StartColumn - lo.StartColumn), 1); // Initialize the Table Formulas 
            worksheet.Cells[lo.EndRow, lo.StartColumn + 1].PutValue(2); // Write values to data row of empty table. 
            worksheet.Cells[lo.EndRow, lo.StartColumn + 3].PutValue("A");

            //lo.Resize(lo.StartRow, lo.StartColumn, lo.EndRow + 1, lo.EndColumn, true);
            lo.PutCellValue((lo.EndRow - lo.StartRow) + 1, (lo.StartColumn - lo.StartColumn), 10); // Write data to second row of table 
            worksheet.Cells[lo.EndRow, lo.StartColumn + 1].PutValue(20);
            worksheet.Cells[lo.EndRow, lo.StartColumn + 3].PutValue("B");

            //// Get Table 24. This table has a row that was added with the Excel UI. 
            //// Call the Resize method to add a new row. This time the VLookup formula is initialized corretly 
            lo = worksheet.ListObjects[2];
            lo.Resize(lo.StartRow, lo.StartColumn, lo.EndRow + 1, lo.EndColumn, true);
            lo.PutCellValue((lo.EndRow - lo.StartRow) + 1, (lo.StartColumn - lo.StartColumn), 100); // Write data to second row of table 
            worksheet.Cells[lo.EndRow, lo.StartColumn + 1].PutValue(200);
            worksheet.Cells[lo.EndRow, lo.StartColumn + 3].PutValue("C");
            workbook.CalculateFormula();
            Assert.AreEqual("A Description", worksheet.Cells["F5"].StringValue);
        }
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


