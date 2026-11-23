---
title: "Classe ImageOrPrintOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Rendering.ImageOrPrintOptions. Permet de spécifier des options lors du rendu d'une feuille de calcul en images, de l'impression de la feuille ou du rendu d'un graphique en image"
type: docs
url: /fr/net/aspose.cells.rendering/imageorprintoptions/
---
## ImageOrPrintOptions class

Permet de spécifier des options lors du rendu d'une feuille de calcul en images, de l'impression d'une feuille de calcul ou du rendu d'un graphique en image.

```csharp
public class ImageOrPrintOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ImageOrPrintOptions](imageorprintoptions/)() | Constructeur. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | Si AllColumnsInOnePagePerSheet est vrai, tout le contenu des colonnes d'une feuille sera exporté sur une seule page dans le résultat. La largeur du format de papier du paramètre pagesetup sera invalide, et les autres paramètres de pagesetup resteront effectifs. |
| [ChartImageType](../../aspose.cells.rendering/imageorprintoptions/chartimagetype/) { get; set; } | (**Obsolete.**) Indique le type d'image du graphique lors de la conversion. Valeur par défaut : PNG. |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont/) { get; set; } | Lorsque les caractères dans le fichier Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le PDF, l'image. Réglez ceci sur true pour essayer d'utiliser la police par défaut du classeur afin d'afficher ces caractères en premier. |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler/) { get; set; } | Le client peut effectuer une sortie spéciale vers l'imprimante lors de l'impression de chaque page en utilisant cet EventHandler |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler/) { get; set; } | Le client peut contrôler les paramètres de page de l'imprimante lors de l'impression de chaque page en utilisant cet EventHandler |
| [CustomRenderSettings](../../aspose.cells.rendering/imageorprintoptions/customrendersettings/) { get; set; } | Obtient ou définit les paramètres personnalisés pendant le rendu. |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage/) { get; set; } | Obtient ou définit la langue d'édition par défaut. |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont/) { get; set; } | Lorsque les caractères dans le fichier Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le PDF, l'image. Définissez la propriété DefaultFont, par exemple MingLiu ou MS Gothic, pour afficher ces caractères. Si cette propriété n'est pas définie, Aspose.Cells utilisera la police par défaut du système pour afficher ces caractères Unicode. |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler/) { get; set; } | Implémentez cette interface pour obtenir DrawObject et Bound lors du rendu. |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg/) { get; set; } | (**Obsolete.**) Indique le nom de fichier de l'image intégrée dans le SVG. Il doit s'agir d'un chemin complet avec répertoire, par exemple "c:\\xpsEmbedded" |
| [EmfRenderSetting](../../aspose.cells.rendering/imageorprintoptions/emfrendersetting/) { get; set; } | Paramètre pour le rendu des métafichiers Emf dans le fichier source. |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype/) { get; set; } | Obtient ou définit un EmfType qui spécifie le format du Metafile. La valeur par défaut est EmfPlusDual. |
| [GridlineColor](../../aspose.cells.rendering/imageorprintoptions/gridlinecolor/) { get; set; } | Obtient ou définit la couleur de la ligne de grille. |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype/) { get; set; } | Obtient ou définit le type de ligne de grille. |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution/) { get; set; } | Obtient ou définit la résolution horizontale des images générées, en points par pouce. |
| virtual [ImageType](../../aspose.cells.rendering/imageorprintoptions/imagetype/) { get; set; } | Obtient ou définit le format des images générées. Valeur par défaut : PNG. |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit/) { get; set; } | (**Obsolete.**) Indique si la largeur et la hauteur des cellules sont automatiquement ajustées en fonction de la valeur de la cellule. La valeur par défaut est false. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | Indique s'il faut uniquement substituer la police du caractère lorsque la police de la cellule n'est pas compatible. |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized/) { get; set; } | Indique s'il faut optimiser les éléments de sortie. |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet/) { get; set; } | Si OnePagePerSheet est vrai, tout le contenu d'une feuille sera exporté sur une seule page dans le résultat. Le format de papier du pagesetup sera invalide, et les autres paramètres du pagesetup resteront effectifs. |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea/) { get; set; } | Si cette propriété est vraie, une zone sera exportée et aucune échelle ne sera appliquée. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | Indique s'il faut générer une page blanche lorsqu'il n'y a rien à imprimer. |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount/) { get; set; } | Obtient ou définit le nombre de pages à enregistrer. |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex/) { get; set; } | Obtient ou définit l'index basé sur zéro de la première page à enregistrer. |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback/) { get; set; } | Contrôler/Indiquer la progression du processus d'enregistrement de la page. |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat/) { get; set; } | Obtient ou définit le format de pixel des images générées. |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage/) { get; set; } | Indique quelles pages ne seront pas imprimées. |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog/) { get; set; } | Si PrintWithStatusDialog = true, une boîte de dialogue affichant l'état d'impression actuel sera affichée. Sinon, aucune boîte de dialogue ne sera affichée. |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality/) { get; set; } | Obtient ou définit une valeur déterminant la qualité des images générées à appliquer uniquement lors de l'enregistrement des pages au format `Jpeg`. La valeur par défaut est 100 |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat/) { get; set; } | (**Obsolete.**) Obtient ou définit le type de format de fichier de sortie. Prise en charge Tiff/XPS |
| [SheetSet](../../aspose.cells.rendering/imageorprintoptions/sheetset/) { get; set; } | Obtient ou définit les feuilles à rendre. La valeur par défaut est toutes les feuilles visibles du classeur : [`Visible`](../sheetset/visible/). |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode/) { get; set; } | Spécifie si le lissage (antialiasing) est appliqué aux lignes et courbes ainsi qu'aux bords des zones remplies. La valeur par défaut est SmoothingMode.None |
| [SvgCssPrefix](../../aspose.cells.rendering/imageorprintoptions/svgcssprefix/) { get; set; } | (**Obsolete.**) Obtient et définit le préfixe du nom css dans svg, la valeur par défaut est une chaîne vide. |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport/) { get; set; } | (**Obsolete.**) si cette propriété est vraie, le svg généré s'adaptera à la zone d'affichage. |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype/) { get; set; } | Obtient ou définit le type d'affichage du texte lorsque la largeur du texte dépasse la largeur de la cellule. |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint/) { get; set; } | Spécifie la qualité du rendu du texte. La valeur par défaut est TextRenderingHint.SystemDefault |
| [TiffBinarizationMethod](../../aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/) { get; set; } | Obtient ou définit la méthode utilisée lors de la conversion d'images au format 1 bpp lorsque [`ImageType`](./imagetype/) est Tiff et que [`TiffCompression`](./tiffcompression/) est égal à Ccitt3 ou Ccitt4. |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth/) { get; set; } | Obtient ou définit la profondeur de bits à appliquer uniquement lors de l'enregistrement des pages au format `Tiff`. |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression/) { get; set; } | Obtient ou définit le type de compression à appliquer uniquement lors de l'enregistrement des pages au format `Tiff`. |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent/) { get; set; } | Indique si l'arrière-plan de l'image générée doit être transparent. |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution/) { get; set; } | Obtient ou définit la résolution verticale des images générées, en points par pouce. |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback/) { get; set; } | Obtient ou définit le rappel d'avertissement. |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/#setdesiredsize)(int, int) | (**Obsolete.**) Définit la largeur et la hauteur souhaitées de l'image. |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/#setdesiredsize_1)(int, int, bool) | Définit la largeur et la hauteur souhaitées de l'image. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class RenderingClassImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Créez ImageOrPrintOptions et définissez les propriétés
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;

            // Créez un nouveau classeur avec des données d'exemple et un graphique
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Enregistrez le graphique en tant qu'image en utilisant les options
            chart.ToImage("output_chart.png", options);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


