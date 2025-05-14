---
title: CellArea.EndRow
second_title: Aspose.Cells for .NET API Reference
description: CellArea field. Gets or set the end row of this area
type: docs
url: /net/aspose.cells/cellarea/endrow/
---
## CellArea.EndRow field

Gets or set the end row of this area.

```csharp
public int EndRow;
```

### Examples

```csharp
// Called: Assert.AreEqual(10, pt.TableRange2.EndRow);
public void CellArea_Field_EndRow()
{
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + @"example.xls");
    workbook.Save(Constants.PivotTableDestPath + "example.ods");
    workbook = new Workbook(Constants.PivotTableDestPath + "example.ods");
    PivotTable pt = workbook.Worksheets[0].PivotTables[0];
    Assert.AreEqual(10, pt.TableRange2.EndRow);
    Assert.AreEqual(ConsolidationFunction.Count, pt.DataFields[0].Function);
    workbook.Worksheets.RefreshAll();
    Assert.AreEqual("Count of b", workbook.Worksheets[0].Cells["F8"].StringValue);
          
}
```

### See Also

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


