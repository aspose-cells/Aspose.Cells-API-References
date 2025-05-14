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
// Called: equals(isSrc.Cfvos, isDest.Cfvos, info + ".Cfvos");
public static void IconSet_Property_Cfvos(IconSet isSrc, IconSet isDest, string info)
        {
            if (AssertHelper.checkNull(isSrc, isDest, info))
            {
                return;
            }
            IconSet_Property_Cfvos(isSrc.Cfvos, isDest.Cfvos, info + ".Cfvos");
            AssertHelper.AreEqual(isSrc.Reverse, isDest.Reverse, info + ".Reverse");
            AssertHelper.AreEqual(isSrc.ShowValue, isDest.ShowValue, info + ".ShowValue");
            AssertHelper.AreEqual(isSrc.Type, isDest.Type, info + ".Type");
        }
```

### See Also

* class [ConditionalFormattingValueCollection](../../conditionalformattingvaluecollection/)
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


