---
title: Range.Value
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets and sets the value of the range
type: docs
url: /net/aspose.cells/range/value/
---
## Range.Value property

Gets and sets the value of the range.

```csharp
public object Value { get; set; }
```

### Remarks

If the range contains multiple cells, the returned/applied object should be a two-dimension Array object.

### Examples

```csharp
// Called: range.Value = new object[,]
[Test]
        public void Property_Value()
        {
            var workbook = new Workbook();
            var worksheet = workbook.Worksheets[0];

            // Populate range            
            var range = worksheet.Cells.CreateRange("B3:D4");
            range.Value = new object[,]
            {
                {"Col1","Col2","Col3" },
                {100,200,300 },
            };

            // Create ListObject
            var firstRow = range.FirstRow;
            var endRow = firstRow + range.RowCount - 1;
            var firstColumn = range.FirstColumn;
            var endColumn = firstColumn + range.ColumnCount - 1;
            worksheet.ListObjects.Add(firstRow, firstColumn, endRow, endColumn, true);

            // Show totals
            worksheet.ListObjects[0].ShowTotals = true;
            Assert.AreEqual("=SUBTOTAL(109,[Col3])", worksheet.Cells["D5"].Formula);
            //workbook.Save(Constants.destPath + "CellsNet44599.xlsx");
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


