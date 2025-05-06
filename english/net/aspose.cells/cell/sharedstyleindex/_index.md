---
title: Cell.SharedStyleIndex
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets cells shared style index in the style pool
type: docs
url: /net/aspose.cells/cell/sharedstyleindex/
---
## Cell.SharedStyleIndex property

Gets cell's shared style index in the style pool.

```csharp
public int SharedStyleIndex { get; }
```

### Examples

```csharp
// Called: int xfIndex = workbook.Worksheets[0].Cells[&amp;quot;A1&amp;quot;].SharedStyleIndex;
[Test]
        public void Property_SharedStyleIndex()
        {
            Workbook workbook = new Workbook();
            
            int xfIndex = workbook.Worksheets[0].Cells[&quot;A1&quot;].SharedStyleIndex;
            Style style = workbook.GetStyleInPool(xfIndex);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


