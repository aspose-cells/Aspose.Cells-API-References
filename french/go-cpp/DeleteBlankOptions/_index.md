---
title: "DeleteBlankOptions Classe"
linktitle: "DeleteBlankOptions"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "DeleteBlankOptions class. Encapsule l'objet qui représente deleteblankoptions en Go."
type: docs
weight: 200
url: /fr/go-cpp/deleteblankoptions/
---

## DeleteBlankOptions class

Représente le paramètre de suppression des cellules/lignes/colonnes vides.

```go

type DeleteBlankOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewDeleteBlankOptions](./newdeleteblankoptions/) | Constructeur par défaut. |
| [NewDeleteBlankOptions_DeleteOptions](./newdeleteblankoptions_deleteoptions/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetEmptyStringAsBlank](./getemptystringasblank/) | Indique si une cellule sera considérée comme vide lorsque sa valeur est une chaîne vide. La valeur par défaut est true. |
| [SetEmptyStringAsBlank](./setemptystringasblank/) | Indique si une cellule sera considérée comme vide lorsque sa valeur est une chaîne vide. La valeur par défaut est true. |
| [GetEmptyFormulaValueAsBlank](./getemptyformulavalueasblank/) | Indique si une cellule sera considérée comme vide lorsqu'il s'agit d'une formule et que le résultat calculé est nul ou une chaîne vide. La valeur par défaut est false. |
| [SetEmptyFormulaValueAsBlank](./setemptyformulavalueasblank/) | Indique si une cellule sera considérée comme vide lorsqu'il s'agit d'une formule et que le résultat calculé est nul ou une chaîne vide. La valeur par défaut est false. |
| [GetDrawingsAsBlank](./getdrawingsasblank/) | Indique si les objets liés aux dessins tels que l'image, la forme, le graphique... seront considérés comme vides. La valeur par défaut est true. |
| [SetDrawingsAsBlank](./setdrawingsasblank/) | Indique si les objets liés aux dessins tels que l'image, la forme, le graphique... seront considérés comme vides. La valeur par défaut est true. |
| [GetMergedCellsShrinkType](./getmergedcellsshrinktype/) | Indique comment traiter les cellules fusionnées lors de la suppression des lignes/colonnes vides. |
| [SetMergedCellsShrinkType](./setmergedcellsshrinktype/) | Indique comment traiter les cellules fusionnées lors de la suppression des lignes/colonnes vides. |
| [GetStartIndex](./getstartindex/) | Spécifie l'index de ligne/colonne de départ de la plage à vérifier et à supprimer les lignes/colonnes vides. |
| [SetStartIndex](./setstartindex/) | Spécifie l'index de ligne/colonne de départ de la plage à vérifier et à supprimer les lignes/colonnes vides. |
| [GetEndIndex](./getendindex/) | Spécifie l'index de ligne/colonne de fin (inclusif) de la plage à vérifier et à supprimer les lignes/colonnes vides. La valeur par défaut est -1 et -1 signifie la plage maximale de tous les objets (cellules, dessins, ...) qui doivent être vérifiés. |
| [SetEndIndex](./setendindex/) | Spécifie l'index de ligne/colonne de fin (inclusif) de la plage à vérifier et à supprimer les lignes/colonnes vides. La valeur par défaut est -1 et -1 signifie la plage maximale de tous les objets (cellules, dessins, ...) qui doivent être vérifiés. |
| [GetUpdateReference](./getupdatereference/) | Indique si les références de mise à jour dans d'autres feuilles de calcul. |
| [SetUpdateReference](./setupdatereference/) | Indique si les références de mise à jour dans d'autres feuilles de calcul. |
| [GetFormulaChangeMonitor](./getformulachangemonitor/) | Obtient/definit le moniteur pour suivre les modifications causées par la suppression. |
| [SetFormulaChangeMonitor](./setformulachangemonitor/) | Obtient/definit le moniteur pour suivre les modifications causées par la suppression. |
