---
title: "DataBar Classe"
linktitle: "DataBar"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "DataBar classe. Encapsule l'objet qui représente databar en Go."
type: docs
weight: 200
url: /fr/go-cpp/databar/
---

## DataBar class

Décrit la règle de mise en forme conditionnelle DataBar. Cette règle de mise en forme conditionnelle affiche une barre de données graduée dans la plage de cellules.

```go

type DataBar struct  {
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
| [GetAxisColor](./getaxiscolor/) | Obtient la couleur de l'axe pour les cellules avec mise en forme conditionnelle sous forme de barres de données. |
| [SetAxisColor](./setaxiscolor/) | Obtient la couleur de l'axe pour les cellules avec mise en forme conditionnelle sous forme de barres de données. |
| [GetAxisPosition](./getaxisposition/) | Obtient ou définit la position de l'axe des barres de données spécifiées par une règle de mise en forme conditionnelle. |
| [SetAxisPosition](./setaxisposition/) | Obtient ou définit la position de l'axe des barres de données spécifiées par une règle de mise en forme conditionnelle. |
| [GetBarFillType](./getbarfilltype/) | Obtient ou définit la façon dont une barre de données est remplie de couleur. |
| [SetBarFillType](./setbarfilltype/) | Obtient ou définit la façon dont une barre de données est remplie de couleur. |
| [GetDirection](./getdirection/) | Obtient ou définit la direction d'affichage de la barre de données. |
| [SetDirection](./setdirection/) | Obtient ou définit la direction d'affichage de la barre de données. |
| [GetBarBorder](./getbarborder/) | Obtient un objet qui spécifie la bordure d'une barre de données. |
| [GetNegativeBarFormat](./getnegativebarformat/) | Obtient l'objet NegativeBarFormat associé à une règle de mise en forme conditionnelle de barre de données. |
| [GetMinCfvo](./getmincfvo/) | Obtenez ou définissez l'objet de valeur minimale de cette DataBar. Impossible de définir null ou CFValueObject avec le type FormatConditionValueType.Max. |
| [GetMaxCfvo](./getmaxcfvo/) | Obtenez ou définissez l'objet de valeur maximale de cette DataBar. Impossible de définir null ou CFValueObject avec le type FormatConditionValueType.Min. |
| [GetColor](./getcolor/) | Obtenez ou définissez la couleur de cette DataBar. |
| [SetColor](./setcolor/) | Obtenez ou définissez la couleur de cette DataBar. |
| [GetMinLength](./getminlength/) | Représente la longueur minimale de la barre de données. |
| [SetMinLength](./setminlength/) | Représente la longueur minimale de la barre de données. |
| [GetMaxLength](./getmaxlength/) | Représente la longueur maximale de la barre de données. |
| [SetMaxLength](./setmaxlength/) | Représente la longueur maximale de la barre de données. |
| [GetShowValue](./getshowvalue/) | Obtenez ou définissez le drapeau indiquant s'il faut afficher les valeurs des cellules sur lesquelles cette barre de données est appliquée. La valeur par défaut est true. |
| [SetShowValue](./setshowvalue/) | Obtenez ou définissez le drapeau indiquant s'il faut afficher les valeurs des cellules sur lesquelles cette barre de données est appliquée. La valeur par défaut est true. |
| [ToImage](./toimage/) | Rendu de la barre de données dans la cellule en tableau d'octets d'image. |
