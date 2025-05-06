---
title: Cell.IsNumericValue
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Indicates whether the value of this cell is numericint double and datetime
type: docs
url: /net/aspose.cells/cell/isnumericvalue/
---
## Cell.IsNumericValue property

Indicates whether the value of this cell is numeric(int, double and datetime)

```csharp
public bool IsNumericValue { get; }
```

### Remarks

Also applies to formula cell to check the calculated result

### Examples

```csharp
// Called: else if (cell == null || !cell.IsNumericValue || cell.IntValue != i - 2)
[Test]
        public void Property_IsNumericValue()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            for (int i = 0; i &lt; 9; i++)
            {
                cells[i, i / 3].PutValue(i + 1);
            }
            wb.DataSorter.Order1 = SortOrder.Descending;
            wb.DataSorter.Key1 = 2; // sort by third data column
            wb.DataSorter.Sort(cells, CellArea.CreateCellArea(0, 0, 8, 2));
            for (int i = 0; i &lt; 3; i++)
            {
                Assert.AreEqual(9 - i, cells[i, 2].IntValue, &quot;C&quot; + (i + 1));
            }
            for (int i = 3; i &lt; 9; i++)
            {
                for (int j = 0; j &lt; 3; j++)
                {
                    Cell cell = cells.CheckCell(i, j);
                    if (j != (i / 3) - 1)
                    {
                        if (cell != null &amp;&amp; cell.Type != CellValueType.IsNull)
                        {
                            Assert.Fail(cell.Name + &quot; should be empty&quot;);
                        }
                    }
                    else if (cell == null || !cell.IsNumericValue || cell.IntValue != i - 2)
                    {
                        Assert.Fail(CellsHelper.CellIndexToName(i, j) + &quot;&apos;s value should be &quot; + (i - 2));
                    }
                }
            }
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


