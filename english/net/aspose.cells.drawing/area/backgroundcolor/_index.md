---
title: Area.BackgroundColor
second_title: Aspose.Cells for .NET API Reference
description: Area property. Gets or sets the background Color of the Area
type: docs
url: /net/aspose.cells.drawing/area/backgroundcolor/
---
## Area.BackgroundColor property

Gets or sets the background Color of the [`Area`](../).

```csharp
public Color BackgroundColor { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.equals(floorSrc.BackgroundColor, floorDest.BackgroundColor, info + &amp;quot;.BackgroundColor&amp;quot;);
public static void Property_BackgroundColor(Floor floorSrc, Floor floorDest, string info)
        {
            if (AssertHelper.checkNull(floorSrc, floorDest, info))
            {
                return;
            }
            LineTest.Property_BackgroundColor(floorSrc.Border, floorDest.Border, info + &quot;.Border&quot;);            
            AssertHelper.AreEqual(floorSrc.Formatting, floorDest.Formatting, info + &quot;.Formatting&quot;);
            if (floorSrc.Formatting == FormattingType.Custom)
            {
                FillFormatTest.Property_BackgroundColor(floorSrc.FillFormat, floorDest.FillFormat, info + &quot;.FillFormat&quot;);
                AssertHelper.Property_BackgroundColor(floorSrc.ForegroundColor, floorDest.ForegroundColor, info + &quot;.ForegroundColor&quot;);
                AssertHelper.Property_BackgroundColor(floorSrc.BackgroundColor, floorDest.BackgroundColor, info + &quot;.BackgroundColor&quot;);
            }
            AssertHelper.AreEqual(floorSrc.InvertIfNegative, floorDest.InvertIfNegative, info + &quot;.InvertIfNegative&quot;);
        }
```

### See Also

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


