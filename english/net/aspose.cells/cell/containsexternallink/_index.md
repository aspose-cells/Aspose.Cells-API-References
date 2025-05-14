---
title: Cell.ContainsExternalLink
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Indicates whether this cell contains an external link. Only applies when the cell is a formula cell
type: docs
url: /net/aspose.cells/cell/containsexternallink/
---
## Cell.ContainsExternalLink property

Indicates whether this cell contains an external link. Only applies when the cell is a formula cell.

```csharp
public bool ContainsExternalLink { get; }
```

### Examples

```csharp
// Called: Assert.IsFalse(sheet.Cells["C3"].ContainsExternalLink);
public void Cell_Property_ContainsExternalLink()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    var sheet = workbook.Worksheets[0]; 
    Assert.IsFalse(sheet.Cells["C3"].ContainsExternalLink);
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


