---
title: Cells.GetRowHeight
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Gets rows height
type: docs
url: /net/aspose.cells/cells/getrowheight/
---
## GetRowHeight(int, bool, CellsUnitType) {#getrowheight_1}

Gets row's height.

```csharp
public double GetRowHeight(int row, bool isOriginal, CellsUnitType unitType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| isOriginal | Boolean | Whether returns the original row height or 0 for hidden row. |
| unitType | CellsUnitType | Unit type of the returned height value |

### Return Value

Row's height

### Examples

```csharp
// Called: Assert.AreEqual(20, workbook.Worksheets[0].Cells.GetRowHeight(3,true,CellsUnitType.Pixel));
[Test]
        public void Method_CellsUnitType_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsJava45881.xlsx");
            Assert.AreEqual(20, workbook.Worksheets[0].Cells.GetRowHeight(3,true,CellsUnitType.Pixel));
            Assert.AreEqual(64, workbook.Worksheets[0].Cells.GetColumnWidth(2,true, CellsUnitType.Point) * 96 / 72);
        }
```

### See Also

* enum [CellsUnitType](../../cellsunittype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRowHeight(int) {#getrowheight}

Gets the height of a specified row, in unit of points.

```csharp
public double GetRowHeight(int row)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index |

### Return Value

Height of row

### Examples

```csharp
// Called: AssertHelper.AreEqual(0, cells.GetRowHeight(3), "cells.GetRowHeight(3)");
private void Method_Int32_(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            AssertHelper.AreEqual(0, cells.GetRowHeight(3), "cells.GetRowHeight(3)");
            AssertHelper.AreEqual(0, cells.GetRowHeight(9), "cells.GetRowHeight(9)");
            AssertHelper.AreEqual(0, cells.GetColumnWidth(4), "cells.GetColumnWidth(4)");
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


