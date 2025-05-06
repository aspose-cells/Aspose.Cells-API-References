---
title: DataBar.MinCfvo
second_title: Aspose.Cells for .NET API Reference
description: DataBar property. Get or set this DataBars min value object. Cannot set null or CFValueObject with type FormatConditionValueType.Max to it
type: docs
url: /net/aspose.cells/databar/mincfvo/
---
## DataBar.MinCfvo property

Get or set this DataBar's min value object. Cannot set null or CFValueObject with type FormatConditionValueType.Max to it.

```csharp
public ConditionalFormattingValue MinCfvo { get; }
```

### Examples

```csharp
// Called: equals(databarSrc.MinCfvo, databarDest.MinCfvo, info + &amp;quot;.MinCfvo&amp;quot;);
public static void Property_MinCfvo(DataBar databarSrc, DataBar databarDest, string info)
        {
            if (AssertHelper.checkNull(databarSrc, databarDest, info))
            {
                return;
            }
            AssertHelper.Property_MinCfvo(databarSrc.Color, databarDest.Color, info + &quot;.Color&quot;);
            Property_MinCfvo(databarSrc.MaxCfvo, databarDest.MaxCfvo, info + &quot;.MaxCfvo&quot;);
            Property_MinCfvo(databarSrc.MinCfvo, databarDest.MinCfvo, info + &quot;.MinCfvo&quot;);
            AssertHelper.AreEqual(databarSrc.ShowValue, databarDest.ShowValue, info + &quot;.ShowValue&quot;);
        }
```

### See Also

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


