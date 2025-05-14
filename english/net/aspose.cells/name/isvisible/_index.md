---
title: Name.IsVisible
second_title: Aspose.Cells for .NET API Reference
description: Name property. Indicates whether the name is visible
type: docs
url: /net/aspose.cells/name/isvisible/
---
## Name.IsVisible property

Indicates whether the name is visible.

```csharp
public bool IsVisible { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(nameSrc.IsVisible, nameDest.IsVisible, info + ".IsVisible");
public static void Name_Property_IsVisible(Name nameSrc, Name nameDest, string info)
        {
            if (AssertHelper.checkNull(nameSrc, nameDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(nameSrc.IsReferred, nameDest.IsReferred, info + ".IsReferred");
            AssertHelper.AreEqual(nameSrc.IsVisible, nameDest.IsVisible, info + ".IsVisible");
            AssertHelper.AreEqual(nameSrc.RefersTo, nameDest.RefersTo, info + ".RefersTo");
            AssertHelper.AreEqual(nameSrc.Text, nameDest.Text, info + ".Text");
        }
```

### See Also

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


