---
title: DropBars.Border
second_title: Aspose.Cells for .NET API Reference
description: DropBars property. Gets the border Line
type: docs
url: /net/aspose.cells.charts/dropbars/border/
---
## DropBars.Border property

Gets the border [`Line`](../../../aspose.cells.drawing/line/).

```csharp
public Line Border { get; }
```

### Examples

```csharp
// Called: LineTest.equals(dropbarsSrc.Border, dropbarsDest.Border, info + ".Border");
public static void Property_Border(DropBars dropbarsSrc, DropBars dropbarsDest, string info)
        {
            if (AssertHelper.checkNull(dropbarsSrc, dropbarsDest, info))
            {
                return;
            }
            LineTest.Property_Border(dropbarsSrc.Border, dropbarsDest.Border, info + ".Border");
            AreaTest.Property_Border(dropbarsSrc.Area, dropbarsDest.Area, info + ".Area");
        }
```

### See Also

* class [Line](../../../aspose.cells.drawing/line/)
* class [DropBars](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


