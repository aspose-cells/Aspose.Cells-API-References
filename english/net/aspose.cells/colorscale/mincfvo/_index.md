---
title: ColorScale.MinCfvo
second_title: Aspose.Cells for .NET API Reference
description: ColorScale property. Get or set this ColorScales min value object. Cannot set null or CFValueObject with type FormatConditionValueType.Max to it
type: docs
url: /net/aspose.cells/colorscale/mincfvo/
---
## ColorScale.MinCfvo property

Get or set this ColorScale's min value object. Cannot set null or CFValueObject with type FormatConditionValueType.Max to it.

```csharp
public ConditionalFormattingValue MinCfvo { get; }
```

### Examples

```csharp
// Called: equals(csSrc.MinCfvo, csDest.MinCfvo, info + &amp;quot;.MinCfvo&amp;quot;);
public static void Property_MinCfvo(ColorScale csSrc, ColorScale csDest, string info)
        {
            if (AssertHelper.checkNull(csSrc, csDest, info))
            {
                return;
            }          
            Property_MinCfvo(csSrc.MaxCfvo, csDest.MaxCfvo, info + &quot;.MaxCfvo&quot;);
            AssertHelper.Property_MinCfvo(csSrc.MaxColor, csDest.MaxColor, info + &quot;.MaxColor&quot;);
            Property_MinCfvo(csSrc.MidCfvo, csDest.MidCfvo, info + &quot;.MidCfvo&quot;);
            AssertHelper.Property_MinCfvo(csSrc.MidColor, csDest.MidColor, info + &quot;.MidColor&quot;);
            Property_MinCfvo(csSrc.MinCfvo, csDest.MinCfvo, info + &quot;.MinCfvo&quot;);
            AssertHelper.Property_MinCfvo(csSrc.MinColor, csDest.MinColor, info + &quot;.MinColor&quot;);
        }
```

### See Also

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


