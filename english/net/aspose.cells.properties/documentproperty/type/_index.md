---
title: DocumentProperty.Type
second_title: Aspose.Cells for .NET API Reference
description: DocumentProperty property. Gets the data type of the property
type: docs
url: /net/aspose.cells.properties/documentproperty/type/
---
## DocumentProperty.Type property

Gets the data type of the property.

```csharp
public PropertyType Type { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(dpSrc.Type, dpDest.Type, info + &amp;quot;.Type&amp;quot;);
public static void Property_Type(DocumentProperty dpSrc, DocumentProperty dpDest, string info)
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

* enum [PropertyType](../../propertytype/)
* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


