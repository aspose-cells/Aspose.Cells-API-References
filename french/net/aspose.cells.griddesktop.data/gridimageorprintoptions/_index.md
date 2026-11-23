---
title: "Classe GridImageOrPrintOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridDesktop.Data.GridImageOrPrintOptions. Permet de spécifier des options lors du rendu d'une feuille de calcul en images, de l'impression de la feuille de calcul ou du rendu d'un graphique en image"
type: docs
url: /fr/net/aspose.cells.griddesktop.data/gridimageorprintoptions/
---
## GridImageOrPrintOptions class

Permet de spécifier des options lors du rendu d'une feuille de calcul en images, de l'impression d'une feuille de calcul ou du rendu d'un graphique en image.

```csharp
public class GridImageOrPrintOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [GridImageOrPrintOptions](gridimageorprintoptions/)() | Le constructeur de GridImageOrPrintOptions |

## Propriétés

| Nom | Description |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | Si AllColumnsInOnePagePerSheet est vrai, tout le contenu des colonnes d'une feuille sera exporté sur une seule page dans le résultat. La largeur du format de papier du paramètre pagesetup sera invalide, et les autres paramètres de pagesetup resteront effectifs. |
| [CheckWorkbookDefaultFont](../../aspose.cells.griddesktop.data/gridimageorprintoptions/checkworkbookdefaultfont/) { get; set; } | Lorsque les caractères dans le fichier Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le PDF, l'image. Réglez ceci sur true pour essayer d'utiliser la police par défaut du classeur afin d'afficher ces caractères en premier. |
| [DefaultFont](../../aspose.cells.griddesktop.data/gridimageorprintoptions/defaultfont/) { get; set; } | Lorsque les caractères dans le fichier Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le PDF, l'image. Définissez la propriété DefaultFont, par exemple MingLiu ou MS Gothic, pour afficher ces caractères. Si cette propriété n'est pas définie, Aspose.Cells utilisera la police par défaut du système pour afficher ces caractères Unicode. |
| [EmbededImageNameInSvg](../../aspose.cells.griddesktop.data/gridimageorprintoptions/embededimagenameinsvg/) { get; set; } | Indique le nom de fichier de l'image intégrée dans le SVG. Cela doit être le chemin complet avec le répertoire, par exemple "c:\\xpsEmbedded" |
| [EmfType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/emftype/) { get; set; } | Obtient ou définit un EmfType qui spécifie le format du Metafile. La valeur par défaut est EmfPlusDual. |
| [GridlineType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/gridlinetype/) { get; set; } | Obtient ou définit le type de ligne de grille. |
| [HorizontalResolution](../../aspose.cells.griddesktop.data/gridimageorprintoptions/horizontalresolution/) { get; set; } | Obtient ou définit la résolution horizontale des images générées, en points par pouce. S'applique à la méthode de génération d'images sauf pour les images au format EMF. |
| [ImageType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/imagetype/) { get; set; } | Obtient ou définit le format des images générées. Valeur par défaut : PNG. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.griddesktop.data/gridimageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | Indique s'il faut uniquement substituer la police du caractère lorsque la police de la cellule n'est pas compatible. |
| [IsOptimized](../../aspose.cells.griddesktop.data/gridimageorprintoptions/isoptimized/) { get; set; } | Indique s'il faut optimiser les éléments de sortie. |
| [OnePagePerSheet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/onepagepersheet/) { get; set; } | Si OnePagePerSheet est vrai, tout le contenu d'une feuille sera exporté sur une seule page dans le résultat. Le format de papier du pagesetup sera invalide, et les autres paramètres du pagesetup resteront effectifs. |
| [OnlyArea](../../aspose.cells.griddesktop.data/gridimageorprintoptions/onlyarea/) { get; set; } | Si cette propriété est vraie, une zone sera exportée et aucune échelle ne sera appliquée. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.griddesktop.data/gridimageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | Indique s'il faut générer une page blanche lorsqu'il n'y a rien à imprimer. |
| [PageCount](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pagecount/) { get; set; } | Obtient ou définit le nombre de pages à enregistrer. |
| [PageIndex](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pageindex/) { get; set; } | Obtient ou définit l'index basé sur zéro de la première page à enregistrer. |
| [PixelFormat](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pixelformat/) { get; set; } | Obtient ou définit le format de pixel des images générées. |
| [PrintingPage](../../aspose.cells.griddesktop.data/gridimageorprintoptions/printingpage/) { get; set; } | Indique quelles pages ne seront pas imprimées. |
| [PrintWithStatusDialog](../../aspose.cells.griddesktop.data/gridimageorprintoptions/printwithstatusdialog/) { get; set; } | Si PrintWithStatusDialog = true, une boîte de dialogue affichant l'état d'impression actuel sera affichée. Sinon, aucune boîte de dialogue ne sera affichée. |
| [Quality](../../aspose.cells.griddesktop.data/gridimageorprintoptions/quality/) { get; set; } | Obtient ou définit une valeur déterminant la qualité des images générées à appliquer uniquement lors de l'enregistrement des pages au format `Jpeg`. La valeur par défaut est 100 |
| [SmoothingMode](../../aspose.cells.griddesktop.data/gridimageorprintoptions/smoothingmode/) { get; set; } | Spécifie si le lissage (antialiasing) est appliqué aux lignes et courbes ainsi qu'aux bords des zones remplies. La valeur par défaut est SmoothingMode.None |
| [SVGFitToViewPort](../../aspose.cells.griddesktop.data/gridimageorprintoptions/svgfittoviewport/) { get; set; } | Si cette propriété est vraie, le SVG généré s’ajustera à la zone d’affichage. |
| [TextCrossType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/textcrosstype/) { get; set; } | Obtient ou définit le type d'affichage du texte lorsque la largeur du texte dépasse la largeur de la cellule. |
| [TextRenderingHint](../../aspose.cells.griddesktop.data/gridimageorprintoptions/textrenderinghint/) { get; set; } | Spécifie la qualité du rendu du texte. La valeur par défaut est TextRenderingHint.SystemDefault |
| [Transparent](../../aspose.cells.griddesktop.data/gridimageorprintoptions/transparent/) { get; set; } | Indique si l'arrière-plan de l'image générée doit être transparent. |
| [VerticalResolution](../../aspose.cells.griddesktop.data/gridimageorprintoptions/verticalresolution/) { get; set; } | Obtient ou définit la résolution verticale des images générées, en points par pouce. S'applique à la méthode de génération d'images sauf pour les images au format EMF. |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.griddesktop.data/gridimageorprintoptions/setdesiredsize/)(int, int) | Définit la largeur et la hauteur souhaitées de l'image. |
| [setRenderSheetSet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/setrendersheetset/)(int[]) | définit les feuilles à rendre. Par défaut, toutes les feuilles visibles du classeur. Indexes des feuilles basés sur zéro. |

### Voir aussi

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


