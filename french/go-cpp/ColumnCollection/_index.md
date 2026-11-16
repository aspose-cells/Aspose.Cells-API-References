---
title: "Classe ColumnCollection"
linktitle: "ColumnCollection"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe ColumnCollection. Encapsule l'objet qui représente columncollection en Go."
type: docs
weight: 200
url: /fr/go-cpp/columncollection/
---

## ColumnCollection class

Collection des objets <see cref=\"Column\"/> qui représentent les colonnes individuelles (paramètres) d'une feuille de calcul. L'objet Column ne représente que les paramètres tels que la largeur de colonne, les styles, etc. pour la colonne entière, et n'a rien à voir avec la présence ou non de cellules non vides (données) dans la colonne correspondante. Et le \"Count\" de cette collection ne représente que le nombre d'objets Column qui ont été instanciés dans cette collection, et n'a rien à voir avec la présence ou non de cellules non vides (données) dans la feuille de calcul.

```go

type ColumnCollection struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetColumnByIndex](./getcolumnbyindex/) | Obtient l'objet Column par la position dans la liste. |
| [Get](./get/) | Obtient un objet Column par l'index de colonne. L'objet Column de l'index de colonne donné sera instancié s'il n'existe pas auparavant. |
| [GetCount](./getcount/) | Obtient le nombre d'éléments contenus dans l'instance. |
