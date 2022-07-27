---
title: ImageOrPrintOptions
second_title: Référence de l'API Aspose.Cells pour .NET
description: Permet de spécifier des options lors du rendu de la feuille de calcul en images de limpression de la feuille de calcul ou du rendu du graphique en image.
type: docs
weight: 5140
url: /fr/net/aspose.cells.rendering/imageorprintoptions/
---
## ImageOrPrintOptions class

Permet de spécifier des options lors du rendu de la feuille de calcul en images, de l'impression de la feuille de calcul ou du rendu du graphique en image.

```csharp
public class ImageOrPrintOptions
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [ImageOrPrintOptions](imageorprintoptions)() | Default_Constructor |

## Propriétés

| Nom | La description |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet) { get; set; } | Si AllColumnsInOnePagePerSheet est true , tout le contenu de la colonne d'une feuille sortira sur une seule page de résultat. La largeur de la taille du papier de pagesetup sera invalide, et les autres paramètres de pagesetup prendront toujours effet. |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont) { get; set; } | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, Ils peuvent apparaître sous forme de bloc dans pdf,image. Définissez ceci sur true pour essayer d'utiliser la police par défaut du classeur pour afficher ces caractères en premier. |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler) { get; set; } | Le client peut imprimer une sortie spéciale sur l'imprimante lors de l'impression de chaque page à l'aide de cet EventHandler |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler) { get; set; } | Le client peut contrôler la mise en page de l'imprimante lors de l'impression de chaque page à l'aide de cet EventHandler |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage) { get; set; } | Obtient ou définit la langue d'édition par défaut. |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont) { get; set; } | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, Ils peuvent apparaître sous forme de bloc dans pdf,image. Définissez la police par défaut telle que MingLiu ou MS Gothic pour afficher ces caractères. Si cette propriété est non défini, Aspose.Cells utilisera la police par défaut du système pour afficher ces caractères Unicode. |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler) { get; set; } | Implémente cette interface pour obtenir DrawObject et Bound lors du rendu. |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg) { get; set; } | Indiquez le nom du fichier de l'image intégrée en svg. Il doit s'agir d'un chemin d'accès complet avec un répertoire tel que "c:\\xpsEmbedded" |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype) { get; set; } | Obtient ou définit un EmfType qui spécifie le format du métafichier.. La valeur par défaut est EmfPlusDual. |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype) { get; set; } | Obtient ou définit le type de quadrillage. |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution) { get; set; } | Obtient ou définit la résolution horizontale des images générées, en points par pouce. Applique la méthode de génération d'image à l'exception des images au format Emf. |
| [ImageType](../../aspose.cells.rendering/imageorprintoptions/imagetype) { get; set; } | Obtient ou définit le format des images générées. valeur par défaut : PNG. |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit) { get; set; } | Indique si la largeur et la hauteur des cellules sont automatiquement ajustées par valeur de cellule. La valeur par défaut est false. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity) { get; set; } | Indique s'il faut uniquement remplacer la police de caractère lorsque la police de cellule n'est pas compatible avec celle-ci. |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized) { get; set; } | Indique s'il faut optimiser les éléments de sortie. |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet) { get; set; } | Si OnePagePerSheet est true , tout le contenu d'une feuille sortira sur une seule page de résultat. Le format de papier de pagesetup ne sera pas valide et les autres paramètres de pagesetup prendront toujours effet. |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea) { get; set; } | Si cette propriété est true , une zone sera sortie et aucune échelle ne prendra effet. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint) { get; set; } | Indique s'il faut imprimer une page vierge lorsqu'il n'y a rien à imprimer. |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount) { get; set; } | Obtient ou définit le nombre de pages à enregistrer. |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex) { get; set; } | Obtient ou définit l'index de base 0 de la première page à enregistrer. |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback) { get; set; } | Contrôler/Indiquer la progression du processus d'enregistrement de la page. |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat) { get; set; } | Obtient ou définit le format de pixel pour les images générées. |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage) { get; set; } | Indique quelles pages ne seront pas imprimées. |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog) { get; set; } | Si PrintWithStatusDialog = true , une boîte de dialogue affiche l'état d'impression actuel. sinon aucune boîte de dialogue de ce type ne s'affichera. |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality) { get; set; } | Obtient ou définit une valeur déterminant la qualité des images générées à appliquer uniquement lors de l'enregistrement de pages dans le`JPEG` format. La valeur par défaut est 100 |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat) { get; set; } | Obtient ou définit le type de format de fichier de sortie Prend en charge Tiff/XPS |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode) { get; set; } | Spécifie si le lissage (anticrénelage) est appliqué aux lignes et aux courbes et aux bords des zones remplies. La valeur par défaut est SmoothingMode.None |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport) { get; set; } | si cette propriété est vraie, le svg généré s'adaptera au port d'affichage. |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype) { get; set; } | Obtient ou définit l'affichage du type de texte lorsque la largeur du texte est supérieure à la largeur de la cellule. |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint) { get; set; } | Spécifie la qualité du rendu du texte. La valeur par défaut est TextRenderingHint.SystemDefault |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth) { get; set; } | Obtient ou définit la profondeur de bits à appliquer uniquement lors de l'enregistrement de pages sur le`Tif` format. |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression) { get; set; } | Obtient ou définit le type de compression à appliquer uniquement lors de l'enregistrement de pages dans le`Tif` format. |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent) { get; set; } | Indique si le fond de l'image générée doit être transparent. |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution) { get; set; } | Obtient ou définit la résolution verticale des images générées, en points par pouce. Applique la méthode de génération d'image à l'exception de l'image au format Emf. |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback) { get; set; } | Obtient ou définit un rappel d'avertissement. |

## Méthodes

| Nom | La description |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize)(int, int) | Définit la largeur et la hauteur souhaitées de l'image. |

### Exemples

```csharp

[C#]

//Définir les options d'image ou d'impression
ImageOrPrintOptions options = new ImageOrPrintOptions();

//Définir le format de l'image de sortie
options.ImageType = ImageType.Png;

//Définir la résolution horizontale
options.HorizontalResolution = 300;

//Définir la résolution verticale
options.VerticalResolution = 300;

//Instancier le classeur
Workbook book = new Workbook("test.xls");

// Enregistrer le graphique en tant qu'image à l'aide des options ImageOrPrint
book.Worksheets[0].Charts[0].ToImage("chart.png", options);

[VB.NET]

'Définir les options d'image ou d'impression
Dim options As New ImageOrPrintOptions()

'Définir le format de l'image de sortie
options.ImageType = ImageType.Png

'Définir la résolution horizontale
options.HorizontalResolution = 300

'Définir la résolution verticale
options.VerticalResolution = 300

'Instancier le classeur
Dim book As New Workbook("test.xls")

'Enregistrer le graphique en tant qu'image à l'aide des options ImageOrPrint
book.Worksheets(0).Charts(0).ToImage("chart.png", options)
```

### Voir également

* espace de noms [Aspose.Cells.Rendering](../../aspose.cells.rendering)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
