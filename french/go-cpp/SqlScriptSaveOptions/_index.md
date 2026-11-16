---
title: "Classe SqlScriptSaveOptions"
linktitle: "SqlScriptSaveOptions"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe SqlScriptSaveOptions. Encapsule l'objet qui représente sqlscriptsaveoptions en Go."
type: docs
weight: 200
url: /fr/go-cpp/sqlscriptsaveoptions/
---

## SqlScriptSaveOptions class

Représente les options d'enregistrement du sql.

```go

type SqlScriptSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewSqlScriptSaveOptions](./newsqlscriptsaveoptions/) | Crée des options pour enregistrer le fichier sql. |
| [NewSqlScriptSaveOptions_SaveOptions](./newsqlscriptsaveoptions_saveoptions/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetCheckIfTableExists](./getcheckiftableexists/) | Vérifie si le nom de la table existe avant la création |
| [SetCheckIfTableExists](./setcheckiftableexists/) | Vérifie si le nom de la table existe avant la création |
| [GetColumnTypeMap](./getcolumntypemap/) | Obtient et définit la correspondance des types de colonnes pour différentes bases de données. |
| [SetColumnTypeMap](./setcolumntypemap/) | Obtient et définit la correspondance des types de colonnes pour différentes bases de données. |
| [GetCheckAllDataForColumnType](./getcheckalldataforcolumntype/) | Vérifie toutes les données pour trouver le type de données des colonnes. |
| [SetCheckAllDataForColumnType](./setcheckalldataforcolumntype/) | Vérifie toutes les données pour trouver le type de données des colonnes. |
| [GetAddBlankLineBetweenRows](./getaddblanklinebetweenrows/) | Insère une ligne vide entre chaque donnée. |
| [SetAddBlankLineBetweenRows](./setaddblanklinebetweenrows/) | Insère une ligne vide entre chaque donnée. |
| [GetSeparator](./getseparator/) | Obtient et définit le séparateur de caractères du script sql. |
| [SetSeparator](./setseparator/) | Obtient et définit le séparateur de caractères du script sql. |
| [GetOperatorType](./getoperatortype/) | Obtient et définit le type d'opérateur du sql. |
| [SetOperatorType](./setoperatortype/) | Obtient et définit le type d'opérateur du sql. |
| [GetPrimaryKey](./getprimarykey/) | Représente la colonne qui est la clé primaire de la table de données. |
| [SetPrimaryKey](./setprimarykey/) | Représente la colonne qui est la clé primaire de la table de données. |
| [GetCreateTable](./getcreatetable/) | Indique si l'exportation du sql de création de table est activée. |
| [SetCreateTable](./setcreatetable/) | Indique si l'exportation du sql de création de table est activée. |
| [GetIdName](./getidname/) | Obtient et définit le nom de la colonne d'identifiant. |
| [SetIdName](./setidname/) | Obtient et définit le nom de la colonne d'identifiant. |
| [GetStartId](./getstartid/) | Obtient et définit l'identifiant de départ. |
| [SetStartId](./setstartid/) | Obtient et définit l'identifiant de départ. |
| [GetTableName](./gettablename/) | Obtient et définit le nom de la table. |
| [SetTableName](./settablename/) | Obtient et définit le nom de la table. |
| [GetExportAsString](./getexportasstring/) | Indique si toutes les données sont exportées sous forme de valeur chaîne. |
| [SetExportAsString](./setexportasstring/) | Indique si toutes les données sont exportées sous forme de valeur chaîne. |
| [GetSheetIndexes](./getsheetindexes/) | Représente les index des feuilles exportées. |
| [SetSheetIndexes](./setsheetindexes/) | Représente les index des feuilles exportées. |
| [GetExportArea](./getexportarea/) | Obtient ou définit la plage d'exportation. |
| [SetExportArea](./setexportarea/) | Obtient ou définit la plage d'exportation. |
| [GetHasHeaderRow](./gethasheaderrow/) | Indique si la plage contient une ligne d'en-tête. |
| [SetHasHeaderRow](./sethasheaderrow/) | Indique si la plage contient une ligne d'en-tête. |
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
