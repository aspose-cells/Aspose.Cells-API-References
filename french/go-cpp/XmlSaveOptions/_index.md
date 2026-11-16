---
title: "Classe XmlSaveOptions"
linktitle: "XmlSaveOptions"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe XmlSaveOptions. Encapsule l’objet qui représente xmlsaveoptions en Go."
type: docs
weight: 200
url: /fr/go-cpp/xmlsaveoptions/
---

## XmlSaveOptions class

Représente les options d'enregistrement du classeur au format xml.

```go

type XmlSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewXmlSaveOptions](./newxmlsaveoptions/) | Crée des options pour l’enregistrement d’un fichier XML. |
| [NewXmlSaveOptions_SaveOptions](./newxmlsaveoptions_saveoptions/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetSheetIndexes](./getsheetindexes/) | Représente les index des feuilles exportées. |
| [SetSheetIndexes](./setsheetindexes/) | Représente les index des feuilles exportées. |
| [GetExportArea](./getexportarea/) | Obtient ou définit la plage d'exportation. |
| [SetExportArea](./setexportarea/) | Obtient ou définit la plage d'exportation. |
| [GetHasHeaderRow](./gethasheaderrow/) | Indique si la plage contient une ligne d'en-tête. |
| [SetHasHeaderRow](./sethasheaderrow/) | Indique si la plage contient une ligne d'en-tête. |
| [GetXmlMapName](./getxmlmapname/) | Indique si la carte XML est exportée dans le fichier. |
| [SetXmlMapName](./setxmlmapname/) | Indique si la carte XML est exportée dans le fichier. |
| [GetSheetNameAsElementName](./getsheetnameaselementname/) | Indique si le nom de la feuille est exporté comme nom de l’élément. |
| [SetSheetNameAsElementName](./setsheetnameaselementname/) | Indique si le nom de la feuille est exporté comme nom de l’élément. |
| [GetDataAsAttribute](./getdataasattribute/) | Indique si l'exportation des données se fait sous forme d'attributs de l'élément. |
| [SetDataAsAttribute](./setdataasattribute/) | Indique si l'exportation des données se fait sous forme d'attributs de l'élément. |
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
