---
title: "Classe OoxmlSaveOptions"
linktitle: "OoxmlSaveOptions"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe OoxmlSaveOptions. Encapsule l'objet qui représente ooxmlsaveoptions en Go."
type: docs
weight: 200
url: /fr/go-cpp/ooxmlsaveoptions/
---

## OoxmlSaveOptions class

Représente les options d'enregistrement du fichier Office Open XML.

```go

type OoxmlSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewOoxmlSaveOptions](./newooxmlsaveoptions/) | Crée les options pour enregistrer le fichier Office Open XML. |
| [NewOoxmlSaveOptions_SaveFormat](./newooxmlsaveoptions_saveformat/) | Crée les options pour enregistrer le fichier Office Open XML. |
| [NewOoxmlSaveOptions_SaveOptions](./newooxmlsaveoptions_saveoptions/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetAsFlatOpc](./getasflatopc/) | Indique si l'enregistrement se fait sous forme de fichier OPC plat qui peut être généré par le SDK Open XML. |
| [SetAsFlatOpc](./setasflatopc/) | Indique si l'enregistrement se fait sous forme de fichier OPC plat qui peut être généré par le SDK Open XML. |
| [GetExportCellName](./getexportcellname/) | Indique si le nom de la cellule est exporté vers un fichier Excel2007 .xlsx (.xlsm, .xltx, .xltm). Si le fichier de sortie peut être accédé par SQL Server DTS, cette valeur doit être vraie. Mettre la valeur à false augmentera fortement les performances et réduira la taille du fichier lors de la création de gros fichiers. La valeur par défaut est true. |
| [SetExportCellName](./setexportcellname/) | Indique si le nom de la cellule est exporté vers un fichier Excel2007 .xlsx (.xlsm, .xltx, .xltm). Si le fichier de sortie peut être accédé par SQL Server DTS, cette valeur doit être vraie. Mettre la valeur à false augmentera fortement les performances et réduira la taille du fichier lors de la création de gros fichiers. La valeur par défaut est true. |
| [GetUpdateZoom](./getupdatezoom/) | Indique s'il faut mettre à jour le facteur d'échelle avant d'enregistrer le fichier si les propriétés PageSetup.FitToPagesWide et PageSetup.FitToPagesTall contrôlent la mise à l'échelle de la feuille de calcul. |
| [SetUpdateZoom](./setupdatezoom/) | Indique s'il faut mettre à jour le facteur d'échelle avant d'enregistrer le fichier si les propriétés PageSetup.FitToPagesWide et PageSetup.FitToPagesTall contrôlent la mise à l'échelle de la feuille de calcul. |
| [GetEnableZip64](./getenablezip64/) | Utilisez les extensions ZIP64 lors de l'écriture d'archives zip, si nécessaire. |
| [SetEnableZip64](./setenablezip64/) | Utilisez les extensions ZIP64 lors de l'écriture d'archives zip, si nécessaire. |
| [GetEmbedOoxmlAsOleObject](./getembedooxmlasoleobject/) | Indique si l'intégration des fichiers Ooxml d'OleObject en tant qu'objet ole est activée. |
| [SetEmbedOoxmlAsOleObject](./setembedooxmlasoleobject/) | Indique si l'intégration des fichiers Ooxml d'OleObject en tant qu'objet ole est activée. |
| [GetCompressionType](./getcompressiontype/) | Obtient et définit le type de compression pour le fichier ooxml. |
| [SetCompressionType](./setcompressiontype/) | Obtient et définit le type de compression pour le fichier ooxml. |
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
