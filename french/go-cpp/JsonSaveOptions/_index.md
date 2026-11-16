---
title: "JsonSaveOptions Class"
linktitle: "JsonSaveOptions"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "JsonSaveOptions class. Encapsule l'objet qui représente jsonsaveoptions en Go."
type: docs
weight: 200
url: /fr/go-cpp/jsonsaveoptions/
---

## JsonSaveOptions class

Représente les options d'enregistrement du classeur au format JSON.

```go

type JsonSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewJsonSaveOptions](./newjsonsaveoptions/) | Crée des options pour enregistrer le fichier json. |
| [NewJsonSaveOptions_SaveOptions](./newjsonsaveoptions_saveoptions/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetExportStylePool](./getexportstylepool/) | Indique s'il faut exporter les styles collectivement ou individuellement pour chaque cellule. |
| [SetExportStylePool](./setexportstylepool/) | Indique s'il faut exporter les styles collectivement ou individuellement pour chaque cellule. |
| [GetExportHyperlinkType](./getexporthyperlinktype/) | Représente le type d'exportation d'hyperlien vers json. |
| [SetExportHyperlinkType](./setexporthyperlinktype/) | Représente le type d'exportation d'hyperlien vers json. |
| [GetSkipEmptyRows](./getskipemptyrows/) | Indique s'il faut ignorer les lignes vides. |
| [SetSkipEmptyRows](./setskipemptyrows/) | Indique s'il faut ignorer les lignes vides. |
| [GetSheetIndexes](./getsheetindexes/) | Représente les index des feuilles exportées. |
| [SetSheetIndexes](./setsheetindexes/) | Représente les index des feuilles exportées. |
| [GetSchemas](./getschemas/) | Le schéma json original de chaque feuille de calcul. |
| [SetSchemas](./setschemas/) | Le schéma json original de chaque feuille de calcul. |
| [GetExportArea](./getexportarea/) | Obtient ou définit la plage d'exportation. |
| [SetExportArea](./setexportarea/) | Obtient ou définit la plage d'exportation. |
| [GetHasHeaderRow](./gethasheaderrow/) | Indique si la plage contient une ligne d'en-tête. |
| [SetHasHeaderRow](./sethasheaderrow/) | Indique si la plage contient une ligne d'en-tête. |
| [GetExportAsString](./getexportasstring/) | Exporte la valeur chaîne des cellules vers json. |
| [SetExportAsString](./setexportasstring/) | Exporte la valeur chaîne des cellules vers json. |
| [GetIndent](./getindent/) | Indique l'indentation. |
| [SetIndent](./setindent/) | Indique l'indentation. |
| [GetExportNestedStructure](./getexportnestedstructure/) | Exporté en tant que structure Json hiérarchique parent-enfant. |
| [SetExportNestedStructure](./setexportnestedstructure/) | Exporté en tant que structure Json hiérarchique parent-enfant. |
| [GetExportEmptyCells](./getexportemptycells/) | Indique s'il faut exporter les cellules vides comme null. |
| [SetExportEmptyCells](./setexportemptycells/) | Indique s'il faut exporter les cellules vides comme null. |
| [GetAlwaysExportAsJsonObject](./getalwaysexportasjsonobject/) | Indique s'il faut toujours exporter Excel vers json en tant qu'objet, même s'il n'y a qu'une seule feuille de calcul dans le fichier. |
| [SetAlwaysExportAsJsonObject](./setalwaysexportasjsonobject/) | Indique s'il faut toujours exporter Excel vers json en tant qu'objet, même s'il n'y a qu'une seule feuille de calcul dans le fichier. |
| [GetToExcelStruct](./gettoexcelstruct/) | Indique si la conversion en structure json du fichier Excel. |
| [SetToExcelStruct](./settoexcelstruct/) | Indique si la conversion en structure json du fichier Excel. |
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
