---
title: "DrawObject Classe"
linktitle: "DrawObject"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "DrawObject classe. Encapsule l'objet qui représente drawobject en Go."
type: docs
weight: 200
url: /fr/go-cpp/drawobject/
---

## DrawObject class

DrawObject sera initialisé et renvoyé lors du rendu.

```go

type DrawObject struct  {
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
| [GetCell](./getcell/) | Indique l'objet Cell lors du rendu. Toutes les propriétés de cell peuvent être accessibles. |
| [GetShape](./getshape/) | Indique l'objet Shape lors du rendu. Toutes les propriétés de shape peuvent être accessibles. |
| [GetImageBytes](./getimagebytes/) | Indique les octets d'image du Chart rendu, Shape lors du rendu. |
| [GetType](./gettype/) | Indique le type de DrawObject. |
| [GetCurrentPage](./getcurrentpage/) | Indique l'index de page de DrawObject. L'index de page commence à zéro. Une Sheet contient plusieurs pages lors du rendu. |
| [GetTotalPages](./gettotalpages/) | Indique le nombre total de pages dans le rendu actuel. |
| [GetSheetIndex](./getsheetindex/) | Indique l'index de la feuille actuelle de DrawObject. |
