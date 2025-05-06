---
title: DocumentProperty.Value
second_title: Aspose.Cells for .NET API Reference
description: DocumentProperty property. Gets or sets the value of the property
type: docs
url: /net/aspose.cells.properties/documentproperty/value/
---
## DocumentProperty.Value property

Gets or sets the value of the property.

```csharp
public object Value { get; set; }
```

### Examples

```csharp
// Called: Value.ToString().StartsWith(&amp;quot; &amp;quot;),true);
[Test]
        public void Property_Value()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;xlsx - Hallo.xlsx&quot;);
            Assert.AreEqual(workbook.Worksheets.CustomDocumentProperties[&quot;rox_Meta1&quot;].
                Value.ToString().StartsWith(&quot; &quot;),true);
        }
```

### See Also

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


