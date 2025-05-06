---
title: DocumentProperty.Name
second_title: Aspose.Cells for .NET API Reference
description: DocumentProperty property. Returns the name of the property
type: docs
url: /net/aspose.cells.properties/documentproperty/name/
---
## DocumentProperty.Name property

Returns the name of the property.

```csharp
public string Name { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(dpSrc.Name, dpDest.Name, info + &amp;quot;.Name&amp;quot;);
public static void Property_Name(DocumentProperty dpSrc, DocumentProperty dpDest, string info)
        {
            if (AssertHelper.checkNull(dpSrc, dpDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(dpSrc.Name, dpDest.Name, info + &quot;.Name&quot;);
            AssertHelper.AreEqual(dpSrc.Type, dpDest.Type, info + &quot;.Type&quot;);
            AssertHelper.AreEqual(dpSrc.Value, dpDest.Value, info + &quot;.Value&quot;);
        }
```

### See Also

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


