---
title: "Classe PivotTableCollection"
linktitle: "PivotTableCollection"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe PivotTableCollection. Encapsule l'objet qui représente pivottablecollection en Go."
type: docs
weight: 200
url: /fr/go-cpp/pivottablecollection/
---

## PivotTableCollection class

Représente la collection de tous les objets PivotTable sur la feuille de calcul spécifiée.

```go

type PivotTableCollection struct  {
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
| [Dispose](./dispose/) | Effectue les tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées. |
| [Add_String_Int_Int](./add_string_int_int/) | Ajoute un nouveau PivotTable à la ligne et à la colonne spécifiées de la feuille de calcul avec les options par défaut. |
| [Add_String_Int_Int_String_Bool_Bool](./add_string_int_int_string_bool_bool/) | Ajoute un nouveau PivotTable avec la mise en page et le style hérités d'Excel 97-2003. |
| [Add_String_String_String_Bool_Bool](./add_string_string_string_bool_bool/) | Ajoute un nouveau PivotTable. |
| [Add_PivotTable_String_String](./add_pivottable_string_string/) | Ajoute un nouveau PivotTable basé sur un autre PivotTable. |
| [Add_PivotTable_Int_Int_String](./add_pivottable_int_int_string/) | Ajoute un nouveau PivotTable basé sur un autre PivotTable. |
| [Add_stringArray_Bool_PivotPageFields_String_String](./add_stringarray_bool_pivotpagefields_string_string/) | Ajoute un nouvel objet PivotTable à la collection avec plusieurs plages de consolidation comme source de données. |
| [Add_stringArray_Bool_PivotPageFields_Int_Int_String](./add_stringarray_bool_pivotpagefields_int_int_string/) | Ajoute un nouvel objet PivotTable à la collection avec plusieurs plages de consolidation comme source de données. |
| [Get_Int](./get_int/) | Obtient le rapport PivotTable par indice. |
| [Get_String](./get_string/) | Obtient le rapport PivotTable par le nom du pivottable. |
| [Get_Int_Int](./get_int_int/) | Obtient le rapport PivotTable par la position du pivottable. |
| [Clear](./clear/) | Efface toutes les tables pivot. |
| [Remove_PivotTable](./remove_pivottable/) | Supprime le PivotTable spécifié et supprime les données du PivotTable. |
| [Remove_PivotTable_Bool](./remove_pivottable_bool/) | Supprime le PivotTable spécifié. |
| [RemoveAt_Int](./removeat_int/) | Supprime le PivotTable à l'indice spécifié et supprime les données du PivotTable. |
| [RemoveAt_Int_Bool](./removeat_int_bool/) | Supprime le PivotTable à l'indice spécifié. |
| [GetCount](./getcount/) | Obtient le nombre d'éléments contenus dans l'instance. |
