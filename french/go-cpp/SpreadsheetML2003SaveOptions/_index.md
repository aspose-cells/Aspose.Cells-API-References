---
title: "Classe SpreadsheetML2003SaveOptions"
linktitle: "SpreadsheetML2003SaveOptions"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe SpreadsheetML2003SaveOptions. Encapsule l'objet qui représente spreadsheetml2003saveoptions en Go."
type: docs
weight: 200
url: /fr/go-cpp/spreadsheetml2003saveoptions/
---

## SpreadsheetML2003SaveOptions class

Représente les options d'enregistrement du fichier Excel 2003 spreadml.

```go

type SpreadsheetML2003SaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewSpreadsheetML2003SaveOptions](./newspreadsheetml2003saveoptions/) | Crée les options pour enregistrer un fichier Excel 2003 spreadml. |
| [NewSpreadsheetML2003SaveOptions_SaveOptions](./newspreadsheetml2003saveoptions_saveoptions/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [IsIndentedFormatting](./isindentedformatting/) | Force l'indentation des éléments enfants. |
| [SetIsIndentedFormatting](./setisindentedformatting/) | Force l'indentation des éléments enfants. |
| [GetLimitAsXls](./getlimitasxls/) | Limite en tant que xls, l'index maximal de ligne est 65535 et l'index maximal de colonne est 255. |
| [SetLimitAsXls](./setlimitasxls/) | Limite en tant que xls, l'index maximal de ligne est 65535 et l'index maximal de colonne est 255. |
| [GetExportColumnIndexOfCell](./getexportcolumnindexofcell/) | La valeur par défaut est false, cela signifie que l'index de colonne sera ignoré si la cellule est contiguë à la cellule précédente. |
| [SetExportColumnIndexOfCell](./setexportcolumnindexofcell/) | La valeur par défaut est false, cela signifie que l'index de colonne sera ignoré si la cellule est contiguë à la cellule précédente. |
| [GetSaveFormat](./getsaveformat/) | Obtient le format du fichier à enregistrer. |
| [GetClearData](./getcleardata/) | Rendre le classeur vide après l'enregistrement du fichier. |
| [SetClearData](./setcleardata/) | Rendre le classeur vide après l'enregistrement du fichier. |
| [GetCachedFileFolder](./getcachedfilefolder/) | Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |
| [SetCachedFileFolder](./setcachedfilefolder/) | Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |
| [GetValidateMergedAreas](./getvalidatemergedareas/) | Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier. |
| [SetValidateMergedAreas](./setvalidatemergedareas/) | Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier. |
| [GetMergeAreas](./getmergeareas/) | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. |
| [SetMergeAreas](./setmergeareas/) | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. |
| [GetCreateDirectory](./getcreatedirectory/) | Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier. |
| [SetCreateDirectory](./setcreatedirectory/) | Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier. |
| [GetSortNames](./getsortnames/) | Indique s'il faut trier les noms définis avant d'enregistrer le fichier. |
| [SetSortNames](./setsortnames/) | Indique s'il faut trier les noms définis avant d'enregistrer le fichier. |
| [GetSortExternalNames](./getsortexternalnames/) | Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier. |
| [SetSortExternalNames](./setsortexternalnames/) | Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier. |
| [GetRefreshChartCache](./getrefreshchartcache/) | Indique s'il faut mettre en cache les dernières données du graphique. |
| [SetRefreshChartCache](./setrefreshchartcache/) | Indique s'il faut mettre en cache les dernières données du graphique. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | Vérifie les restrictions du fichier Excel lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Si vous saisissez une valeur supérieure à 32 K, elle sera tronquée. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | Vérifie les restrictions du fichier Excel lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Si vous saisissez une valeur supérieure à 32 K, elle sera tronquée. |
| [GetUpdateSmartArt](./getupdatesmartart/) | Indique s'il faut mettre à jour le paramètre SmartArt. La valeur par défaut est false. |
| [SetUpdateSmartArt](./setupdatesmartart/) | Indique s'il faut mettre à jour le paramètre SmartArt. La valeur par défaut est false. |
| [GetEncryptDocumentProperties](./getencryptdocumentproperties/) | Indique s'il faut chiffrer les propriétés du document lors de l'enregistrement au format .xls. La valeur par défaut est true. |
| [SetEncryptDocumentProperties](./setencryptdocumentproperties/) | Indique s'il faut chiffrer les propriétés du document lors de l'enregistrement au format .xls. La valeur par défaut est true. |
