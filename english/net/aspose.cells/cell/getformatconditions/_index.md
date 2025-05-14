---
title: Cell.GetFormatConditions
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Gets format conditions which applies to this cell
type: docs
url: /net/aspose.cells/cell/getformatconditions/
---
## Cell.GetFormatConditions method

Gets format conditions which applies to this cell.

```csharp
public FormatConditionCollection[] GetFormatConditions()
```

### Return Value

Returns [`FormatConditionCollection`](../../formatconditioncollection/) object

### Examples

```csharp
// Called: Assert.AreEqual(1, cell.GetFormatConditions().Length);
public void Cell_Method_GetFormatConditions()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsb");
    Cells cells = wb.Worksheets[0].Cells;
    cells.InsertColumns(11, 2);
    cells.CopyColumn(cells, 9, 11);
    Cell cell = cells["L81"];
    Assert.AreEqual(1, cell.GetFormatConditions().Length);
    wb = Util.ReSave(wb, SaveFormat.Xlsx);
    //wb.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [FormatConditionCollection](../../formatconditioncollection/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


