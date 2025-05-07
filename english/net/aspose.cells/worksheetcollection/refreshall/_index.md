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
[Test]
        public void Method_RefreshAll()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "CellsNet56643.xlsx");
            workbook.Worksheets.RefreshAll();
            Cells cells = workbook.Worksheets[0].Cells;
            Assert.IsTrue(Util.CompareColor(Color.Red, cells["E14"].GetStyle().ForegroundColor));
            Assert.IsTrue(Util.CompareColor(Color.Red, cells["F13"].GetStyle().ForegroundColor));
        }
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


