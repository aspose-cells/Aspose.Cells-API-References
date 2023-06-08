---
title: PictureCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: PictureCollection property. Gets the Picture element at the specified index
type: docs
url: /net/aspose.cells.drawing/picturecollection/item/
---
## PictureCollection indexer

Gets the [`Picture`](../../picture/) element at the specified index.

```csharp
public Picture this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp

[C#]
//get picture collection
//PictureCollection pictures = workbook.Worksheets[0].Pictures;
//add a picture
int index = pictures.Add(1, 1, "image.png");
//get the picture
Picture pic = pictures[index];
```

### See Also

* class [Picture](../../picture/)
* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


