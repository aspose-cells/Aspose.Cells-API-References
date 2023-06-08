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

### See Also

* class [DocumentProperty](../../documentproperty/)
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


