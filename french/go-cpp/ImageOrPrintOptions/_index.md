---
title: "Classe ImageOrPrintOptions"
linktitle: "ImageOrPrintOptions"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "ImageOrPrintOptions classe. Encapsule l'objet qui représente imageorprintoptions en Go."
type: docs
weight: 200
url: /fr/go-cpp/imageorprintoptions/
---

## ImageOrPrintOptions class

Permet de spécifier des options lors du rendu d'une feuille de calcul en images, de l'impression de la feuille de calcul ou du rendu d'un graphique en image.

```go

type ImageOrPrintOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewImageOrPrintOptions](./newimageorprintoptions/) | Constructeur. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [SetPrintWithStatusDialog](./setprintwithstatusdialog/) | Si PrintWithStatusDialog = true, une boîte de dialogue affichant l'état d'impression actuel sera affichée ; sinon aucune boîte de dialogue ne sera affichée. |
| [GetPrintWithStatusDialog](./getprintwithstatusdialog/) | Si PrintWithStatusDialog = true, une boîte de dialogue affichant l'état d'impression actuel sera affichée ; sinon aucune boîte de dialogue ne sera affichée. |
| [GetHorizontalResolution](./gethorizontalresolution/) | Obtient ou définit la résolution horizontale des images générées, en points par pouce. |
| [SetHorizontalResolution](./sethorizontalresolution/) | Obtient ou définit la résolution horizontale des images générées, en points par pouce. |
| [GetVerticalResolution](./getverticalresolution/) | Obtient ou définit la résolution verticale des images générées, en points par pouce. |
| [SetVerticalResolution](./setverticalresolution/) | Obtient ou définit la résolution verticale des images générées, en points par pouce. |
| [GetTiffCompression](./gettiffcompression/) | Obtient ou définit le type de compression à appliquer uniquement lors de l'enregistrement des pages au format <c>Tiff</c>. |
| [SetTiffCompression](./settiffcompression/) | Obtient ou définit le type de compression à appliquer uniquement lors de l'enregistrement des pages au format <c>Tiff</c>. |
| [GetTiffColorDepth](./gettiffcolordepth/) | Obtient ou définit la profondeur de bits à appliquer uniquement lors de l'enregistrement des pages au format <c>Tiff</c>. |
| [SetTiffColorDepth](./settiffcolordepth/) | Obtient ou définit la profondeur de bits à appliquer uniquement lors de l'enregistrement des pages au format <c>Tiff</c>. |
| [GetTiffBinarizationMethod](./gettiffbinarizationmethod/) | Obtient ou définit la méthode utilisée lors de la conversion des images au format 1 bpp lorsque ImageType est Tiff et que TiffCompression est égal à Ccitt3 ou Ccitt4. |
| [SetTiffBinarizationMethod](./settiffbinarizationmethod/) | Obtient ou définit la méthode utilisée lors de la conversion des images au format 1 bpp lorsque ImageType est Tiff et que TiffCompression est égal à Ccitt3 ou Ccitt4. |
| [GetPrintingPage](./getprintingpage/) | Indique quelles pages ne seront pas imprimées. |
| [SetPrintingPage](./setprintingpage/) | Indique quelles pages ne seront pas imprimées. |
| [GetQuality](./getquality/) | Obtient ou définit une valeur déterminant la qualité des images générées à appliquer uniquement lors de l'enregistrement des pages au format <c>Jpeg</c>. La valeur par défaut est 100. |
| [SetQuality](./setquality/) | Obtient ou définit une valeur déterminant la qualité des images générées à appliquer uniquement lors de l'enregistrement des pages au format <c>Jpeg</c>. La valeur par défaut est 100. |
| [GetOnePagePerSheet](./getonepagepersheet/) | Si OnePagePerSheet est true, tout le contenu d'une feuille sera exporté sur une seule page dans le résultat. La taille du papier du paramètre pagesetup sera invalide, mais les autres paramètres de pagesetup resteront effectifs. |
| [SetOnePagePerSheet](./setonepagepersheet/) | Si OnePagePerSheet est true, tout le contenu d'une feuille sera exporté sur une seule page dans le résultat. La taille du papier du paramètre pagesetup sera invalide, mais les autres paramètres de pagesetup resteront effectifs. |
| [GetAllColumnsInOnePagePerSheet](./getallcolumnsinonepagepersheet/) | Si AllColumnsInOnePagePerSheet est vrai, le contenu de toutes les colonnes d'une feuille sera exporté sur une seule page dans le résultat. La largeur du format de papier du paramètre pagesetup sera invalide, mais les autres paramètres de pagesetup resteront effectifs. |
| [SetAllColumnsInOnePagePerSheet](./setallcolumnsinonepagepersheet/) | Si AllColumnsInOnePagePerSheet est vrai, le contenu de toutes les colonnes d'une feuille sera exporté sur une seule page dans le résultat. La largeur du format de papier du paramètre pagesetup sera invalide, mais les autres paramètres de pagesetup resteront effectifs. |
| [GetDrawObjectEventHandler](./getdrawobjecteventhandler/) | Implémente cette interface pour obtenir DrawObject et Bound lors du rendu. |
| [SetDrawObjectEventHandler](./setdrawobjecteventhandler/) | Implémente cette interface pour obtenir DrawObject et Bound lors du rendu. |
| [GetOnlyArea](./getonlyarea/) | Si cette propriété est vraie, une zone sera générée, et aucune échelle ne sera appliquée. |
| [SetOnlyArea](./setonlyarea/) | Si cette propriété est vraie, une zone sera générée, et aucune échelle ne sera appliquée. |
| [GetTransparent](./gettransparent/) | Indique si l'arrière-plan de l'image générée doit être transparent. |
| [SetTransparent](./settransparent/) | Indique si l'arrière-plan de l'image générée doit être transparent. |
| [SetIsFontSubstitutionCharGranularity](./setisfontsubstitutionchargranularity/) | Indique s'il faut uniquement substituer la police du caractère lorsque la police de la cellule n'est pas compatible. |
| [IsFontSubstitutionCharGranularity](./isfontsubstitutionchargranularity/) | Indique s'il faut uniquement substituer la police du caractère lorsque la police de la cellule n'est pas compatible. |
| [SetPageIndex](./setpageindex/) | Obtient ou définit l'index basé sur zéro de la première page à enregistrer. |
| [GetPageIndex](./getpageindex/) | Obtient ou définit l'index basé sur zéro de la première page à enregistrer. |
| [SetPageCount](./setpagecount/) | Obtient ou définit le nombre de pages à enregistrer. |
| [GetPageCount](./getpagecount/) | Obtient ou définit le nombre de pages à enregistrer. |
| [SetDesiredSize](./setdesiredsize/) | Définit la largeur et la hauteur souhaitées de l'image. |
| [IsOptimized](./isoptimized/) | Indique s'il faut optimiser les éléments de sortie. |
| [SetIsOptimized](./setisoptimized/) | Indique s'il faut optimiser les éléments de sortie. |
| [GetDefaultFont](./getdefaultfont/) | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le PDF ou l'image. Définissez la propriété DefaultFont, par exemple MingLiu ou MS Gothic, pour afficher ces caractères. Si cette propriété n'est pas définie, Aspose.Cells utilisera la police système par défaut pour afficher ces caractères Unicode. |
| [SetDefaultFont](./setdefaultfont/) | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le PDF ou l'image. Définissez la propriété DefaultFont, par exemple MingLiu ou MS Gothic, pour afficher ces caractères. Si cette propriété n'est pas définie, Aspose.Cells utilisera la police système par défaut pour afficher ces caractères Unicode. |
| [GetCheckWorkbookDefaultFont](./getcheckworkbookdefaultfont/) | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le PDF ou l'image. Réglez cette propriété sur true pour essayer d'utiliser d'abord la police par défaut du classeur afin d'afficher ces caractères. |
| [SetCheckWorkbookDefaultFont](./setcheckworkbookdefaultfont/) | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le PDF ou l'image. Réglez cette propriété sur true pour essayer d'utiliser d'abord la police par défaut du classeur afin d'afficher ces caractères. |
| [GetOutputBlankPageWhenNothingToPrint](./getoutputblankpagewhennothingtoprint/) | Indique s'il faut générer une page blanche lorsqu'il n'y a rien à imprimer. |
| [SetOutputBlankPageWhenNothingToPrint](./setoutputblankpagewhennothingtoprint/) | Indique s'il faut générer une page blanche lorsqu'il n'y a rien à imprimer. |
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
| [GetEmfRenderSetting](./getemfrendersetting/) | Paramètre pour le rendu des métafichiers Emf dans le fichier source. |
| [SetEmfRenderSetting](./setemfrendersetting/) | Paramètre pour le rendu des métafichiers Emf dans le fichier source. |
| [GetCustomRenderSettings](./getcustomrendersettings/) | Obtient ou définit les paramètres personnalisés pendant le rendu. |
| [SetCustomRenderSettings](./setcustomrendersettings/) | Obtient ou définit les paramètres personnalisés pendant le rendu. |
| [GetImageType](./getimagetype/) | Obtient ou définit le format des images générées. Valeur par défaut : PNG. |
| [SetImageType](./setimagetype/) | Obtient ou définit le format des images générées. Valeur par défaut : PNG. |
