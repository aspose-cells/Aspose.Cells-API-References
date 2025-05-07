---
title: Workbook.CountOfStylesInPool
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets number of the styles in the style pool
type: docs
url: /net/aspose.cells/workbook/countofstylesinpool/
---
## Workbook.CountOfStylesInPool property

Gets number of the styles in the style pool.

```csharp
public int CountOfStylesInPool { get; }
```

### Examples

```csharp
// Called: if (wb.CountOfStylesInPool > styleCount)
private void Property_CountOfStylesInPool(Workbook wb, string info, int styleCount)
        {
            IEnumerator enCell = wb.Worksheets[0].Cells.GetEnumerator();
            int sn = 0;
            while (enCell.MoveNext())
            {
                Cell cell = (Cell)enCell.Current;
                if (cell.Row != sn || cell.Column != sn)
                {
                    Assert.Fail(info + "Extra cell-" + cell.Name);
                }
                StyleProcessCell(cell, false, info);
                sn++;
            }
            if (wb.CountOfStylesInPool > styleCount)
            {
                Assert.Fail(info + "Extra styles, original count is " + styleCount + ", current is " + wb.CountOfStylesInPool);
            }
            //check string pool in debug mode here.
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


