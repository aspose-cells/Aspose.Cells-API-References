---
title: "Classe FormatConditionCollection"
linktitle: "FormatConditionCollection"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe FormatConditionCollection. Encapsule l'objet qui représente formatconditioncollection en Go."
type: docs
weight: 200
url: /fr/go-cpp/formatconditioncollection/
---

## FormatConditionCollection class

Représente la mise en forme conditionnelle. Les FormatConditions peuvent contenir jusqu'à trois formats conditionnels.

```go

type FormatConditionCollection struct  {
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
| [Add](./add/) | Ajoute une condition de formatage et la plage de cellules affectée aux FormatConditions. Les FormatConditions peuvent contenir jusqu'à trois formats conditionnels. Les références aux autres feuilles ne sont pas autorisées dans les formules de formatage conditionnel. |
| [AddArea](./addarea/) | Ajoute une plage de cellules formatée conditionnellement. |
| [AddCondition_FormatConditionType_OperatorType_String_String](./addcondition_formatconditiontype_operatortype_string_string/) | Ajoute une condition de formatage. |
| [AddCondition_FormatConditionType](./addcondition_formatconditiontype/) | Ajoute une condition de format. |
| [GetCount](./getcount/) | Obtient le nombre de conditions. |
| [GetRangeCount](./getrangecount/) | Obtient le nombre de plages formatées conditionnellement. |
| [Get](./get/) | Obtient la condition de formatage par indice. |
| [GetCellArea](./getcellarea/) | Obtient la plage de cellules formatée conditionnellement par indice. |
| [RemoveArea_Int](./removearea_int/) | Supprime la plage de cellules formatée conditionnellement par indice. |
| [RemoveArea_Int_Int_Int_Int](./removearea_int_int_int_int/) | Supprime le formatage conditionnel dans la plage. |
| [RemoveCondition](./removecondition/) | Supprime la condition de formatage par indice. |
