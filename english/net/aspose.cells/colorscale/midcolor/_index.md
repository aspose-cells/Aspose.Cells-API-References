---
title: ColorScale.MidColor
second_title: Aspose.Cells for .NET API Reference
description: ColorScale property. Get or set the gradient color for the middle value in the range
type: docs
url: /net/aspose.cells/colorscale/midcolor/
---
## ColorScale.MidColor property

Get or set the gradient color for the middle value in the range.

```csharp
public Color MidColor { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.equals(csSrc.MidColor, csDest.MidColor, info + ".MidColor");
public static void Property_MidColor(ColorScale csSrc, ColorScale csDest, string info)
        {
            if (AssertHelper.checkNull(csSrc, csDest, info))
            {
                return;
            }          
            Property_MidColor(csSrc.MaxCfvo, csDest.MaxCfvo, info + ".MaxCfvo");
            AssertHelper.Property_MidColor(csSrc.MaxColor, csDest.MaxColor, info + ".MaxColor");
            Property_MidColor(csSrc.MidCfvo, csDest.MidCfvo, info + ".MidCfvo");
            AssertHelper.Property_MidColor(csSrc.MidColor, csDest.MidColor, info + ".MidColor");
            Property_MidColor(csSrc.MinCfvo, csDest.MinCfvo, info + ".MinCfvo");
            AssertHelper.Property_MidColor(csSrc.MinColor, csDest.MinColor, info + ".MinColor");
        }
```

### See Also

* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


