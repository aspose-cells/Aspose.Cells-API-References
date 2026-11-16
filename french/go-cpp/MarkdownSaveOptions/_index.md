---
title: "MarkdownSaveOptions Classe"
linktitle: "MarkdownSaveOptions"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "MarkdownSaveOptions classe. Encapsule l'objet qui représente markdownsaveoptions en Go."
type: docs
weight: 200
url: /fr/go-cpp/markdownsaveoptions/
---

## MarkdownSaveOptions class

Représente les options d'enregistrement pour le markdown.

```go

type MarkdownSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewMarkdownSaveOptions](./newmarkdownsaveoptions/) | Crée des options pour enregistrer le document markdown |
| [NewMarkdownSaveOptions_SaveOptions](./newmarkdownsaveoptions_saveoptions/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetEncoding](./getencoding/) | Obtient et définit l'encodage par défaut. |
| [SetEncoding](./setencoding/) | Obtient et définit l'encodage par défaut. |
| [GetFormatStrategy](./getformatstrategy/) | Obtient et définit la stratégie de format lors de l'exportation de la valeur de la cellule en tant que chaîne. |
| [SetFormatStrategy](./setformatstrategy/) | Obtient et définit la stratégie de format lors de l'exportation de la valeur de la cellule en tant que chaîne. |
| [GetLineSeparator](./getlineseparator/) | Obtient et définit le séparateur de ligne. |
| [SetLineSeparator](./setlineseparator/) | Obtient et définit le séparateur de ligne. |
| [GetTableHeaderType](./gettableheadertype/) | Obtient et définit la façon de définir l'en-tête du tableau. |
| [SetTableHeaderType](./settableheadertype/) | Obtient et définit la façon de définir l'en-tête du tableau. |
| [GetSheetSet](./getsheetset/) | Obtient ou définit les feuilles à rendre. La valeur par défaut est toutes les feuilles visibles du classeur : Aspose.Cells.Rendering.SheetSet.Active. |
| [SetSheetSet](./setsheetset/) | Obtient ou définit les feuilles à rendre. La valeur par défaut est toutes les feuilles visibles du classeur : Aspose.Cells.Rendering.SheetSet.Active. |
| [GetImageOptions](./getimageoptions/) | Obtenez l'objet ImageOrPrintOptions avant l'exportation. |
| [GetExportImagesAsBase64](./getexportimagesasbase64/) | Spécifie si les images sont enregistrées au format Base64 dans le Markdown. La valeur par défaut est true. |
| [SetExportImagesAsBase64](./setexportimagesasbase64/) | Spécifie si les images sont enregistrées au format Base64 dans le Markdown. La valeur par défaut est true. |
| [GetCalculateFormula](./getcalculateformula/) | Indique s'il faut calculer les formules avant d'enregistrer le fichier markdown. |
| [SetCalculateFormula](./setcalculateformula/) | Indique s'il faut calculer les formules avant d'enregistrer le fichier markdown. |
| [GetExportHyperlinkAsReference](./getexporthyperlinkasreference/) | Indique s'il faut exporter les hyperliens en utilisant des définitions de référence au lieu du format en ligne. La valeur par défaut est false. |
| [SetExportHyperlinkAsReference](./setexporthyperlinkasreference/) | Indique s'il faut exporter les hyperliens en utilisant des définitions de référence au lieu du format en ligne. La valeur par défaut est false. |
| [GetAlignColumnPadding](./getaligncolumnpadding/) | Indique si l'alignement des colonnes est activé pour les tables Markdown générées. Lorsqu'il est activé, les colonnes sont alignées en remplissant le contenu des cellules avec le caractère spécifié (généralement ' ' pour les espaces). Définissez à '\0' pour désactiver l'alignement des colonnes (par défaut). |
| [SetAlignColumnPadding](./setaligncolumnpadding/) | Indique si l'alignement des colonnes est activé pour les tables Markdown générées. Lorsqu'il est activé, les colonnes sont alignées en remplissant le contenu des cellules avec le caractère spécifié (généralement ' ' pour les espaces). Définissez à '\0' pour désactiver l'alignement des colonnes (par défaut). |
| [GetSplitTablesByBlankRow](./getsplittablesbyblankrow/) | Indique si les lignes vides de la feuille de calcul doivent être traitées comme des séparateurs de tableau lors de l'exportation vers le Markdown. La valeur par défaut est false. |
| [SetSplitTablesByBlankRow](./setsplittablesbyblankrow/) | Indique si les lignes vides de la feuille de calcul doivent être traitées comme des séparateurs de tableau lors de l'exportation vers le Markdown. La valeur par défaut est false. |
| [GetOfficeMathOutputType](./getofficemathoutputtype/) | Indique comment les objets OfficeMath sont exportés vers le Markdown. La valeur par défaut est Image. |
| [SetOfficeMathOutputType](./setofficemathoutputtype/) | Indique comment les objets OfficeMath sont exportés vers le Markdown. La valeur par défaut est Image. |
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
