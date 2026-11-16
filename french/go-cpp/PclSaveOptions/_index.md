---
title: "Classe PclSaveOptions"
linktitle: "PclSaveOptions"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe PclSaveOptions. Encapsule l'objet qui représente pclsaveoptions en Go."
type: docs
weight: 200
url: /fr/go-cpp/pclsaveoptions/
---

## PclSaveOptions class

Représente les options d'enregistrement d'un fichier Pcl.

```go

type PclSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewPclSaveOptions](./newpclsaveoptions/) | Crée les options pour enregistrer le fichier pcl. |
| [NewPclSaveOptions_PaginatedSaveOptions](./newpclsaveoptions_paginatedsaveoptions/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetEmbedFont](./getembedfont/) | Indique s'il faut incorporer la police dans le fichier Pcl de sortie. |
| [SetEmbedFont](./setembedfont/) | Indique s'il faut incorporer la police dans le fichier Pcl de sortie. |
| [AddPrinterFont](./addprinterfont/) | Ajoute des informations sur la police déjà ajoutée à l'imprimante par le fabricant. |
| [GetDefaultFont](./getdefaultfont/) | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le PDF ou l'image. Définissez la propriété DefaultFont, par exemple MingLiu ou MS Gothic, pour afficher ces caractères. Si cette propriété n'est pas définie, Aspose.Cells utilisera la police système par défaut pour afficher ces caractères Unicode. |
| [SetDefaultFont](./setdefaultfont/) | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le PDF ou l'image. Définissez la propriété DefaultFont, par exemple MingLiu ou MS Gothic, pour afficher ces caractères. Si cette propriété n'est pas définie, Aspose.Cells utilisera la police système par défaut pour afficher ces caractères Unicode. |
| [GetCheckWorkbookDefaultFont](./getcheckworkbookdefaultfont/) | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le PDF ou l'image. Réglez cette propriété sur true pour essayer d'utiliser d'abord la police par défaut du classeur afin d'afficher ces caractères. |
| [SetCheckWorkbookDefaultFont](./setcheckworkbookdefaultfont/) | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le PDF ou l'image. Réglez cette propriété sur true pour essayer d'utiliser d'abord la police par défaut du classeur afin d'afficher ces caractères. |
| [SetCheckFontCompatibility](./setcheckfontcompatibility/) | Indique s'il faut vérifier la compatibilité des polices pour chaque caractère du texte. |
| [GetCheckFontCompatibility](./getcheckfontcompatibility/) | Indique s'il faut vérifier la compatibilité des polices pour chaque caractère du texte. |
| [SetIsFontSubstitutionCharGranularity](./setisfontsubstitutionchargranularity/) | Indique s'il faut uniquement substituer la police du caractère lorsque la police de la cellule n'est pas compatible. |
| [IsFontSubstitutionCharGranularity](./isfontsubstitutionchargranularity/) | Indique s'il faut uniquement substituer la police du caractère lorsque la police de la cellule n'est pas compatible. |
| [GetOnePagePerSheet](./getonepagepersheet/) | Si OnePagePerSheet est true, tout le contenu d'une feuille sera exporté sur une seule page dans le résultat. La taille du papier du paramètre pagesetup sera invalide, mais les autres paramètres de pagesetup resteront effectifs. |
| [SetOnePagePerSheet](./setonepagepersheet/) | Si OnePagePerSheet est true, tout le contenu d'une feuille sera exporté sur une seule page dans le résultat. La taille du papier du paramètre pagesetup sera invalide, mais les autres paramètres de pagesetup resteront effectifs. |
| [GetAllColumnsInOnePagePerSheet](./getallcolumnsinonepagepersheet/) | Si AllColumnsInOnePagePerSheet est true, tout le contenu des colonnes d'une feuille sera exporté sur une seule page dans le résultat. La largeur du papier du paramètre pagesetup sera ignorée, mais les autres paramètres de pagesetup resteront effectifs. |
| [SetAllColumnsInOnePagePerSheet](./setallcolumnsinonepagepersheet/) | Si AllColumnsInOnePagePerSheet est true, tout le contenu des colonnes d'une feuille sera exporté sur une seule page dans le résultat. La largeur du papier du paramètre pagesetup sera ignorée, mais les autres paramètres de pagesetup resteront effectifs. |
| [GetIgnoreError](./getignoreerror/) | Indique si vous devez masquer l'erreur lors du rendu. L'erreur peut provenir d'une forme, d'une image, du rendu d'un graphique, etc. |
| [SetIgnoreError](./setignoreerror/) | Indique si vous devez masquer l'erreur lors du rendu. L'erreur peut provenir d'une forme, d'une image, du rendu d'un graphique, etc. |
| [GetOutputBlankPageWhenNothingToPrint](./getoutputblankpagewhennothingtoprint/) | Indique s'il faut générer une page blanche lorsqu'il n'y a rien à imprimer. |
| [SetOutputBlankPageWhenNothingToPrint](./setoutputblankpagewhennothingtoprint/) | Indique s'il faut générer une page blanche lorsqu'il n'y a rien à imprimer. |
| [SetPageIndex](./setpageindex/) | Obtient ou définit l'index basé sur zéro de la première page à enregistrer. |
| [GetPageIndex](./getpageindex/) | Obtient ou définit l'index basé sur zéro de la première page à enregistrer. |
| [SetPageCount](./setpagecount/) | Obtient ou définit le nombre de pages à enregistrer. |
| [GetPageCount](./getpagecount/) | Obtient ou définit le nombre de pages à enregistrer. |
| [GetPrintingPageType](./getprintingpagetype/) | Indique quelles pages ne seront pas imprimées. |
| [SetPrintingPageType](./setprintingpagetype/) | Indique quelles pages ne seront pas imprimées. |
| [GetGridlineType](./getgridlinetype/) | Obtient ou définit le type de ligne de grille. |
| [SetGridlineType](./setgridlinetype/) | Obtient ou définit le type de ligne de grille. |
| [GetGridlineColor](./getgridlinecolor/) | Obtient ou définit la couleur de la ligne de grille. |
| [SetGridlineColor](./setgridlinecolor/) | Obtient ou définit la couleur de la ligne de grille. |
| [GetTextCrossType](./gettextcrosstype/) | Obtient ou définit le type d'affichage du texte lorsque la largeur du texte dépasse celle de la cellule. |
| [SetTextCrossType](./settextcrosstype/) | Obtient ou définit le type d'affichage du texte lorsque la largeur du texte dépasse celle de la cellule. |
| [GetDefaultEditLanguage](./getdefaulteditlanguage/) | Obtient ou définit la langue d'édition par défaut. |
| [SetDefaultEditLanguage](./setdefaulteditlanguage/) | Obtient ou définit la langue d'édition par défaut. |
| [GetSheetSet](./getsheetset/) | Obtient ou définit les feuilles à rendre. La valeur par défaut est toutes les feuilles visibles du classeur : Aspose.Cells.Rendering.SheetSet.Visible. |
| [SetSheetSet](./setsheetset/) | Obtient ou définit les feuilles à rendre. La valeur par défaut est toutes les feuilles visibles du classeur : Aspose.Cells.Rendering.SheetSet.Visible. |
| [GetDrawObjectEventHandler](./getdrawobjecteventhandler/) | Implémente cette interface pour obtenir DrawObject et Bound lors du rendu. |
| [SetDrawObjectEventHandler](./setdrawobjecteventhandler/) | Implémente cette interface pour obtenir DrawObject et Bound lors du rendu. |
| [GetEmfRenderSetting](./getemfrendersetting/) | Paramètre pour le rendu du métafichier Emf. |
| [SetEmfRenderSetting](./setemfrendersetting/) | Paramètre pour le rendu du métafichier Emf. |
| [GetCustomRenderSettings](./getcustomrendersettings/) | Obtient ou définit les paramètres personnalisés pendant le rendu. |
| [SetCustomRenderSettings](./setcustomrendersettings/) | Obtient ou définit les paramètres personnalisés pendant le rendu. |
| [GetRenderingBehavior](./getrenderingbehavior/) | Obtient ou définit les comportements de rendu spécifiques à Excel à appliquer. |
| [SetRenderingBehavior](./setrenderingbehavior/) | Obtient ou définit les comportements de rendu spécifiques à Excel à appliquer. |
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
