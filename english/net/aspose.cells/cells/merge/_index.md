---
title: Cells.Merge
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Merges a specified range of cells into a single cell
type: docs
url: /net/aspose.cells/cells/merge/
---
## Merge(int, int, int, int) {#merge}

Merges a specified range of cells into a single cell.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | First row of this range(zero based) |
| firstColumn | Int32 | First column of this range(zero based) |
| totalRows | Int32 | Number of rows(one based) |
| totalColumns | Int32 | Number of columns(one based) |

### Remarks

Reference the merged cell via the address of the upper-left cell in the range.

### Examples

```csharp
// Called: cells.Merge(0, 0, 65536, 1);
		public void Cells_Method_Merge()
		{
			Workbook excel = new Workbook();
			Cells cells = excel.Worksheets[0].Cells;
			cells["g1"].PutValue("hello");
			cells.Merge(0, 0, 1, 256);

			excel.Save(Constants.destPath + "mergerow.xls");

			excel = new Workbook();
			cells = excel.Worksheets[0].Cells;

			cells["a11"].PutValue(123);

			cells.Merge(0, 0, 65536, 1);

			excel.Save(Constants.destPath + "mergecolumn.xls");



		}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Merge(int, int, int, int, bool) {#merge_1}

Merges a specified range of cells into a single cell.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool mergeConflict)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | First row of this range(zero based) |
| firstColumn | Int32 | First column of this range(zero based) |
| totalRows | Int32 | Number of rows(one based) |
| totalColumns | Int32 | Number of columns(one based) |
| mergeConflict | Boolean | Merge conflict merged ranges. |

### Remarks

Reference the merged cell via the address of the upper-left cell in the range. If mergeConflict is true and the merged range conflicts with other merged cells, other merged cells will be automatically removed.

### Examples

```csharp
// Called: workbook.Worksheets[0].Cells.Merge(3,4,5,2,true);//Range("E4:F8").Select
public void Cells_Method_Merge()
{
    Workbook workbook = new Workbook(Constants.sourcePath +"merge-issue.xls");
    workbook.Worksheets[0].Cells.Merge(3,4,5,2,true);//Range("E4:F8").Select
    Assert.AreEqual(workbook.Worksheets[0].Cells.GetMergedAreas().Length, 1);

}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Merge(int, int, int, int, bool, bool) {#merge_2}

Merges a specified range of cells into a single cell.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool checkConflict, bool mergeConflict)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | First row of this range(zero based) |
| firstColumn | Int32 | First column of this range(zero based) |
| totalRows | Int32 | Number of rows(one based) |
| totalColumns | Int32 | Number of columns(one based) |
| checkConflict | Boolean | Indicates whether check the merged cells intersects other merged cells |
| mergeConflict | Boolean | Merge conflict merged ranges. |

### Remarks

Reference the merged cell via the address of the upper-left cell in the range. If mergeConflict is true and the merged range conflicts with other merged cells, other merged cells will be automatically removed.

### Examples

```csharp
// Called: cells.Merge(0, 1, 2, 2, true, true);
public void Cells_Method_Merge()
{
    Workbook wb = new Workbook();
    Cells cells = wb.Worksheets[0].Cells;
    Cell cell = cells[2, 0];
    cells[0, 1].PutValue(1);
    cells.Merge(0, 1, 2, 2);
    cells.DeleteBlankRows();
    Assert.AreEqual(1, cells.GetMergedAreas().Length, "No options, MergedAreas.Count");
    AssertHelper.checkCellArea(CellArea.CreateCellArea(0, 1, 0, 2),
        cells.GetMergedAreas()[0], "No options, MergedArea");

    cell = cells[2, 0];
    cells.Merge(0, 1, 2, 2, true, true);
    DeleteBlankOptions dbo = new DeleteBlankOptions();
    cells.DeleteBlankRows(dbo); //CELLSNET-56864
    Assert.AreEqual(1, cells.GetMergedAreas().Length, "Options with default shrink type, MergedAreas.Count");
    AssertHelper.checkCellArea(CellArea.CreateCellArea(0, 1, 0, 2),
        cells.GetMergedAreas()[0], "Options with default shrink type, MergedArea");

    cell = cells[2, 0];
    cells.Merge(0, 1, 2, 2, true, true);
    dbo.MergedCellsShrinkType = MergedCellsShrinkType.None;
    cells.DeleteBlankRows(dbo);
    Assert.AreEqual(1, cells.GetMergedAreas().Length, "Options with shrink type None, MergedAreas.Count");
    AssertHelper.checkCellArea(CellArea.CreateCellArea(0, 1, 1, 2),
        cells.GetMergedAreas()[0], "Options with shrink type None, MergedArea");

    cell = cells[2, 0];
    cells.Merge(0, 1, 2, 2, true, true);
    dbo.MergedCellsShrinkType = MergedCellsShrinkType.ShrinkToFit;
    cells.DeleteBlankRows(dbo);
    Assert.AreEqual(1, cells.GetMergedAreas().Length, "Options with ShrinkToFit, MergedAreas.Count");
    AssertHelper.checkCellArea(CellArea.CreateCellArea(0, 1, 0, 2),
        cells.GetMergedAreas()[0], "Options with ShrinkToFit, MergedArea");
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


