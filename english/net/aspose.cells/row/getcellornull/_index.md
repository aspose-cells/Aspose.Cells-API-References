---
title: Row.GetCellOrNull
second_title: Aspose.Cells for .NET API Reference
description: Row method. Gets the cell or null in the specific index
type: docs
url: /net/aspose.cells/row/getcellornull/
---
## Row.GetCellOrNull method

Gets the cell or null in the specific index.

```csharp
public Cell GetCellOrNull(int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | The column index |

### Return Value

Returns the cell object if the cell exists. Or returns null if the cell object does not exist.

### Examples

```csharp
// Called: Cell c1 = row.GetCellOrNull(colIndex);
[Test]
        public void Method_Int32_()
        {
            TxtLoadOptions opts = new TxtLoadOptions(LoadFormat.Auto);
            //using (Workbook wb = new Workbook(Constants.TemplatePath + "Book_test_1.xlsx", opts))
            using (Workbook wb = new Workbook(Constants.TemplatePath + "NetCoreTests/Book_test_1.xlsx"))
            {
                Worksheet ws = wb.Worksheets[wb.Worksheets.ActiveSheetIndex];
                Row row = ws.Cells.Rows[0];
                string s;
                for (int colIndex = 0; colIndex <= ws.Cells.MaxDataColumn; colIndex++)
                {
                    Cell c1 = row.GetCellOrNull(colIndex);
                    s = c1.StringValue;
                }
                object o;
                for (int indexRow = 1; indexRow <= ws.Cells.MaxDataRow; indexRow++)
                {
                    row = ws.Cells.Rows[indexRow];
                    for (int colIndex = 0; colIndex <= ws.Cells.MaxDataColumn; colIndex++)
                    {
                        Cell c1 = row.GetCellOrNull(colIndex);
                        o = c1.Value;
                    }
                }
            }
        }
```

### See Also

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


