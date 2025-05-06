---
title: IconSet.Cfvos
second_title: Aspose.Cells for .NET API Reference
description: IconSet property. Get the CFValueObjects instance
type: docs
url: /net/aspose.cells/iconset/cfvos/
---
## IconSet.Cfvos property

Get the CFValueObjects instance.

```csharp
public ConditionalFormattingValueCollection Cfvos { get; }
```

### Examples

```csharp
// Called: equals(isSrc.Cfvos, isDest.Cfvos, info + &amp;quot;.Cfvos&amp;quot;);
public static void Property_Cfvos(IconSet isSrc, IconSet isDest, string info)
        {
            if (AssertHelper.checkNull(isSrc, isDest, info))
            {
                return;
            }
            Property_Cfvos(isSrc.Cfvos, isDest.Cfvos, info + &quot;.Cfvos&quot;);
            AssertHelper.AreEqual(isSrc.Reverse, isDest.Reverse, info + &quot;.Reverse&quot;);
            AssertHelper.AreEqual(isSrc.ShowValue, isDest.ShowValue, info + &quot;.ShowValue&quot;);
            AssertHelper.AreEqual(isSrc.Type, isDest.Type, info + &quot;.Type&quot;);
        }
```

### See Also

* class [ConditionalFormattingValueCollection](../../conditionalformattingvaluecollection/)
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


