---
title: ToImage
second_title: Référence de l'API Aspose.Cells pour .NET
description: Rendre certaines pages en Graphics
type: docs
weight: 60
url: /fr/net/aspose.cells.rendering/sheetrender/toimage/
---
## ToImage(int, Graphics, float, float, float, float) {#toimage_2}

Rendre certaines pages en Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y, float width, float height)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pageIndex | Int32 | indiquer quelle page doit être convertie |
| g | Graphics | L'objet vers lequel effectuer le rendu. |
| x | Single | Coordonnée X (en pixels) du coin supérieur gauche de la page rendue. |
| y | Single | La coordonnée Y (en pixels) du coin supérieur gauche de la page rendue. |
| width | Single | La largeur maximale (en pixels) pouvant être occupée par la page rendue. |
| height | Single | La hauteur maximale (en pixels) pouvant être occupée par la page rendue. |

### Voir également

* class [SheetRender](../../sheetrender)
* espace de noms [Aspose.Cells.Rendering](../../sheetrender)
* Assemblée [Aspose.Cells](../../../)

---

## ToImage(int, Graphics, float, float) {#toimage_1}

Rendre certaines pages en Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pageIndex | Int32 | indiquer quelle page doit être convertie |
| g | Graphics | L'objet vers lequel effectuer le rendu. |
| x | Single | Coordonnée X (en pixels) du coin supérieur gauche de la page rendue. |
| y | Single | La coordonnée Y (en pixels) du coin supérieur gauche de la page rendue. |

### Voir également

* class [SheetRender](../../sheetrender)
* espace de noms [Aspose.Cells.Rendering](../../sheetrender)
* Assemblée [Aspose.Cells](../../../)

---

## ToImage(int, string) {#toimage_4}

Afficher certaines pages dans un fichier.

```csharp
public void ToImage(int pageIndex, string fileName)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pageIndex | Int32 | indiquer quelle page doit être convertie |
| fileName | String | nom de fichier de l'image de sortie |

### Exemples

Le code suivant génère la première page de la première feuille en image png.

```csharp
// charge le fichier source avec des images.
Workbook wb = new Workbook("Book1.xlsx");

ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();

// définit le type d'image de sortie.
imgOpt.ImageType = ImageType.Png;

// rend la première feuille.
SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);

// affiche la première page de la feuille sur l'image.
sr.ToImage(0, "output.png");
```

### Voir également

* class [SheetRender](../../sheetrender)
* espace de noms [Aspose.Cells.Rendering](../../sheetrender)
* Assemblée [Aspose.Cells](../../../)

---

## ToImage(int, Stream) {#toimage_3}

Afficher une certaine page dans un flux.

```csharp
public void ToImage(int pageIndex, Stream stream)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pageIndex | Int32 | indiquer quelle page doit être convertie |
| stream | Stream | le flux de l'image de sortie |

### Voir également

* class [SheetRender](../../sheetrender)
* espace de noms [Aspose.Cells.Rendering](../../sheetrender)
* Assemblée [Aspose.Cells](../../../)

---

## ToImage(int) {#toimage}

Afficher une certaine page dans un objet Bitmap.

```csharp
public Bitmap ToImage(int pageIndex)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pageIndex | Int32 | indiquer quelle page doit être convertie |

### Return_Value

l'objet bitmap de la page

### Voir également

* class [SheetRender](../../sheetrender)
* espace de noms [Aspose.Cells.Rendering](../../sheetrender)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
