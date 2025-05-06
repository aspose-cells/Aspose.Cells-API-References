---
title: ColorScale.MaxColor
second_title: Aspose.Cells for .NET API Reference
description: ColorScale property. Get or set the gradient color for the maximum value in the range
type: docs
url: /net/aspose.cells/colorscale/maxcolor/
---
## ColorScale.MaxColor property

Get or set the gradient color for the maximum value in the range.

```csharp
public Color MaxColor { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.equals(csSrc.MaxColor, csDest.MaxColor, info + &amp;quot;.MaxColor&amp;quot;);
public static void Property_MaxColor(ColorScale csSrc, ColorScale csDest, string info)
        {
            if (AssertHelper.checkNull(csSrc, csDest, info))
            {
                return;
            }          
            Property_MaxColor(csSrc.MaxCfvo, csDest.MaxCfvo, info + &quot;.MaxCfvo&quot;);
            AssertHelper.Property_MaxColor(csSrc.MaxColor, csDest.MaxColor, info + &quot;.MaxColor&quot;);
            Property_MaxColor(csSrc.MidCfvo, csDest.MidCfvo, info + &quot;.MidCfvo&quot;);
            AssertHelper.Property_MaxColor(csSrc.MidColor, csDest.MidColor, info + &quot;.MidColor&quot;);
            Property_MaxColor(csSrc.MinCfvo, csDest.MinCfvo, info + &quot;.MinCfvo&quot;);
            AssertHelper.Property_MaxColor(csSrc.MinColor, csDest.MinColor, info + &quot;.MinColor&quot;);
        }
```

### See Also

* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


