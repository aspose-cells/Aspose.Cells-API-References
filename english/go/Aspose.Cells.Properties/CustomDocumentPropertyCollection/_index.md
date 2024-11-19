---
title: CustomDocumentPropertyCollection Class 
linktitle: CustomDocumentPropertyCollection
second_title: Aspose.Cells for Go API Reference
description: 'CustomDocumentPropertyCollection class. Encapsulates the object that represents customdocumentpropertycollection in Go.'
type: docs
weight: 200
url: /go/aspose.cells.properties/customdocumentpropertycollection/
---

## CustomDocumentPropertyCollection class

A collection of custom document properties.

```go

type CustomDocumentPropertyCollection struct 

customdocumentpropertycollection, _ := asposecells.NewCustomDocumentPropertyCollection()

```
## Constructors

| Method | Description |
| --- | --- |
|[NewCustomDocumentPropertyCollection_CustomDocumentPropertyCollection](./newcustomdocumentpropertycollection_customdocumentpropertycollection/) | Constructs from an implementation object. | 
|[NewCustomDocumentPropertyCollection_DocumentPropertyCollection](./newcustomdocumentpropertycollection_documentpropertycollection/) | Constructs from a parent object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[Add](./add/) | Creates a new custom document property of the <b>PropertyType.String</b> data type. | 
|[Add](./add/) | Creates a new custom document property of the <b>PropertyType.Number</b> data type. | 
|[Add](./add/) | Creates a new custom document property of the <b>PropertyType.DateTime</b> data type. | 
|[Add](./add/) | Creates a new custom document property of the <b>PropertyType.Boolean</b> data type. | 
|[Add](./add/) | Creates a new custom document property of the <b>PropertyType.Float</b> data type. | 
|[AddLinkToContent](./addlinktocontent/) | Creates a new custom document property which links to content. | 
|[UpdateLinkedPropertyValue](./updatelinkedpropertyvalue/) | Update custom document property value which links to content. | 
|[UpdateLinkedRange](./updatelinkedrange/) | Update custom document property value to linked range. | 
|[Get](./get/) | Returns a <see cref="DocumentProperty"/> object by index. | 
|[Contains](./contains/) | Returns true if a property with the specified name exists in the collection. | 
|[IndexOf](./indexof/) | Gets the index of a property by name. | 
|[Remove](./remove/) | Removes a property with the specified name from the collection. | 
|[RemoveAt](./removeat/) | Removes a property at the specified index. | 
|[Get](./get/) | Returns a <see cref="DocumentProperty"/> object by the name of the property. | 
|[GetCount](./getcount/) |  | 
