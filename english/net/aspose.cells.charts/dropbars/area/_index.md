---
title: DropBars.Area
second_title: Aspose.Cells for .NET API Reference
description: DropBars property. Gets the Area
type: docs
url: /net/aspose.cells.charts/dropbars/area/
---
## DropBars.Area property

Gets the `Area`.

```csharp
public Area Area { get; }
```

### Examples

```csharp
// Called: AreaTest.equals(dropbarsSrc.Area, dropbarsDest.Area, info + &amp;quot;.Area&amp;quot;);
public static void Property_Area(DropBars dropbarsSrc, DropBars dropbarsDest, string info)
        {
            if (AssertHelper.checkNull(dropbarsSrc, dropbarsDest, info))
            {
                return;
            }
            LineTest.Property_Area(dropbarsSrc.Border, dropbarsDest.Border, info + &quot;.Border&quot;);
            AreaTest.Property_Area(dropbarsSrc.Area, dropbarsDest.Area, info + &quot;.Area&quot;);
        }
```

### See Also

* class [Area](../../../aspose.cells.drawing/area/)
* class [DropBars](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


