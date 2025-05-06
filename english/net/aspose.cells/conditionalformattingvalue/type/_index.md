---
title: ConditionalFormattingValue.Type
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingValue property. Get or set the type of this conditional formatting value object. Setting the type to FormatConditionValueType.Min or FormatConditionValueType.Max will auto set Value to null
type: docs
url: /net/aspose.cells/conditionalformattingvalue/type/
---
## ConditionalFormattingValue.Type property

Get or set the type of this conditional formatting value object. Setting the type to FormatConditionValueType.Min or FormatConditionValueType.Max will auto set "Value" to null.

```csharp
public FormatConditionValueType Type { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(cfoSrc.Type, cfoDest.Type, info + &amp;quot;.Type&amp;quot;);
public static void Property_Type(ConditionalFormattingValue cfoSrc, ConditionalFormattingValue cfoDest, string info)
        {
            if (AssertHelper.checkNull(cfoSrc, cfoDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(cfoSrc.IsGTE, cfoDest.IsGTE, info + &quot;.IsGTE&quot;);
            AssertHelper.AreEqual(cfoSrc.Type, cfoDest.Type, info + &quot;.Type&quot;);
            AssertHelper.AreEqual(cfoSrc.Value, cfoDest.Value, info + &quot;.Value&quot;);
        }
```

### See Also

* enum [FormatConditionValueType](../../formatconditionvaluetype/)
* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


