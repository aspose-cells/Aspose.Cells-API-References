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
// Called: AssertHelper.AreEqual(dpSrc.Type, dpDest.Type, info + ".Type");
public static void DocumentProperty_Property_Type(DocumentProperty dpSrc, DocumentProperty dpDest, string info)
        {
            if (AssertHelper.checkNull(dpSrc, dpDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(dpSrc.Name, dpDest.Name, info + ".Name");
            AssertHelper.AreEqual(dpSrc.Type, dpDest.Type, info + ".Type");
            AssertHelper.AreEqual(dpSrc.Value, dpDest.Value, info + ".Value");
        }
```

### See Also

* enum [PropertyType](../../propertytype/)
* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


