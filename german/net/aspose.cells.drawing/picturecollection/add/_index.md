---
title: Add
second_title: Aspose.Cells für .NET-API-Referenz
description: Fügt der Sammlung ein Bild hinzu.
type: docs
weight: 20
url: /de/net/aspose.cells.drawing/picturecollection/add/
---
## Add(int, int, int, int, Stream) {#add}

Fügt der Sammlung ein Bild hinzu.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, 
    Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| upperLeftRow | Int32 | Zeilenindex oben links. |
| upperLeftColumn | Int32 | Spaltenindex oben links. |
| lowerRightRow | Int32 | Zeilenindex unten rechts |
| lowerRightColumn | Int32 | Spaltenindex unten rechts |
| stream | Stream | Stream-Objekt, das die Bilddaten enthält. |

### Rückgabewert

[`Picture`](../../picture) Objektindex.

### Beispiele

```csharp

[C#]
//Bild hinzufügen
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, 5, 5, fs);
}
```

### Siehe auch

* class [PictureCollection](../../picturecollection)
* namensraum [Aspose.Cells.Drawing](../../picturecollection)
* Montage [Aspose.Cells](../../../)

---

## Add(int, int, int, int, string) {#add_1}

Fügt der Sammlung ein Bild hinzu.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, 
    string fileName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| upperLeftRow | Int32 | Zeilenindex oben links. |
| upperLeftColumn | Int32 | Spaltenindex oben links. |
| lowerRightRow | Int32 | Zeilenindex unten rechts |
| lowerRightColumn | Int32 | Spaltenindex unten rechts |
| fileName | String | Bilddateiname. |

### Rückgabewert

[`Picture`](../../picture) Objektindex.

### Beispiele

```csharp

[C#]
//Bild hinzufügen
pictures.Add(1, 1, 5, 5, "image.jpg");
```

### Siehe auch

* class [PictureCollection](../../picturecollection)
* namensraum [Aspose.Cells.Drawing](../../picturecollection)
* Montage [Aspose.Cells](../../../)

---

## Add(int, int, Stream) {#add_2}

Fügt der Sammlung ein Bild hinzu.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| upperLeftRow | Int32 | Zeilenindex oben links. |
| upperLeftColumn | Int32 | Spaltenindex oben links. |
| stream | Stream | Stream-Objekt, das die Bilddaten enthält. |

### Rückgabewert

[`Picture`](../../picture) Objektindex.

### Beispiele

```csharp

[C#]
//Bild hinzufügen
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, fs);
}
```

### Siehe auch

* class [PictureCollection](../../picturecollection)
* namensraum [Aspose.Cells.Drawing](../../picturecollection)
* Montage [Aspose.Cells](../../../)

---

## Add(int, int, string) {#add_4}

Fügt der Sammlung ein Bild hinzu.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, string fileName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| upperLeftRow | Int32 | Zeilenindex oben links. |
| upperLeftColumn | Int32 | Spaltenindex oben links. |
| fileName | String | Bilddateiname. |

### Rückgabewert

[`Picture`](../../picture) Objektindex.

### Beispiele

```csharp

[C#]
//Bild hinzufügen
pictures.Add(1, 1, "image.jpg");
```

### Siehe auch

* class [PictureCollection](../../picturecollection)
* namensraum [Aspose.Cells.Drawing](../../picturecollection)
* Montage [Aspose.Cells](../../../)

---

## Add(int, int, Stream, int, int) {#add_3}

Fügt der Sammlung ein Bild hinzu.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, Stream stream, int widthScale, 
    int heightScale)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| upperLeftRow | Int32 | Zeilenindex oben links. |
| upperLeftColumn | Int32 | Spaltenindex oben links. |
| stream | Stream | Stream-Objekt, das die Bilddaten enthält. |
| widthScale | Int32 | Maßstab der Bildbreite, ein Prozentsatz. |
| heightScale | Int32 | Maßstab der Bildhöhe, ein Prozentsatz. |

### Rückgabewert

[`Picture`](../../picture) Objektindex.

### Beispiele

```csharp

[C#]
//Bild hinzufügen
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, fs, 50, 50);
}
```

### Siehe auch

* class [PictureCollection](../../picturecollection)
* namensraum [Aspose.Cells.Drawing](../../picturecollection)
* Montage [Aspose.Cells](../../../)

---

## Add(int, int, string, int, int) {#add_5}

Fügt der Sammlung ein Bild hinzu.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, string fileName, int widthScale, 
    int heightScale)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| upperLeftRow | Int32 | Zeilenindex oben links. |
| upperLeftColumn | Int32 | Spaltenindex oben links. |
| fileName | String | Bilddateiname. |
| widthScale | Int32 | Maßstab der Bildbreite, ein Prozentsatz. |
| heightScale | Int32 | Maßstab der Bildhöhe, ein Prozentsatz. |

### Rückgabewert

[`Picture`](../../picture) Objektindex.

### Beispiele

```csharp

[C#]
//Bild hinzufügen
pictures.Add(1, 1, "image.jpg", 50, 50);
```

### Siehe auch

* class [PictureCollection](../../picturecollection)
* namensraum [Aspose.Cells.Drawing](../../picturecollection)
* Montage [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
