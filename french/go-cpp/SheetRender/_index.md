---
title: "Classe SheetRender"
linktitle: "SheetRender"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe SheetRender. Encapsule l'objet qui représente sheetrender en Go."
type: docs
weight: 200
url: /fr/go-cpp/sheetrender/
---

## SheetRender class

Représente un rendu de feuille de calcul qui peut rendre la feuille de calcul en diverses images telles que (BMP, PNG, JPEG, TIFF...). Le constructeur de cette classe doit être utilisé après la modification de la configuration de la page et du style des cellules.

```go

type SheetRender struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewSheetRender](./newsheetrender/) | la construction de SheetRender, nécessite une feuille de calcul et ImageOrPrintOptions comme paramètres |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetPageCount](./getpagecount/) | Obtient le nombre total de pages de la feuille de calcul actuelle. |
| [GetPageScale](./getpagescale/) | Obtient l'échelle de page calculée de la feuille. Retourne l'échelle définie si PageSetup.Zoom est défini. Sinon, retourne l'échelle calculée selon PageSetup.FitToPagesWide et PageSetup.FitToPagesTall. |
| [GetPageSizeInch](./getpagesizeinch/) | Obtenez la taille de la page en pouces de l'image de sortie. |
| [ToImage_Int_String](./toimage_int_string/) | Rendre une certaine page vers un fichier. |
| [ToImage_Int](./toimage_int/) | Rendre une certaine page vers le flux. |
| [ToTiff](./totiff/) | Rendu de la feuille de calcul entière en image Tiff vers un flux. |
| [ToTiff_String](./totiff_string/) | Rendu de la feuille de calcul entière en image Tiff vers un fichier. |
| [Dispose](./dispose/) | Libère les ressources créées et utilisées pour le rendu. |
