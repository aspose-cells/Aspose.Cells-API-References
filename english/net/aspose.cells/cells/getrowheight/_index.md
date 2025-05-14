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
public void Cells_Method_GetRowHeight()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
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
// Called: Assert.AreEqual(cells.GetRowHeight(0), 191.25, 0.01);
public void Cells_Method_GetRowHeight()
{
    Workbook wb = new Workbook();
    string strText = "Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. ";
    strText += "\n\n";
    strText += "Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.";
    strText += "\n\n";
    strText += "Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. ";
    strText += "\n\n";
    strText += "Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.";
    Worksheet ws = wb.Worksheets["Sheet1"];
    Cells cells = ws.Cells;
    Cell cell = cells[0, 0];
    cell.PutValue(strText);
    Style style = cell.GetStyle();
    style.IsTextWrapped = true;
    style.Font.Size = 8;
    style.VerticalAlignment = Aspose.Cells.TextAlignmentType.Bottom;
    cell.SetStyle(style);

    ws.Cells.SetColumnWidth(0, 50);
    ws.AutoFitRows();
    wb.Save(Constants.destPath + "example.xls");
    Assert.AreEqual(cells.GetRowHeight(0), 191.25, 0.01);
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


