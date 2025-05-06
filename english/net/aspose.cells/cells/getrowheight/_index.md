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
// Called: Assert.AreEqual(17, wb.Worksheets[0].Cells.GetRowHeight(1, true, CellsUnitType.Pixel));
[Test]
        public void Method_CellsUnitType_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET56650_1.ods&quot;);
            wb.Worksheets[0].Cells.HideRow(1);
            wb.Save(Constants.destPath + &quot;CELLSNET56698.ods&quot;);
            wb = new Workbook(Constants.destPath + &quot;CELLSNET56698.ods&quot;);
           Assert.AreEqual(85,wb.Worksheets[0].Cells.GetColumnWidth(2, true, CellsUnitType.Pixel));
            Assert.AreEqual(17, wb.Worksheets[0].Cells.GetRowHeight(1, true, CellsUnitType.Pixel));
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
// Called: testAreEqual(0, cells.GetRowHeight(3), caseName);
private void Method_Int32_(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            testAreEqual(0, cells.GetRowHeight(3), caseName);
            testAreEqual(0, cells.GetRowHeight(9), caseName);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


