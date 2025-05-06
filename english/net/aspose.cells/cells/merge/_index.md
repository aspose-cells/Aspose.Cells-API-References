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
// Called: cells.Merge(2, 2, 3, 2);
[Test]
        public void Method_Int32_()
        {
            caseName = &quot;testMerge_001&quot;;
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.Merge(2, 2, 3, 2);

            checkMerge_001(workbook);
            workbook.Save(Constants.destPath + &quot; testMerge.xls&quot;);            
            workbook = new Workbook(Constants.destPath + &quot; testMerge.xls&quot;);
            checkMerge_001(workbook);
            workbook.Save(Constants.destPath + &quot; testMerge.xlsx&quot;);            
            workbook = new Workbook(Constants.destPath + &quot; testMerge.xlsx&quot;);
            checkMerge_001(workbook);
            workbook.Save(Constants.destPath + &quot; testMerge.xml&quot;, SaveFormat.SpreadsheetML);            
            workbook = new Workbook(Constants.destPath + &quot; testMerge.xml&quot;);
            checkMerge_001(workbook);
            workbook.Save(Constants.destPath + &quot; testMerge.xls&quot;);  
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
// Called: workbook.Worksheets[0].Cells.Merge(3,4,5,2,true);//Range(&amp;quot;E4:F8&amp;quot;).Select
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath +&quot;merge-issue.xls&quot;);
            workbook.Worksheets[0].Cells.Merge(3,4,5,2,true);//Range(&quot;E4:F8&quot;).Select
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
[Test]
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            Cell cell = cells[2, 0];
            cells[0, 1].PutValue(1);
            cells.Merge(0, 1, 2, 2);
            cells.DeleteBlankRows();
            Assert.AreEqual(1, cells.GetMergedAreas().Length, &quot;No options, MergedAreas.Count&quot;);
            AssertHelper.checkCellArea(CellArea.CreateCellArea(0, 1, 0, 2),
                cells.GetMergedAreas()[0], &quot;No options, MergedArea&quot;);

            cell = cells[2, 0];
            cells.Merge(0, 1, 2, 2, true, true);
            DeleteBlankOptions dbo = new DeleteBlankOptions();
            cells.DeleteBlankRows(dbo); //CELLSNET-56864
            Assert.AreEqual(1, cells.GetMergedAreas().Length, &quot;Options with default shrink type, MergedAreas.Count&quot;);
            AssertHelper.checkCellArea(CellArea.CreateCellArea(0, 1, 0, 2),
                cells.GetMergedAreas()[0], &quot;Options with default shrink type, MergedArea&quot;);

            cell = cells[2, 0];
            cells.Merge(0, 1, 2, 2, true, true);
            dbo.MergedCellsShrinkType = MergedCellsShrinkType.None;
            cells.DeleteBlankRows(dbo);
            Assert.AreEqual(1, cells.GetMergedAreas().Length, &quot;Options with shrink type None, MergedAreas.Count&quot;);
            AssertHelper.checkCellArea(CellArea.CreateCellArea(0, 1, 1, 2),
                cells.GetMergedAreas()[0], &quot;Options with shrink type None, MergedArea&quot;);

            cell = cells[2, 0];
            cells.Merge(0, 1, 2, 2, true, true);
            dbo.MergedCellsShrinkType = MergedCellsShrinkType.ShrinkToFit;
            cells.DeleteBlankRows(dbo);
            Assert.AreEqual(1, cells.GetMergedAreas().Length, &quot;Options with ShrinkToFit, MergedAreas.Count&quot;);
            AssertHelper.checkCellArea(CellArea.CreateCellArea(0, 1, 0, 2),
                cells.GetMergedAreas()[0], &quot;Options with ShrinkToFit, MergedArea&quot;);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


