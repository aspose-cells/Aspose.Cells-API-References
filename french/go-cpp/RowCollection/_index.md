---
title: "Classe RowCollection"
linktitle: "RowCollection"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe RowCollection. Encapsule l'objet qui représente rowcollection en Go."
type: docs
weight: 200
url: /fr/go-cpp/rowcollection/
---

## RowCollection class

Collecte les objets <see cref=\"Row\"/> qui représentent les lignes individuelles dans une feuille de calcul.

```go

type RowCollection struct  {
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
| [GetCount](./getcount/) | Obtient le nombre de lignes dans cette collection. |
| [GetEnumerator](./getenumerator/) | Obtient un énumérateur qui parcourt les lignes de cette collection |
| [GetEnumerator_Bool_Bool](./getenumerator_bool_bool/) | Obtient un énumérateur qui parcourt les lignes de cette collection |
| [GetRowByIndex](./getrowbyindex/) | Obtient l'objet Row par la position dans la liste. |
| [Get](./get/) | Obtient un objet Row par l'index de ligne donné. L'objet Row de l'index de ligne donné sera instancié s'il n'existe pas déjà. |
| [Clear](./clear/) | Efface toutes les lignes et cellules. |
| [RemoveAt](./removeat/) | Supprime l'élément de ligne à l'index (position) spécifié dans cette collection. |
