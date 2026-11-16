---
title: "Classe Slicer"
linktitle: "Slicer"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe Slicer. Encapsule l'objet qui représente le slicer dans Go."
type: docs
weight: 200
url: /fr/go-cpp/slicer/
---

## Slicer class

Description résumée de la vue Slicer View.

```go

type Slicer struct  {
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
| [GetSortOrderType](./getsortordertype/) | Indique le type de tri des éléments. |
| [SetSortOrderType](./setsortordertype/) | Indique le type de tri des éléments. |
| [GetShowMissing](./getshowmissing/) | Indique s'il faut afficher les éléments supprimés de la source de données. |
| [SetShowMissing](./setshowmissing/) | Indique s'il faut afficher les éléments supprimés de la source de données. |
| [GetShowTypeOfItemsWithNoData](./getshowtypeofitemswithnodata/) | Indique s'il faut afficher les éléments supprimés de la source de données. |
| [SetShowTypeOfItemsWithNoData](./setshowtypeofitemswithnodata/) | Indique s'il faut afficher les éléments supprimés de la source de données. |
| [GetShowAllItems](./getshowallitems/) | Indique s'il faut afficher tous les éléments même s'il n'y a pas de données ou s'ils sont supprimés. La valeur par défaut est true; |
| [SetShowAllItems](./setshowallitems/) | Indique s'il faut afficher tous les éléments même s'il n'y a pas de données ou s'ils sont supprimés. La valeur par défaut est true; |
| [AddPivotConnection](./addpivotconnection/) | Ajoute une connexion de tableau croisé dynamique. |
| [RemovePivotConnection](./removepivotconnection/) | Supprime la connexion du tableau croisé dynamique. |
| [GetLockedPosition](./getlockedposition/) | Indique si le slicer spécifié peut être déplacé ou redimensionné via l'interface utilisateur. |
| [SetLockedPosition](./setlockedposition/) | Indique si le slicer spécifié peut être déplacé ou redimensionné via l'interface utilisateur. |
| [Refresh](./refresh/) | Actualisation des éléments du slicer à partir des tableaux croisés dynamiques associés. |
| [GetShape](./getshape/) | Renvoie l'objet Shape associé au slicer spécifié. Lecture seule. |
| [GetSlicerCache](./getslicercache/) | Renvoie l'objet SlicerCache associé au slicer. Lecture seule. |
| [GetWorksheet](./getworksheet/) | Renvoie l'objet Worksheet qui contient ce slicer. Lecture seule. |
| [GetStyleType](./getstyletype/) | Spécifiez le type de style de slicer intégré. Le type par défaut est SlicerStyleLight1. |
| [SetStyleType](./setstyletype/) | Spécifiez le type de style de slicer intégré. Le type par défaut est SlicerStyleLight1. |
| [GetName](./getname/) | Renvoie ou définit le nom du slicer spécifié |
| [SetName](./setname/) | Renvoie ou définit le nom du slicer spécifié |
| [GetCaption](./getcaption/) | Renvoie ou définit la légende du slicer spécifié. |
| [SetCaption](./setcaption/) | Renvoie ou définit la légende du slicer spécifié. |
| [GetFirstItemIndex](./getfirstitemindex/) | Spécifie l'index basé sur zéro du premier élément du slicer. |
| [SetFirstItemIndex](./setfirstitemindex/) | Spécifie l'index basé sur zéro du premier élément du slicer. |
|[SelectItems](./selectitems/) |  | 
| [UnselectItems](./unselectitems/) | Supprimer les libellés de filtre sélectionnés. |
| [ClearFilter](./clearfilter/) | Supprimer les filtres |
| [GetShowCaption](./getshowcaption/) | Indique si l'en-tête du slicer est visible. La valeur par défaut est true |
| [SetShowCaption](./setshowcaption/) | Indique si l'en-tête du slicer est visible. La valeur par défaut est true |
| [GetNumberOfColumns](./getnumberofcolumns/) | Renvoie ou définit le nombre de colonnes dans le slicer. La valeur par défaut est 1. |
| [SetNumberOfColumns](./setnumberofcolumns/) | Renvoie ou définit le nombre de colonnes dans le slicer. La valeur par défaut est 1. |
| [GetColumnWidthPixel](./getcolumnwidthpixel/) | Obtient ou définit la largeur de chaque colonne du slicer, en unités de pixels. |
| [SetColumnWidthPixel](./setcolumnwidthpixel/) | Obtient ou définit la largeur de chaque colonne du slicer, en unités de pixels. |
| [GetColumnWidth](./getcolumnwidth/) | Renvoie ou définit la largeur de chaque colonne du slicer en unités de points. |
| [SetColumnWidth](./setcolumnwidth/) | Renvoie ou définit la largeur de chaque colonne du slicer en unités de points. |
| [GetRowHeightPixel](./getrowheightpixel/) | Renvoie ou définit la hauteur de chaque ligne du slicer spécifié, en unités de pixels. |
| [SetRowHeightPixel](./setrowheightpixel/) | Renvoie ou définit la hauteur de chaque ligne du slicer spécifié, en unités de pixels. |
| [GetRowHeight](./getrowheight/) | Renvoie ou définit la hauteur de chaque ligne du slicer spécifié en unités de points. |
| [SetRowHeight](./setrowheight/) | Renvoie ou définit la hauteur de chaque ligne du slicer spécifié en unités de points. |
