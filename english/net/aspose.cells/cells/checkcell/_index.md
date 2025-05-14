---
title: Cells.CheckCell
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Gets the Cell element or null at the specified cell row index and column index
type: docs
url: /net/aspose.cells/cells/checkcell/
---
## Cells.CheckCell method

Gets the [`Cell`](../../cell/) element or null at the specified cell row index and column index.

```csharp
public Cell CheckCell(int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index |
| column | Int32 | Column index |

### Return Value

Return Cell object if a Cell object exists. Return null if the cell does not exist.

### Examples

```csharp
// Called: Cell cellDest = cellsDest.CheckCell(cellSrc.Row, cellSrc.Column);
private void Cells_Method_CheckCell(Workbook wb, TxtSaveOptions tso, TxtLoadOptions tlo, string csvTxt)
        {
            string csvResult = SaveAsCsv(wb, tso);
            if (csvTxt != null)
            {
                Assert.AreEqual(csvTxt, csvResult);
            }
            Workbook wb1 = LoadAsCsv(csvResult, tlo);
            Cells cellsSrc = wb.Worksheets[wb.Worksheets.ActiveSheetIndex].Cells;
            Cells cellsDest = wb1.Worksheets[0].Cells;
            IEnumerator en = cellsSrc.GetEnumerator();
            while (en.MoveNext())
            {
                Cell cellSrc = (Cell)en.Current;
                string sv = cellSrc.StringValue;
                if (sv != null)
                {
                    Cell cellDest = cellsDest.CheckCell(cellSrc.Row, cellSrc.Column);
                    if (cellDest == null)
                    {
                        Assert.Fail("Lost cell " + cellSrc.Name + ": " + sv);
                    }
                    Assert.AreEqual(sv, cellDest.StringValue, cellSrc.Name);
                }
            }
        }
```

### See Also

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


