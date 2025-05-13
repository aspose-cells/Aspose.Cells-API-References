---
title: Cells.GetMergedAreas
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Gets all merged cells
type: docs
url: /net/aspose.cells/cells/getmergedareas/
---
## Cells.GetMergedAreas method

Gets all merged cells.

```csharp
public CellArea[] GetMergedAreas()
```

### Examples

```csharp
// Called: Assert.AreEqual(wb.Worksheets["Sheet2"].Cells.GetMergedAreas().Length, 17);
public void Cells_Method_GetMergedAreas()
{
    string filePath = Constants.PivotTableSourcePath + @"NET45975_";
    Workbook wb = new Workbook(filePath + "Sample.xlsx");

    wb.Worksheets["Sheet2"].RefreshPivotTables();
    CellArea[] mergeCells = wb.Worksheets["Sheet2"].Cells.GetMergedAreas();
    for (int i = 0; i < mergeCells.Length; i++)
    {
        CellArea area = (CellArea)mergeCells[i];
        Console.WriteLine(area.ToString());
    }
    Assert.AreEqual(wb.Worksheets["Sheet2"].Cells.GetMergedAreas().Length, 17);
}
```

### See Also

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


