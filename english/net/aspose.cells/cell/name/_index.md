---
title: Cell.Name
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets the name of the cell
type: docs
url: /net/aspose.cells/cell/name/
---
## Cell.Name property

Gets the name of the cell.

```csharp
public string Name { get; }
```

### Remarks

A cell name includes its column letter and row number. For example, the name of a cell in row 0 and column 0 is A1.

### Examples

```csharp
// Called: Assert.Fail("Lost cell " + cellSrc.Name + ": " + sv);
private void Property_Name(Workbook wb, TxtSaveOptions tso, TxtLoadOptions tlo, string csvTxt)
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

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


