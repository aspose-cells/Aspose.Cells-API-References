---
title: "GridSheetRender.ToImage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GridSheetRender. Rendre une certaine page vers un Graphics"
type: docs
url: /fr/net/aspose.cells.griddesktop.data/gridsheetrender/toimage/
---
## ToImage(int, Graphics, float, float, float, float) {#toimage_2}

Rendre une certaine page vers un Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y, float width, float height)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indiquer quelle page doit être convertie |
| g | Graphiques | L'objet où rendre. |
| x | Single | La coordonnée X (en pixels) du coin supérieur gauche de la page rendue. |
| y | Single | La coordonnée Y (en pixels) du coin supérieur gauche de la page rendue. |
| largeur | Single | La largeur maximale (en pixels) pouvant être occupée par la page rendue. |
| hauteur | Single | La hauteur maximale (en pixels) pouvant être occupée par la page rendue. |

### Voir aussi

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, Graphics, float, float) {#toimage_1}

Rendre une certaine page vers un Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indiquer quelle page doit être convertie |
| g | Graphiques | L'objet où rendre. |
| x | Single | La coordonnée X (en pixels) du coin supérieur gauche de la page rendue. |
| y | Single | La coordonnée Y (en pixels) du coin supérieur gauche de la page rendue. |

### Voir aussi

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, string) {#toimage_4}

Rendre une page donnée vers un fichier.

```csharp
public void ToImage(int pageIndex, string fileName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indiquer quelle page doit être convertie |
| fileName | String | nom de fichier de l'image de sortie |

### Exemples

Le code suivant génère la première page de la première feuille en image png.

```csharp
//chargez le fichier source avec les images.
Workbook wb = new Workbook("Book1.xlsx");

ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();

//définir le type d'image de sortie.
imgOpt.ImageType = ImageType.Png;

//rendre la première feuille.
SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);

//générer la première page de la feuille en image.
sr.ToImage(0, "output.png");
```

### Voir aussi

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, Stream) {#toimage_3}

Rendre une page donnée vers un flux.

```csharp
public void ToImage(int pageIndex, Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indiquer quelle page doit être convertie |
| stream | Stream | le flux de l'image de sortie |

### Voir aussi

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int) {#toimage}

Rendre une page donnée vers un objet Bitmap.

```csharp
public Bitmap ToImage(int pageIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indiquer quelle page doit être convertie |

### Valeur de retour

l'objet bitmap de la page

### Voir aussi

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


