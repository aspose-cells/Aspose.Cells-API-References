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
// Called: AssertHelper.AreEqual(dpSrc.Name, dpDest.Name, info + ".Name");
public static void Property_Name(DocumentProperty dpSrc, DocumentProperty dpDest, string info)
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

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


