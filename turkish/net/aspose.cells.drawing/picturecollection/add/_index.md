---
title: Add
second_title: Aspose.Cells for .NET API Referansı
description: Koleksiyona bir resim ekler.
type: docs
weight: 20
url: /tr/net/aspose.cells.drawing/picturecollection/add/
---
## Add(int, int, int, int, Stream) {#add}

Koleksiyona bir resim ekler.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, 
    Stream stream)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| upperLeftRow | Int32 | Sol üst satır dizini. |
| upperLeftColumn | Int32 | Sol üst sütun dizini. |
| lowerRightRow | Int32 | Sağ alt satır dizini |
| lowerRightColumn | Int32 | Sağ alt sütun dizini |
| stream | Stream | Görüntü verilerini içeren akış nesnesi. |

### Geri dönüş değeri

[`Picture`](../../picture) nesne indeksi.

### Örnekler

```csharp

[C#]
//resim ekle
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, 5, 5, fs);
}
```

### Ayrıca bakınız

* class [PictureCollection](../../picturecollection)
* ad alanı [Aspose.Cells.Drawing](../../picturecollection)
* toplantı [Aspose.Cells](../../../)

---

## Add(int, int, int, int, string) {#add_1}

Koleksiyona bir resim ekler.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, 
    string fileName)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| upperLeftRow | Int32 | Sol üst satır dizini. |
| upperLeftColumn | Int32 | Sol üst sütun dizini. |
| lowerRightRow | Int32 | Sağ alt satır dizini |
| lowerRightColumn | Int32 | Sağ alt sütun dizini |
| fileName | String | Resim dosya adı. |

### Geri dönüş değeri

[`Picture`](../../picture) nesne indeksi.

### Örnekler

```csharp

[C#]
//resim ekle
pictures.Add(1, 1, 5, 5, "image.jpg");
```

### Ayrıca bakınız

* class [PictureCollection](../../picturecollection)
* ad alanı [Aspose.Cells.Drawing](../../picturecollection)
* toplantı [Aspose.Cells](../../../)

---

## Add(int, int, Stream) {#add_2}

Koleksiyona bir resim ekler.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, Stream stream)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| upperLeftRow | Int32 | Sol üst satır dizini. |
| upperLeftColumn | Int32 | Sol üst sütun dizini. |
| stream | Stream | Görüntü verilerini içeren akış nesnesi. |

### Geri dönüş değeri

[`Picture`](../../picture) nesne indeksi.

### Örnekler

```csharp

[C#]
//resim ekle
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, fs);
}
```

### Ayrıca bakınız

* class [PictureCollection](../../picturecollection)
* ad alanı [Aspose.Cells.Drawing](../../picturecollection)
* toplantı [Aspose.Cells](../../../)

---

## Add(int, int, string) {#add_4}

Koleksiyona bir resim ekler.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, string fileName)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| upperLeftRow | Int32 | Sol üst satır dizini. |
| upperLeftColumn | Int32 | Sol üst sütun dizini. |
| fileName | String | Resim dosya adı. |

### Geri dönüş değeri

[`Picture`](../../picture) nesne indeksi.

### Örnekler

```csharp

[C#]
//resim ekle
pictures.Add(1, 1, "image.jpg");
```

### Ayrıca bakınız

* class [PictureCollection](../../picturecollection)
* ad alanı [Aspose.Cells.Drawing](../../picturecollection)
* toplantı [Aspose.Cells](../../../)

---

## Add(int, int, Stream, int, int) {#add_3}

Koleksiyona bir resim ekler.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, Stream stream, int widthScale, 
    int heightScale)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| upperLeftRow | Int32 | Sol üst satır dizini. |
| upperLeftColumn | Int32 | Sol üst sütun dizini. |
| stream | Stream | Görüntü verilerini içeren akış nesnesi. |
| widthScale | Int32 | Görüntü genişliği ölçeği, bir yüzde. |
| heightScale | Int32 | Görüntü yüksekliği ölçeği, yüzde. |

### Geri dönüş değeri

[`Picture`](../../picture) nesne indeksi.

### Örnekler

```csharp

[C#]
//resim ekle
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, fs, 50, 50);
}
```

### Ayrıca bakınız

* class [PictureCollection](../../picturecollection)
* ad alanı [Aspose.Cells.Drawing](../../picturecollection)
* toplantı [Aspose.Cells](../../../)

---

## Add(int, int, string, int, int) {#add_5}

Koleksiyona bir resim ekler.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, string fileName, int widthScale, 
    int heightScale)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| upperLeftRow | Int32 | Sol üst satır dizini. |
| upperLeftColumn | Int32 | Sol üst sütun dizini. |
| fileName | String | Resim dosya adı. |
| widthScale | Int32 | Görüntü genişliği ölçeği, bir yüzde. |
| heightScale | Int32 | Görüntü yüksekliği ölçeği, yüzde. |

### Geri dönüş değeri

[`Picture`](../../picture) nesne indeksi.

### Örnekler

```csharp

[C#]
//resim ekle
pictures.Add(1, 1, "image.jpg", 50, 50);
```

### Ayrıca bakınız

* class [PictureCollection](../../picturecollection)
* ad alanı [Aspose.Cells.Drawing](../../picturecollection)
* toplantı [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
