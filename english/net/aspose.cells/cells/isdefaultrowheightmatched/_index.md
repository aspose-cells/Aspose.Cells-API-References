---
title: Cells.IsDefaultRowHeightMatched
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Indicates that row height and default font height matches
type: docs
url: /net/aspose.cells/cells/isdefaultrowheightmatched/
---
## Cells.IsDefaultRowHeightMatched property

Indicates that row height and default font height matches

```csharp
public bool IsDefaultRowHeightMatched { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(cells.IsDefaultRowHeightMatched);
public void Cells_Property_IsDefaultRowHeightMatched(){
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    cells.IsDefaultRowHidden = false;
    Assert.IsTrue(cells.IsDefaultRowHeightMatched);
    Assert.IsFalse(cells.IsDefaultRowHidden);
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    cells = workbook.Worksheets[0].Cells;
    Assert.IsTrue(cells.IsDefaultRowHeightMatched);
    Assert.IsFalse(cells.IsDefaultRowHidden);
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


