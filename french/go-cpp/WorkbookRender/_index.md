---
title: "WorkbookRender Classe"
linktitle: "WorkbookRender"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "WorkbookRender classe. Encapsule l'objet qui représente workbookrender en Go."
type: docs
weight: 200
url: /fr/go-cpp/workbookrender/
---

## WorkbookRender class

Représente un rendu de classeur. Le constructeur de cette classe doit être utilisé après la modification de la configuration de la page et du style des cellules.

```go

type WorkbookRender struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewWorkbookRender](./newworkbookrender/) | La construction de WorkbookRender |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetPageCount](./getpagecount/) | Obtient le nombre total de pages du classeur. |
| [GetPageSizeInch](./getpagesizeinch/) | Obtenez la taille de la page en pouces de l'image de sortie. |
| [ToImage](./toimage/) | Rendre le classeur complet en image Tiff vers le flux. |
| [ToImage_String](./toimage_string/) | Rendre le classeur complet en image Tiff vers un fichier. |
| [ToImage_Int_String](./toimage_int_string/) | Rendre une certaine page vers un fichier. |
| [ToImage_Int](./toimage_int/) | Rendre une certaine page vers le flux. |
| [Dispose](./dispose/) | Libère les ressources créées et utilisées pour le rendu. |
