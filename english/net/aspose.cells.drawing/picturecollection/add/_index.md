---
title: PictureCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: PictureCollection method. Adds a picture to the collection
type: docs
url: /net/aspose.cells.drawing/picturecollection/add/
---
## Add(int, int, int, int, Stream) {#add}

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

[`Picture`](../../picture/) object index.

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

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, int, int, string) {#add_1}

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

[`Picture`](../../picture/) object index.

### Examples

```csharp

[C#]
//add a picture
pictures.Add(1, 1, 5, 5, "image.jpg");
```

### See Also

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, Stream) {#add_2}

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

[`Picture`](../../picture/) object index.

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

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, string) {#add_4}

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

[`Picture`](../../picture/) object index.

### Examples

```csharp

[C#]
//add a picture
pictures.Add(1, 1, "image.jpg");
```

### See Also

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, Stream, int, int) {#add_3}

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

[`Picture`](../../picture/) object index.

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

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, string, int, int) {#add_5}

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

[`Picture`](../../picture/) object index.

### Examples

```csharp

[C#]
//add a picture
pictures.Add(1, 1, "image.jpg", 50, 50);
```

### See Also

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


