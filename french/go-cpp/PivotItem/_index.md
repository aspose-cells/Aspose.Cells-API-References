---
title: "Classe PivotItem"
linktitle: "PivotItem"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe PivotItem. Encapsule l'objet qui représente pivotitem en Go."
type: docs
weight: 200
url: /fr/go-cpp/pivotitem/
---

## PivotItem class

Représente un élément dans un rapport PivotField.

```go

type PivotItem struct  {
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
| [IsHidden](./ishidden/) | Obtient et définit si l'élément pivot est masqué. |
| [SetIsHidden](./setishidden/) | Obtient et définit si l'élément pivot est masqué. |
| [GetPosition](./getposition/) | Spécifie l'index de cet élément parmi tous les PivotItems du champ. |
| [SetPosition](./setposition/) | Spécifie l'index de cet élément parmi tous les PivotItems du champ. |
| [GetPositionInSameParentNode](./getpositioninsameparentnode/) | Spécifie l'index de position dans les PivotItems sous le même nœud parent. |
| [SetPositionInSameParentNode](./setpositioninsameparentnode/) | Spécifie l'index de position dans les PivotItems sous le même nœud parent. |
| [Move](./move/) | Déplace l'élément vers le haut ou vers le bas |
| [IsDetailHidden](./isdetailhidden/) | Obtient et définit si le détail de cet élément pivot est masqué. |
| [SetIsDetailHidden](./setisdetailhidden/) | Obtient et définit si le détail de cet élément pivot est masqué. |
| [IsCalculatedItem](./iscalculateditem/) | Indique si cet élément pivot est un élément de formule calculée. |
| [GetFormula](./getformula/) | Obtient la formule de cet élément calculé. Fonctionne uniquement lorsque cet élément est un élément calculé. |
| [IsMissing](./ismissing/) | Indique si l'élément a été supprimé de la source de données. |
| [GetStringValue](./getstringvalue/) | Obtient la valeur chaîne de l'élément pivot. Si la valeur est nulle, elle renverra "". |
| [GetDoubleValue](./getdoublevalue/) | Obtient la valeur double de l'élément pivot. Si la valeur est nulle ou n'est pas un nombre, elle renverra 0. |
| [GetDateTimeValue](./getdatetimevalue/) | Obtient la valeur date/heure de l'élément pivot. Si la valeur est nulle, elle renverra DateTime.MinValue. |
| [GetValue](./getvalue/) | Obtient la valeur de l'élément pivot |
| [GetName](./getname/) | Obtient le nom de l'élément pivot. |
| [SetName](./setname/) | Obtient le nom de l'élément pivot. |
