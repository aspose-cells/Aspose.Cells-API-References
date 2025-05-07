---
title: Row.IsHidden
second_title: Aspose.Cells for .NET API Reference
description: Row property. Indicates whether the row is hidden
type: docs
url: /net/aspose.cells/row/ishidden/
---
## Row.IsHidden property

Indicates whether the row is hidden.

```csharp
public bool IsHidden { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(d.Worksheets[0].Cells.Rows[19].IsHidden);
[Test]
        public void Property_IsHidden()
        {
            Workbook d = new Workbook(Constants.sourcePath + "CellsNet57060.xlsx");
           Assert.IsTrue(d.Worksheets[0].Cells.Rows[6].IsHidden);
            Assert.IsTrue(d.Worksheets[0].Cells.Rows[19].IsHidden);
            d.Worksheets[0].RemoveAutoFilter();
            Assert.IsFalse(d.Worksheets[0].Cells.Rows[6].IsHidden);
            Assert.IsTrue(d.Worksheets[0].Cells.Rows[19].IsHidden);
            d.Save(Constants.destPath + "CellsNet57060.xlsx");
        }
```

### See Also

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


