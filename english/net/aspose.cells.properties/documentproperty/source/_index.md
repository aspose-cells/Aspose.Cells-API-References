---
title: DocumentProperty.Source
second_title: Aspose.Cells for .NET API Reference
description: DocumentProperty property. The linked content source
type: docs
url: /net/aspose.cells.properties/documentproperty/source/
---
## DocumentProperty.Source property

The linked content source.

```csharp
public string Source { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(property1.Source, property2.Source, "Workbook--DocumentProperty.getSource()");
private static void DocumentProperty_Property_Source(
            CustomDocumentPropertyCollection cp1,
            CustomDocumentPropertyCollection cp2)
        {
            Assert.AreEqual(cp1.Count, cp2.Count, "Workbook--CustomDocumentPropertyCollection--Count");
            for (int i = 0; i < cp1.Count; i++)
            {
                DocumentProperty property1 = cp1[i];
                DocumentProperty property2 = cp2[i];
                Assert.AreEqual(property1.Value, property2.Value, "Workbook--DocumentProperty.getValue()");
                Assert.AreEqual(property1.Source, property2.Source, "Workbook--DocumentProperty.getSource()");
                Assert.AreEqual(property1.Type, property2.Type, "Workbook--DocumentProperty.getType()");
            }
        }
```

### See Also

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


