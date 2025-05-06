---
title: Name.IsReferred
second_title: Aspose.Cells for .NET API Reference
description: Name property. Indicates whether this name is referred by other formulas
type: docs
url: /net/aspose.cells/name/isreferred/
---
## Name.IsReferred property

Indicates whether this name is referred by other formulas.

```csharp
public bool IsReferred { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(nameSrc.IsReferred, nameDest.IsReferred, info + &amp;quot;.IsReferred&amp;quot;);
public static void Property_IsReferred(Name nameSrc, Name nameDest, string info)
        {
            if (AssertHelper.checkNull(nameSrc, nameDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(nameSrc.IsReferred, nameDest.IsReferred, info + &quot;.IsReferred&quot;);
            AssertHelper.AreEqual(nameSrc.IsVisible, nameDest.IsVisible, info + &quot;.IsVisible&quot;);
            AssertHelper.AreEqual(nameSrc.RefersTo, nameDest.RefersTo, info + &quot;.RefersTo&quot;);
            AssertHelper.AreEqual(nameSrc.Text, nameDest.Text, info + &quot;.Text&quot;);
        }
```

### See Also

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


