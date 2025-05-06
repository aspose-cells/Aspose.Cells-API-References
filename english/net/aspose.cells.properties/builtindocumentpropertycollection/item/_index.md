---
title: BuiltInDocumentPropertyCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Returns a DocumentProperty object by the name of the property
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/item/
---
## BuiltInDocumentPropertyCollection indexer

Returns a [`DocumentProperty`](../../documentproperty/) object by the name of the property.

```csharp
public override DocumentProperty this[string name] { get; }
```

| Parameter | Description |
| --- | --- |
| name | The case-insensitive name of the property to retrieve. |

### Remarks

The string names of the properties correspond to the names of the typed properties available from [`BuiltInDocumentPropertyCollection`](../).

If you request a property that is not present in the document, but the name of the property is recognized as a valid built-in name, a new [`DocumentProperty`](../../documentproperty/) is created, added to the collection and returned. The newly created property is assigned a default value (empty string, zero, false or DateTime.MinValue depending on the type of the built-in property).

If you request a property that is not present in the document and the name is not recognized as a built-in name, a null is returned.

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;15.0300&amp;quot;, workbook.Worksheets.BuiltInDocumentProperties[&amp;quot;Version&amp;quot;].ToString());
[Test]
        public void Property_String_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET-43355.xlsx&quot;);
            Assert.AreEqual(&quot;15.0300&quot;, workbook.Worksheets.BuiltInDocumentProperties[&quot;Version&quot;].ToString());
            workbook.Save(Constants.destPath + &quot;CELLSNET43355.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET43355.xls&quot;);
            Assert.AreEqual(&quot;15.0300&quot;, workbook.Worksheets.BuiltInDocumentProperties[&quot;Version&quot;].ToString());
        }
```

### See Also

* class [DocumentProperty](../../documentproperty/)
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


