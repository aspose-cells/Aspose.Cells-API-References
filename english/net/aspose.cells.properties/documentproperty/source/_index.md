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
// Called: Assert.AreEqual(property1.Source, property2.Source, &amp;quot;Workbook--DocumentProperty.getSource()&amp;quot;);
private static void Property_Source(
            CustomDocumentPropertyCollection cp1,
            CustomDocumentPropertyCollection cp2)
        {
            Assert.AreEqual(cp1.Count, cp2.Count, &quot;Workbook--CustomDocumentPropertyCollection--Count&quot;);
            for (int i = 0; i &lt; cp1.Count; i++)
            {
                DocumentProperty property1 = cp1[i];
                DocumentProperty property2 = cp2[i];
                Assert.AreEqual(property1.Value, property2.Value, &quot;Workbook--DocumentProperty.getValue()&quot;);
                Assert.AreEqual(property1.Source, property2.Source, &quot;Workbook--DocumentProperty.getSource()&quot;);
                Assert.AreEqual(property1.Type, property2.Type, &quot;Workbook--DocumentProperty.getType()&quot;);
            }
        }
```

### See Also

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


