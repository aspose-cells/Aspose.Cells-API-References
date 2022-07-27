---
title: Add
second_title: Référence de l'API Aspose.Cells pour .NET
description: Ajoute une image à la collection.
type: docs
weight: 20
url: /fr/net/aspose.cells.drawing/picturecollection/add/
---
## Add(int, int, int, int, Stream) {#add}

Ajoute une image à la collection.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, 
    Stream stream)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| upperLeftRow | Int32 | Index de ligne en haut à gauche. |
| upperLeftColumn | Int32 | Index de la colonne en haut à gauche. |
| lowerRightRow | Int32 | Index de ligne en bas à droite |
| lowerRightColumn | Int32 | Index de la colonne en bas à droite |
| stream | Stream | Objet de flux qui contient les données d'image. |

### Return_Value

[`Picture`](../../picture) indice d'objet.

### Exemples

```csharp

[C#]
// ajouter une image
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, 5, 5, fs);
}
```

### Voir également

* class [PictureCollection](../../picturecollection)
* espace de noms [Aspose.Cells.Drawing](../../picturecollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(int, int, int, int, string) {#add_1}

Ajoute une image à la collection.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, 
    string fileName)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| upperLeftRow | Int32 | Index de ligne en haut à gauche. |
| upperLeftColumn | Int32 | Index de la colonne en haut à gauche. |
| lowerRightRow | Int32 | Index de ligne en bas à droite |
| lowerRightColumn | Int32 | Index de la colonne en bas à droite |
| fileName | String | Nom du fichier image. |

### Return_Value

[`Picture`](../../picture) indice d'objet.

### Exemples

```csharp

[C#]
// ajouter une image
pictures.Add(1, 1, 5, 5, "image.jpg");
```

### Voir également

* class [PictureCollection](../../picturecollection)
* espace de noms [Aspose.Cells.Drawing](../../picturecollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(int, int, Stream) {#add_2}

Ajoute une image à la collection.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, Stream stream)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| upperLeftRow | Int32 | Index de ligne en haut à gauche. |
| upperLeftColumn | Int32 | Index de la colonne en haut à gauche. |
| stream | Stream | Objet de flux qui contient les données d'image. |

### Return_Value

[`Picture`](../../picture) indice d'objet.

### Exemples

```csharp

[C#]
// ajouter une image
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, fs);
}
```

### Voir également

* class [PictureCollection](../../picturecollection)
* espace de noms [Aspose.Cells.Drawing](../../picturecollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(int, int, string) {#add_4}

Ajoute une image à la collection.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, string fileName)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| upperLeftRow | Int32 | Index de ligne en haut à gauche. |
| upperLeftColumn | Int32 | Index de la colonne en haut à gauche. |
| fileName | String | Nom du fichier image. |

### Return_Value

[`Picture`](../../picture) indice d'objet.

### Exemples

```csharp

[C#]
// ajouter une image
pictures.Add(1, 1, "image.jpg");
```

### Voir également

* class [PictureCollection](../../picturecollection)
* espace de noms [Aspose.Cells.Drawing](../../picturecollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(int, int, Stream, int, int) {#add_3}

Ajoute une image à la collection.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, Stream stream, int widthScale, 
    int heightScale)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| upperLeftRow | Int32 | Index de ligne en haut à gauche. |
| upperLeftColumn | Int32 | Index de la colonne en haut à gauche. |
| stream | Stream | Objet de flux qui contient les données d'image. |
| widthScale | Int32 | Échelle de la largeur de l'image, un pourcentage. |
| heightScale | Int32 | Échelle de la hauteur de l'image, un pourcentage. |

### Return_Value

[`Picture`](../../picture) indice d'objet.

### Exemples

```csharp

[C#]
// ajouter une image
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, fs, 50, 50);
}
```

### Voir également

* class [PictureCollection](../../picturecollection)
* espace de noms [Aspose.Cells.Drawing](../../picturecollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(int, int, string, int, int) {#add_5}

Ajoute une image à la collection.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, string fileName, int widthScale, 
    int heightScale)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| upperLeftRow | Int32 | Index de ligne en haut à gauche. |
| upperLeftColumn | Int32 | Index de la colonne en haut à gauche. |
| fileName | String | Nom du fichier image. |
| widthScale | Int32 | Échelle de la largeur de l'image, un pourcentage. |
| heightScale | Int32 | Échelle de la hauteur de l'image, un pourcentage. |

### Return_Value

[`Picture`](../../picture) indice d'objet.

### Exemples

```csharp

[C#]
// ajouter une image
pictures.Add(1, 1, "image.jpg", 50, 50);
```

### Voir également

* class [PictureCollection](../../picturecollection)
* espace de noms [Aspose.Cells.Drawing](../../picturecollection)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
