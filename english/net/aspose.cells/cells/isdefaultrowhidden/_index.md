---
title: Cells.IsDefaultRowHidden
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Indicates whether the row is default hidden
type: docs
url: /net/aspose.cells/cells/isdefaultrowhidden/
---
## Cells.IsDefaultRowHidden property

Indicates whether the row is default hidden.

```csharp
public bool IsDefaultRowHidden { get; set; }
```

### Examples

```csharp
// Called: cells.IsDefaultRowHidden = true;
[Test]
        public void Property_IsDefaultRowHidden()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET44291.xlsx&quot;);
            foreach (Worksheet worksheet in workbook.Worksheets)
            {
                Cells cells = worksheet.Cells;
                cells.IsDefaultRowHidden = true;
                //      cells.StandardWidth = 0;
                bool[] cols = new bool[cells.MaxColumn + 1];
                bool[] rows = new bool[cells.MaxRow + 1];
                for (int i = 0; i &lt; rows.Length; i++)
                {
                    rows[i] = true;
                }
                for (int i = 0; i &lt; cols.Length; i++)
                {
                    cols[i] = true;
                }
                foreach (Cell cell in cells)
                {
                    if (cell.Type != CellValueType.IsNull)
                    {
                        cols[cell.Column] = false;
                        rows[cell.Row] = false;
                    }
                }
                foreach (Column col in cells.Columns)
                {
                    if (col.Index &lt; cols.Length)
                    {
                        if (!col.IsHidden)
                        {
                            col.IsHidden = cols[col.Index];
                        }
                    }
                }
                foreach (Row row in cells.Rows)
                {
                    if (row.Index &lt; rows.Length)
                    {
                        if (!row.IsHidden)
                        {
                            row.IsHidden = rows[row.Index];
                        }
                    }
                }
            }
            //for(int i =workbook.Worksheets.Count - 1; i &gt;=2;i--)
            //{

            //    workbook.Worksheets.RemoveAt(i);
            //}
            Assert.IsTrue(workbook.Worksheets[0].Cells.IsRowHidden(50));
            workbook.Save(Constants.destPath + &quot;CELLSNET44291.xlsx&quot;);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


