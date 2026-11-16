---
title: "Classe PivotField"
linktitle: "PivotField"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe PivotField. Encapsule l'objet qui représente pivotfield en Go."
type: docs
weight: 200
url: /fr/go-cpp/pivotfield/
---

## PivotField class

Représente un champ dans un rapport de tableau croisé dynamique.

```go

type PivotField struct  {
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
| [GetPivotItems](./getpivotitems/) | Obtient les éléments pivot du champ pivot |
| [GetMaxValue](./getmaxvalue/) | Obtient la valeur maximale de ce champ. |
| [GetMinValue](./getminvalue/) | Obtient la valeur maximale de ce champ. |
| [GetGroupSettings](./getgroupsettings/) | Obtient les paramètres de groupe du champ pivot. |
| [InitPivotItems](./initpivotitems/) | Initialise les éléments pivot du champ pivot |
| [Group](./group/) | Regroupe automatiquement le champ. |
| [Group_PivotFieldGroupOptions](./group_pivotfieldgroupoptions/) | Regroupe le champ pivot avec des options. |
| [GroupBy](./groupby/) | Regroupe le champ de manière personnalisée. |
| [Ungroup](./ungroup/) | Dégroupe le champ pivot. |
| [GetPivotFilterByType](./getpivotfilterbytype/) | Obtient le filtre pivot du champ pivot par type |
| [GetFilters](./getfilters/) | Obtient tous les filtres pivot appliqués à ce champ pivot. |
| [ClearFilter](./clearfilter/) | Efface les paramètres de filtre sur ce champ pivot. |
| [FilterTop10](./filtertop10/) | Filtre par les valeurs du champ pivot de données. |
| [FilterByValue](./filterbyvalue/) | Filtre par les valeurs du champ pivot de données. |
| [FilterByLabel](./filterbylabel/) | Filtre par les légendes du champ pivot de ligne ou de colonne. |
| [FilterByDate](./filterbydate/) | Filtre par valeurs de date du champ pivot de ligne ou de colonne. |
| [IsCalculatedField](./iscalculatedfield/) | Indique si ce champ pivot est un champ calculé. |
| [GetFormula](./getformula/) | Obtient la formule du champ calculé. Ne fonctionne que pour les champs calculés. |
| [IsValuesField](./isvaluesfield/) | Indique si ce champ représente le champ de valeurs. |
| [GetBaseIndex](./getbaseindex/) | Représente l'index dans les champs pivot source. |
| [SetBaseIndex](./setbaseindex/) | Représente l'index dans les champs pivot source. |
| [GetPosition](./getposition/) | Représente l'index du champ PivotField dans la région. |
| [GetRegionType](./getregiontype/) | Spécifie la région du tableau croisé dynamique où ce champ est affiché. |
| [GetName](./getname/) | Représente le nom du champ PivotField. |
| [SetName](./setname/) | Représente le nom du champ PivotField. |
| [GetDisplayName](./getdisplayname/) | Représente le nom d'affichage du champ pivot dans la vue du tableau croisé dynamique. |
| [SetDisplayName](./setdisplayname/) | Représente le nom d'affichage du champ pivot dans la vue du tableau croisé dynamique. |
| [SetSubtotals_PivotFieldSubtotalType_Bool](./setsubtotals_pivotfieldsubtotaltype_bool/) | Définit comment sous-totaliser le champ spécifié. |
| [GetSubtotals_PivotFieldSubtotalType](./getsubtotals_pivotfieldsubtotaltype/) | Indique s'il faut afficher le sous-total spécifié pour ce champ pivot. |
| [GetSubtotals](./getsubtotals/) | Obtient ou définit les sous-totaux du champ. Seulement pour les champs pivot de ligne ou de colonne. |
| [SetSubtotals_PivotFieldSubtotalType](./setsubtotals_pivotfieldsubtotaltype/) | Obtient ou définit les sous-totaux du champ. Seulement pour les champs pivot de ligne ou de colonne. |
| [IsAutoSubtotals](./isautosubtotals/) | Indique si le champ spécifié affiche des sous-totaux automatiques. La valeur par défaut est vraie. |
| [SetIsAutoSubtotals](./setisautosubtotals/) | Indique si le champ spécifié affiche des sous-totaux automatiques. La valeur par défaut est vraie. |
| [GetAllowDraggingToRow](./getallowdraggingtorow/) | Indique si le champ spécifié peut être glissé vers la région de lignes. La valeur par défaut est vraie. |
| [SetAllowDraggingToRow](./setallowdraggingtorow/) | Indique si le champ spécifié peut être glissé vers la région de lignes. La valeur par défaut est vraie. |
| [GetAllowDraggingToColumn](./getallowdraggingtocolumn/) | Indique si le champ spécifié peut être glissé vers la région de colonnes. La valeur par défaut est vraie. |
| [SetAllowDraggingToColumn](./setallowdraggingtocolumn/) | Indique si le champ spécifié peut être glissé vers la région de colonnes. La valeur par défaut est vraie. |
| [GetAllowDraggingToPage](./getallowdraggingtopage/) | Indique si le champ spécifié peut être glissé vers la région de pages. La valeur par défaut est vraie. |
| [SetAllowDraggingToPage](./setallowdraggingtopage/) | Indique si le champ spécifié peut être glissé vers la région de pages. La valeur par défaut est vraie. |
| [GetAllowRemovingFromView](./getallowremovingfromview/) | Indique si ce champ pivot peut être supprimé de la vue du tableau croisé dynamique. La valeur par défaut est vraie. |
| [SetAllowRemovingFromView](./setallowremovingfromview/) | Indique si ce champ pivot peut être supprimé de la vue du tableau croisé dynamique. La valeur par défaut est vraie. |
| [GetAllowDraggingToData](./getallowdraggingtodata/) | Indique si le champ spécifié peut être glissé vers la région des valeurs. La valeur par défaut est vraie. |
| [SetAllowDraggingToData](./setallowdraggingtodata/) | Indique si le champ spécifié peut être glissé vers la région des valeurs. La valeur par défaut est vraie. |
| [IsMultipleItemSelectionAllowed](./ismultipleitemselectionallowed/) | Indique si plusieurs éléments peuvent être sélectionnés dans le champ de page. La valeur par défaut est fausse. |
| [SetIsMultipleItemSelectionAllowed](./setismultipleitemselectionallowed/) | Indique si plusieurs éléments peuvent être sélectionnés dans le champ de page. La valeur par défaut est fausse. |
| [IsRepeatItemLabels](./isrepeatitemlabels/) | Indique s'il faut répéter les libellés du champ dans la région. La valeur par défaut est fausse. |
| [SetIsRepeatItemLabels](./setisrepeatitemlabels/) | Indique s'il faut répéter les libellés du champ dans la région. La valeur par défaut est fausse. |
| [IsIncludeNewItemsInFilter](./isincludenewitemsinfilter/) | Indique s'il faut inclure de nouveaux éléments au champ dans le filtre manuel. La valeur par défaut est fausse. |
| [SetIsIncludeNewItemsInFilter](./setisincludenewitemsinfilter/) | Indique s'il faut inclure de nouveaux éléments au champ dans le filtre manuel. La valeur par défaut est fausse. |
| [IsInsertPageBreaksBetweenItems](./isinsertpagebreaksbetweenitems/) | Indique s'il faut insérer des sauts de page après chaque élément. La valeur par défaut est fausse. |
| [SetIsInsertPageBreaksBetweenItems](./setisinsertpagebreaksbetweenitems/) | Indique s'il faut insérer des sauts de page après chaque élément. La valeur par défaut est fausse. |
| [GetShowAllItems](./getshowallitems/) | Indique s'il faut afficher tous les éléments dans la vue du tableau croisé dynamique, même s'ils ne contiennent pas de données de synthèse. La valeur par défaut est false. |
| [SetShowAllItems](./setshowallitems/) | Indique s'il faut afficher tous les éléments dans la vue du tableau croisé dynamique, même s'ils ne contiennent pas de données de synthèse. La valeur par défaut est false. |
| [SortBy_SortOrder](./sortby_sortorder/) | Trie ce champ de tableau croisé dynamique. |
| [SortBy_SortOrder_Int_String](./sortby_sortorder_int_string/) | Trie ce champ de tableau croisé dynamique. |
| [GetSortSetting](./getsortsetting/) | Obtient tous les paramètres du tri automatique |
| [GetTop10AutoShowSettings](./gettop10autoshowsettings/) | Obtient les paramètres AutoShow Top 10 pour un champ de tableau croisé dynamique. |
| [Top10AutoShow](./top10autoshow/) | Configure les paramètres AutoShow Top10 pour ce champ de tableau croisé dynamique. |
| [GetFunction](./getfunction/) | Représente la fonction utilisée pour résumer ce champ de données du tableau croisé dynamique. |
| [SetFunction](./setfunction/) | Représente la fonction utilisée pour résumer ce champ de données du tableau croisé dynamique. |
| [ShowValuesAs](./showvaluesas/) | Affiche les valeurs du champ de données dans un format d'affichage différent lorsque le calcul ShowDataAs est utilisé. |
| [GetShowValuesSetting](./getshowvaluessetting/) | Obtient les paramètres d'affichage des valeurs lorsque le calcul ShowDataAs est utilisé. |
| [GetCurrentPageItem](./getcurrentpageitem/) | Représente l'élément de page actuellement sélectionné du champ de page pour filtrer les données. Valide uniquement pour les champs de page. |
| [SetCurrentPageItem](./setcurrentpageitem/) | Représente l'élément de page actuellement sélectionné du champ de page pour filtrer les données. Valide uniquement pour les champs de page. |
| [GetInsertBlankRow](./getinsertblankrow/) | Indique s'il faut insérer une ligne vide après chaque élément. Valide uniquement pour les champs de ligne. |
| [SetInsertBlankRow](./setinsertblankrow/) | Indique s'il faut insérer une ligne vide après chaque élément. Valide uniquement pour les champs de ligne. |
| [GetShowSubtotalAtTop](./getshowsubtotalattop/) | Indique s'il faut afficher les sous-totaux en haut ou en bas des éléments lorsque ShowInOutlineForm est vrai, alors |
| [SetShowSubtotalAtTop](./setshowsubtotalattop/) | Indique s'il faut afficher les sous-totaux en haut ou en bas des éléments lorsque ShowInOutlineForm est vrai, alors |
| [GetShowInOutlineForm](./getshowinoutlineform/) | Indique s'il faut disposer ce champ sous forme de plan dans la vue du tableau croisé dynamique. |
| [SetShowInOutlineForm](./setshowinoutlineform/) | Indique s'il faut disposer ce champ sous forme de plan dans la vue du tableau croisé dynamique. |
| [GetNumber](./getnumber/) | Représente le format d'affichage intégré des nombres et des dates. |
| [SetNumber](./setnumber/) | Représente le format d'affichage intégré des nombres et des dates. |
| [Get_NumberFormat](./get_numberformat/) | Représente le format d'affichage personnalisé des nombres et des dates. |
| [SetNumberFormat](./setnumberformat/) | Représente le format d'affichage personnalisé des nombres et des dates. |
| [HideAllDetails](./hidealldetails/) | Masque tous les détails |
| [ShowAllDetails](./showalldetails/) | Afficher tous les détails |
| [GetItems](./getitems/) | Obtenir toutes les étiquettes des éléments de tableau croisé dynamique dans ce champ. |
| [GetOriginalItems](./getoriginalitems/) | Obtenir les éléments de base originaux ; |
| [AddCalculatedItem](./addcalculateditem/) | Ajouter un élément de formule calculée au champ de tableau croisé dynamique. |
| [GetShowCompact](./getshowcompact/) | Indique s'il faut afficher les étiquettes du champ suivant dans la même colonne dans la vue du tableau croisé dynamique |
| [SetShowCompact](./setshowcompact/) | Indique s'il faut afficher les étiquettes du champ suivant dans la même colonne dans la vue du tableau croisé dynamique |
