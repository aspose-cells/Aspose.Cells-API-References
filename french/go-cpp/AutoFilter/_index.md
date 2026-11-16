---
title: "Classe AutoFilter"
linktitle: "AutoFilter"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe AutoFilter. Encapsule l'objet qui représente le filtre automatique en Go."
type: docs
weight: 200
url: /fr/go-cpp/autofilter/
---

## AutoFilter class

Représente le filtrage automatique pour la feuille de calcul spécifiée.

```go

type AutoFilter struct  {
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
| [GetSorter](./getsorter/) | Obtient le trieur de données. |
| [SetRange_Int_Int_Int](./setrange_int_int_int/) | Définit la plage à laquelle le filtre automatique spécifié s'applique. |
| [GetCellArea](./getcellarea/) | Obtient la CellArea où ce filtre automatique s'applique. |
| [GetCellArea_Bool](./getcellarea_bool/) | Obtient le Aspose.Cells.CellArea où le filtre automatique spécifié s'applique. |
| [GetRange](./getrange/) | Représente la plage à laquelle le filtre automatique spécifié s'applique. |
| [SetRange_String](./setrange_string/) | Représente la plage à laquelle le filtre automatique spécifié s'applique. |
| [AddFilter](./addfilter/) | Ajoute un filtre pour une colonne de filtre. |
| [AddDateFilter](./adddatefilter/) | Ajoute un filtre de date. |
| [RemoveDateFilter](./removedatefilter/) | Supprime un filtre de date. |
| [RemoveFilter_Int_String](./removefilter_int_string/) | Supprime un filtre pour une colonne de filtre. |
| [Filter](./filter/) | Filtre une liste avec les critères spécifiés. |
| [FilterTop10](./filtertop10/) | Filtrer les 10 meilleurs éléments de la liste |
| [Dynamic_Filter](./dynamic_filter/) | Ajoute un filtre dynamique. |
| [AddFontColorFilter](./addfontcolorfilter/) | Ajoute un filtre de couleur de police. |
| [AddFillColorFilter](./addfillcolorfilter/) | Ajoute un filtre de couleur de remplissage. |
| [AddIconFilter](./addiconfilter/) | Ajoute un filtre d'icône. |
| [MatchBlanks](./matchblanks/) | Correspond à toutes les cellules vides de la liste. |
| [MatchNonBlanks](./matchnonblanks/) | Correspond à toutes les cellules non vides de la liste. |
| [Custom_Int_FilterOperatorType_Object](./custom_int_filteroperatortype_object/) | Filtre une liste avec un critère personnalisé. |
| [Custom_Int_FilterOperatorType_Object_Bool_FilterOperatorType_Object](./custom_int_filteroperatortype_object_bool_filteroperatortype_object/) | Filtre une liste avec des critères personnalisés. |
| [ShowAll](./showall/) | Rendre visibles toutes les lignes. |
| [RemoveFilter_Int](./removefilter_int/) | Supprimer le filtre spécifique. |
| [Refresh](./refresh/) | Actualiser les filtres automatiques pour masquer ou afficher les lignes. |
| [Refresh_Bool](./refresh_bool/) | Obtient les index de toutes les lignes masquées. |
| [GetShowFilterButton](./getshowfilterbutton/) | Indique si le bouton AutoFilter pour cette colonne est visible. |
| [SetShowFilterButton](./setshowfilterbutton/) | Indique si le bouton AutoFilter pour cette colonne est visible. |
| [GetFilterColumns](./getfiltercolumns/) | Obtient la collection des colonnes de filtre. |
