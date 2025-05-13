---
title: IconSet.Reverse
second_title: Aspose.Cells for .NET API Reference
description: IconSet property. Get or set the flag indicating whether to reverses the default order of the icons in this icon set. Default value is false
type: docs
url: /net/aspose.cells/iconset/reverse/
---
## IconSet.Reverse property

Get or set the flag indicating whether to reverses the default order of the icons in this icon set. Default value is false.

```csharp
public bool Reverse { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(isSrc.Reverse, isDest.Reverse, info + ".Reverse");
public static void IconSet_Property_Reverse(IconSet isSrc, IconSet isDest, string info)
        {
            if (AssertHelper.checkNull(isSrc, isDest, info))
            {
                return;
            }
            IconSet_Property_Reverse(isSrc.Cfvos, isDest.Cfvos, info + ".Cfvos");
            AssertHelper.AreEqual(isSrc.Reverse, isDest.Reverse, info + ".Reverse");
            AssertHelper.AreEqual(isSrc.ShowValue, isDest.ShowValue, info + ".ShowValue");
            AssertHelper.AreEqual(isSrc.Type, isDest.Type, info + ".Type");
        }
```

### See Also

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


