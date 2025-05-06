---
title: DocumentPropertyCollection.Contains
second_title: Aspose.Cells for .NET API Reference
description: DocumentPropertyCollection method. Returns true if a property with the specified name exists in the collection
type: docs
url: /net/aspose.cells.properties/documentpropertycollection/contains/
---
## DocumentPropertyCollection.Contains method

Returns true if a property with the specified name exists in the collection.

```csharp
public bool Contains(string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The case-insensitive name of the property. |

### Return Value

True if the property exists in the collection; false otherwise.

### Examples

```csharp
// Called: Assert.IsFalse(workbook.BuiltInDocumentProperties.Contains(&amp;quot;RevisionNumber&amp;quot;));
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA42769.xlsb&quot;);
            Assert.IsFalse(workbook.BuiltInDocumentProperties.Contains(&quot;RevisionNumber&quot;));
        }
```

### See Also

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


