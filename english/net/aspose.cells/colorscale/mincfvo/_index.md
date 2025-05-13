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
// Called: equals(csSrc.MinCfvo, csDest.MinCfvo, info + ".MinCfvo");
public static void ColorScale_Property_MinCfvo(ColorScale csSrc, ColorScale csDest, string info)
        {
            if (AssertHelper.checkNull(csSrc, csDest, info))
            {
                return;
            }          
            ColorScale_Property_MinCfvo(csSrc.MaxCfvo, csDest.MaxCfvo, info + ".MaxCfvo");
            AssertHelper.ColorScale_Property_MinCfvo(csSrc.MaxColor, csDest.MaxColor, info + ".MaxColor");
            ColorScale_Property_MinCfvo(csSrc.MidCfvo, csDest.MidCfvo, info + ".MidCfvo");
            AssertHelper.ColorScale_Property_MinCfvo(csSrc.MidColor, csDest.MidColor, info + ".MidColor");
            ColorScale_Property_MinCfvo(csSrc.MinCfvo, csDest.MinCfvo, info + ".MinCfvo");
            AssertHelper.ColorScale_Property_MinCfvo(csSrc.MinColor, csDest.MinColor, info + ".MinColor");
        }
```

### See Also

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


