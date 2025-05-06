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
// Called: Assert.IsFalse(sheet.Cells[&amp;quot;C3&amp;quot;].ContainsExternalLink);
[Test]
        public void Property_ContainsExternalLink()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet44239.xlsx&quot;);
            var sheet = workbook.Worksheets[0]; 
            Assert.IsFalse(sheet.Cells[&quot;C3&quot;].ContainsExternalLink);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


