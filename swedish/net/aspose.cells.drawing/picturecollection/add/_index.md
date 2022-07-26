---
title: Add
second_title: Aspose.Cells för .NET API-referens
description: Lägger till en bild i samlingen.
type: docs
weight: 20
url: /sv/net/aspose.cells.drawing/picturecollection/add/
---
## Add(int, int, int, int, Stream) {#add}

Lägger till en bild i samlingen.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, 
    Stream stream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| upperLeftRow | Int32 | Övre vänstra radens index. |
| upperLeftColumn | Int32 | Övre vänstra kolumnindex. |
| lowerRightRow | Int32 | Nedre högra radindex |
| lowerRightColumn | Int32 | Nedre högra kolumnindex |
| stream | Stream | Strömobjekt som innehåller bilddata. |

### Returvärde

[`Picture`](../../picture) objektindex.

### Exempel

```csharp

[C#]
//lägg till en bild
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, 5, 5, fs);
}
```

### Se även

* class [PictureCollection](../../picturecollection)
* namnutrymme [Aspose.Cells.Drawing](../../picturecollection)
* hopsättning [Aspose.Cells](../../../)

---

## Add(int, int, int, int, string) {#add_1}

Lägger till en bild i samlingen.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, 
    string fileName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| upperLeftRow | Int32 | Övre vänstra radens index. |
| upperLeftColumn | Int32 | Övre vänstra kolumnindex. |
| lowerRightRow | Int32 | Nedre högra radindex |
| lowerRightColumn | Int32 | Nedre högra kolumnindex |
| fileName | String | Bildfilnamn. |

### Returvärde

[`Picture`](../../picture) objektindex.

### Exempel

```csharp

[C#]
//lägg till en bild
pictures.Add(1, 1, 5, 5, "image.jpg");
```

### Se även

* class [PictureCollection](../../picturecollection)
* namnutrymme [Aspose.Cells.Drawing](../../picturecollection)
* hopsättning [Aspose.Cells](../../../)

---

## Add(int, int, Stream) {#add_2}

Lägger till en bild i samlingen.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, Stream stream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| upperLeftRow | Int32 | Övre vänstra radens index. |
| upperLeftColumn | Int32 | Övre vänstra kolumnindex. |
| stream | Stream | Strömobjekt som innehåller bilddata. |

### Returvärde

[`Picture`](../../picture) objektindex.

### Exempel

```csharp

[C#]
//lägg till en bild
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, fs);
}
```

### Se även

* class [PictureCollection](../../picturecollection)
* namnutrymme [Aspose.Cells.Drawing](../../picturecollection)
* hopsättning [Aspose.Cells](../../../)

---

## Add(int, int, string) {#add_4}

Lägger till en bild i samlingen.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, string fileName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| upperLeftRow | Int32 | Övre vänstra radens index. |
| upperLeftColumn | Int32 | Övre vänstra kolumnindex. |
| fileName | String | Bildfilnamn. |

### Returvärde

[`Picture`](../../picture) objektindex.

### Exempel

```csharp

[C#]
//lägg till en bild
pictures.Add(1, 1, "image.jpg");
```

### Se även

* class [PictureCollection](../../picturecollection)
* namnutrymme [Aspose.Cells.Drawing](../../picturecollection)
* hopsättning [Aspose.Cells](../../../)

---

## Add(int, int, Stream, int, int) {#add_3}

Lägger till en bild i samlingen.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, Stream stream, int widthScale, 
    int heightScale)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| upperLeftRow | Int32 | Övre vänstra radens index. |
| upperLeftColumn | Int32 | Övre vänstra kolumnindex. |
| stream | Stream | Strömobjekt som innehåller bilddata. |
| widthScale | Int32 | Skala på bildens bredd, en procentandel. |
| heightScale | Int32 | Skala för bildhöjd, en procentandel. |

### Returvärde

[`Picture`](../../picture) objektindex.

### Exempel

```csharp

[C#]
//lägg till en bild
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, fs, 50, 50);
}
```

### Se även

* class [PictureCollection](../../picturecollection)
* namnutrymme [Aspose.Cells.Drawing](../../picturecollection)
* hopsättning [Aspose.Cells](../../../)

---

## Add(int, int, string, int, int) {#add_5}

Lägger till en bild i samlingen.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, string fileName, int widthScale, 
    int heightScale)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| upperLeftRow | Int32 | Övre vänstra radens index. |
| upperLeftColumn | Int32 | Övre vänstra kolumnindex. |
| fileName | String | Bildfilnamn. |
| widthScale | Int32 | Skala på bildens bredd, en procentandel. |
| heightScale | Int32 | Skala för bildhöjd, en procentandel. |

### Returvärde

[`Picture`](../../picture) objektindex.

### Exempel

```csharp

[C#]
//lägg till en bild
pictures.Add(1, 1, "image.jpg", 50, 50);
```

### Se även

* class [PictureCollection](../../picturecollection)
* namnutrymme [Aspose.Cells.Drawing](../../picturecollection)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
