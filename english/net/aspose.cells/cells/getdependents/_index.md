---
title: Cells.GetDependents
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Get all cells which refer to the specific cell
type: docs
url: /net/aspose.cells/cells/getdependents/
---
## Cells.GetDependents method

Get all cells which refer to the specific cell.

```csharp
public Cell[] GetDependents(bool isAll, int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| isAll | Boolean | Indicates whether check other worksheets |
| row | Int32 | The row index. |
| column | Int32 | The column index. |

### Examples

```csharp
// Called: cs = cells.GetDependents(true, 0, 0);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Formula/CellsNet40294.xls");
            Cells cells = workbook.Worksheets[0].Cells;
            Cell[] cs = cells.GetDependents(false, 0, 0);
            Assert.AreEqual(cs.Length, 3);
            Assert.AreEqual(cs[0].Name, "B1");
            Assert.AreEqual(cs[1].Name, "C1");
            Assert.AreEqual(cs[2].Name, "F4");
            cs = cells["A1"].GetDependents(false);
            Assert.AreEqual(cs.Length, 3);
            cs = cells.GetDependents(true, 0, 0);
            Assert.AreEqual(cs.Length, 5);
            Assert.AreEqual(cs[0].Name, "B1");
            Assert.AreEqual(cs[1].Name, "C1");
            Assert.AreEqual(cs[2].Name, "F4");
            Assert.AreEqual(cs[3].Name, "B1");
            Assert.AreEqual(cs[4].Name, "D1");
        }
```

### See Also

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


