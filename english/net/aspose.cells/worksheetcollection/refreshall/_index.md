---
title: WorksheetCollection.RefreshAll
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Refresh all pivot tables and charts with pivot source
type: docs
url: /net/aspose.cells/worksheetcollection/refreshall/
---
## WorksheetCollection.RefreshAll method

Refresh all pivot tables and charts with pivot source.

```csharp
public void RefreshAll()
```

### Examples

```csharp
// Called: workbook.Worksheets.RefreshAll();
public void WorksheetCollection_Method_RefreshAll()
{
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    workbook.Worksheets.RefreshAll();
    Cells cells = workbook.Worksheets[0].Cells;
    Assert.IsTrue(Util.CompareColor(Color.FromArgb(146, 208, 80), cells["G8"].GetStyle().ForegroundColor));
    Assert.IsTrue(Util.CompareColor(Color.FromArgb(146, 208, 80), cells["H8"].GetStyle().ForegroundColor));
    Assert.IsTrue(Util.CompareColor(Color.Yellow, cells["J8"].GetStyle().ForegroundColor));
    Assert.IsTrue(Util.CompareColor(Color.Yellow, cells["K8"].GetStyle().ForegroundColor));
}
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


