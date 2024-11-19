---
title: NameCollection Class 
linktitle: NameCollection
second_title: Aspose.Cells for Go API Reference
description: 'NameCollection class. Encapsulates the object that represents namecollection in Go.'
type: docs
weight: 200
url: /go/aspose.cells/namecollection/
---

## NameCollection class

Represents a collection of all the <see cref="Name"/> objects in the spreadsheet.

```go

type NameCollection struct 

namecollection, _ := asposecells.NewNameCollection()

```
## Constructors

| Method | Description |
| --- | --- |
|[NewNameCollection](./newnamecollection/) | Constructs from an implementation object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[Add](./add/) | Defines a new name. | 
|[Get](./get/) | Gets the <see cref="Name"/> element at the specified index. | 
|[Get](./get/) | Gets the <see cref="Name"/> element with the specified name. | 
|[Remove](./remove/) | Remove the name. | 
|[RemoveAt](./removeat/) | Remove the name at the specific index. | 
|[Clear](./clear/) | Remove all defined names which are not referenced by the formulas and data source.If the defined name is referred, we only set Name.ReferTo as null and hide them. | 
|[RemoveDuplicateNames](./removeduplicatenames/) | Remove the duplicate defined names | 
|[Sort](./sort/) | Sorts defined names. | 
|[GetCount](./getcount/) |  | 
