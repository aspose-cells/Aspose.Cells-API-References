---
title: Add
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 20
url: /net/aspose.cells.drawing/picturecollection/add/
---
## PictureCollection.Add method (1 of 6)

Adds a picture to the collection.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, 
    Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| upperLeftColumn | Int32 | Upper left column index. |
| lowerRightRow | Int32 | Lower right row index |
| lowerRightColumn | Int32 | Lower right column index |
| stream | Stream | Stream object which contains the image data. |

### Return Value

[`Picture`](../../picture) object index.

### Examples

```csharp

[C#]
//add a picture
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, 5, 5, fs);
}
```

### See Also

* class [PictureCollection](../../picturecollection)
* namespace [Aspose.Cells.Drawing](../../picturecollection)
* assembly [Aspose.Cells](../../../)

---

## PictureCollection.Add method (2 of 6)

Adds a picture to the collection.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, 
    string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| upperLeftColumn | Int32 | Upper left column index. |
| lowerRightRow | Int32 | Lower right row index |
| lowerRightColumn | Int32 | Lower right column index |
| fileName | String | Image filename. |

### Return Value

[`Picture`](../../picture) object index.

### Examples

```csharp

[C#]
//add a picture
pictures.Add(1, 1, 5, 5, "image.jpg");
```

### See Also

* class [PictureCollection](../../picturecollection)
* namespace [Aspose.Cells.Drawing](../../picturecollection)
* assembly [Aspose.Cells](../../../)

---

## PictureCollection.Add method (3 of 6)

Adds a picture to the collection.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| upperLeftColumn | Int32 | Upper left column index. |
| stream | Stream | Stream object which contains the image data. |

### Return Value

[`Picture`](../../picture) object index.

### Examples

```csharp

[C#]
//add a picture
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, fs);
}
```

### See Also

* class [PictureCollection](../../picturecollection)
* namespace [Aspose.Cells.Drawing](../../picturecollection)
* assembly [Aspose.Cells](../../../)

---

## PictureCollection.Add method (4 of 6)

Adds a picture to the collection.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| upperLeftColumn | Int32 | Upper left column index. |
| fileName | String | Image filename. |

### Return Value

[`Picture`](../../picture) object index.

### Examples

```csharp

[C#]
//add a picture
pictures.Add(1, 1, "image.jpg");
```

### See Also

* class [PictureCollection](../../picturecollection)
* namespace [Aspose.Cells.Drawing](../../picturecollection)
* assembly [Aspose.Cells](../../../)

---

## PictureCollection.Add method (5 of 6)

Adds a picture to the collection.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, Stream stream, int widthScale, 
    int heightScale)
```

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| upperLeftColumn | Int32 | Upper left column index. |
| stream | Stream | Stream object which contains the image data. |
| widthScale | Int32 | Scale of image width, a percentage. |
| heightScale | Int32 | Scale of image height, a percentage. |

### Return Value

[`Picture`](../../picture) object index.

### Examples

```csharp

[C#]
//add a picture
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, fs, 50, 50);
}
```

### See Also

* class [PictureCollection](../../picturecollection)
* namespace [Aspose.Cells.Drawing](../../picturecollection)
* assembly [Aspose.Cells](../../../)

---

## PictureCollection.Add method (6 of 6)

Adds a picture to the collection.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, string fileName, int widthScale, 
    int heightScale)
```

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| upperLeftColumn | Int32 | Upper left column index. |
| fileName | String | Image filename. |
| widthScale | Int32 | Scale of image width, a percentage. |
| heightScale | Int32 | Scale of image height, a percentage. |

### Return Value

[`Picture`](../../picture) object index.

### Examples

```csharp

[C#]
//add a picture
pictures.Add(1, 1, "image.jpg", 50, 50);
```

### See Also

* class [PictureCollection](../../picturecollection)
* namespace [Aspose.Cells.Drawing](../../picturecollection)
* assembly [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
