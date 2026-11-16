---
title: "Classe TxtSaveOptions"
linktitle: "TxtSaveOptions"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe TxtSaveOptions. Encapsule l'objet qui représente txtsaveoptions en Go."
type: docs
weight: 200
url: /fr/go-cpp/txtsaveoptions/
---

## TxtSaveOptions class

Représente les options d'enregistrement pour le format csv/tab délimité/autre format texte.

```go

type TxtSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewTxtSaveOptions](./newtxtsaveoptions/) | Crée des options d'enregistrement de fichier texte. |
| [NewTxtSaveOptions_SaveFormat](./newtxtsaveoptions_saveformat/) | Crée des options d'enregistrement de fichier texte. |
| [NewTxtSaveOptions_SaveOptions](./newtxtsaveoptions_saveoptions/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetSeparator](./getseparator/) | Obtient et définit le délimiteur de caractères du fichier texte. |
| [SetSeparator](./setseparator/) | Obtient et définit le délimiteur de caractères du fichier texte. |
| [GetSeparatorString](./getseparatorstring/) | Obtient et définit une valeur chaîne comme séparateur. |
| [SetSeparatorString](./setseparatorstring/) | Obtient et définit une valeur chaîne comme séparateur. |
| [GetEncoding](./getencoding/) | Obtient et définit l'encodage par défaut. |
| [SetEncoding](./setencoding/) | Obtient et définit l'encodage par défaut. |
| [GetQuoteType](./getquotetype/) | Obtient ou définit comment citer les valeurs dans le fichier texte exporté. |
| [SetQuoteType](./setquotetype/) | Obtient ou définit comment citer les valeurs dans le fichier texte exporté. |
| [GetFormatStrategy](./getformatstrategy/) | Obtient et définit la stratégie de format lors de l'exportation de la valeur de la cellule en tant que chaîne. |
| [SetFormatStrategy](./setformatstrategy/) | Obtient et définit la stratégie de format lors de l'exportation de la valeur de la cellule en tant que chaîne. |
| [GetTrimLeadingBlankRowAndColumn](./gettrimleadingblankrowandcolumn/) | Indique si les lignes et colonnes vides en début doivent être supprimées comme le fait MS Excel. La valeur par défaut est true. |
| [SetTrimLeadingBlankRowAndColumn](./settrimleadingblankrowandcolumn/) | Indique si les lignes et colonnes vides en début doivent être supprimées comme le fait MS Excel. La valeur par défaut est true. |
| [GetTrimTailingBlankCells](./gettrimtailingblankcells/) | Indique si les cellules vides en fin de ligne doivent être supprimées. La valeur par défaut est false. |
| [SetTrimTailingBlankCells](./settrimtailingblankcells/) | Indique si les cellules vides en fin de ligne doivent être supprimées. La valeur par défaut est false. |
| [GetKeepSeparatorsForBlankRow](./getkeepseparatorsforblankrow/) | Indique si des séparateurs doivent être générés pour une ligne vide. La valeur par défaut est false, donc le contenu d'une ligne vide sera vide. |
| [SetKeepSeparatorsForBlankRow](./setkeepseparatorsforblankrow/) | Indique si des séparateurs doivent être générés pour une ligne vide. La valeur par défaut est false, donc le contenu d'une ligne vide sera vide. |
| [GetExportArea](./getexportarea/) | La plage de cellules à exporter. |
| [SetExportArea](./setexportarea/) | La plage de cellules à exporter. |
| [GetExportQuotePrefix](./getexportquoteprefix/) | Indique si le signe apostrophe simple doit être exporté comme partie de la valeur d'une cellule lorsque Style.QuotePrefix est vrai pour celle‑ci. La valeur par défaut est false. |
| [SetExportQuotePrefix](./setexportquoteprefix/) | Indique si le signe apostrophe simple doit être exporté comme partie de la valeur d'une cellule lorsque Style.QuotePrefix est vrai pour celle‑ci. La valeur par défaut est false. |
| [GetExportAllSheets](./getexportallsheets/) | Indique si toutes les feuilles doivent être exportées vers le fichier texte. Si false, seule la feuille active est exportée, comme dans MS Excel. |
| [SetExportAllSheets](./setexportallsheets/) | Indique si toutes les feuilles doivent être exportées vers le fichier texte. Si false, seule la feuille active est exportée, comme dans MS Excel. |
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
