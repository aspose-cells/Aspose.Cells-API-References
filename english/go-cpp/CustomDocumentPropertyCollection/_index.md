---
title: CustomDocumentPropertyCollection Class 
linktitle: CustomDocumentPropertyCollection
second_title: Aspose.Cells for Go API Reference
description: 'CustomDocumentPropertyCollection class. Encapsulates the object that represents customdocumentpropertycollection in Go.'
type: docs
weight: 200
url: /go-cpp/customdocumentpropertycollection/
---

## CustomDocumentPropertyCollection class

A collection of custom document properties.

```go

type CustomDocumentPropertyCollection struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
|[NewCustomDocumentPropertyCollection](./newcustomdocumentpropertycollection/) | Constructs from a parent object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[Add_String_String](./add_string_string/) | Creates a new custom document property of the <b>PropertyType.String</b> data type. | 
|[Add_String_Int](./add_string_int/) | Creates a new custom document property of the <b>PropertyType.Number</b> data type. | 
|[Add_String_Date](./add_string_date/) | Creates a new custom document property of the <b>PropertyType.DateTime</b> data type. | 
|[Add_String_Bool](./add_string_bool/) | Creates a new custom document property of the <b>PropertyType.Boolean</b> data type. | 
|[Add_String_Double](./add_string_double/) | Creates a new custom document property of the <b>PropertyType.Float</b> data type. | 
|[AddLinkToContent](./addlinktocontent/) | Creates a new custom document property which links to content. | 
|[UpdateLinkedPropertyValue](./updatelinkedpropertyvalue/) | Update custom document property value which links to content. | 
|[UpdateLinkedRange](./updatelinkedrange/) | Update custom document property value to linked range. | 
|[Get_Int](./get_int/) | Returns a <see cref="DocumentProperty"/> object by index. | 
|[Contains](./contains/) | Returns true if a property with the specified name exists in the collection. | 
|[IndexOf](./indexof/) | Gets the index of a property by name. | 
|[Remove](./remove/) | Removes a property with the specified name from the collection. | 
|[RemoveAt](./removeat/) | Removes a property at the specified index. | 
|[Get_String](./get_string/) | Returns a <see cref="DocumentProperty"/> object by the name of the property. | 
|[GetCount](./getcount/) |  | 
