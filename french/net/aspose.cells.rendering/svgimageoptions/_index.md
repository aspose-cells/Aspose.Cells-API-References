---
title: "Classe SvgImageOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Rendering.SvgImageOptions. Options pour générer une image Svg"
type: docs
url: /fr/net/aspose.cells.rendering/svgimageoptions/
---
## SvgImageOptions class

Options pour générer une image Svg.

```csharp
public class SvgImageOptions : ImageOrPrintOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [SvgImageOptions](svgimageoptions/)() | Constructeur. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | Si AllColumnsInOnePagePerSheet est vrai, le contenu de toutes les colonnes d’une feuille sera exporté sur une seule page dans le résultat. La largeur du format de papier du paramètre pagesetup sera invalide, mais les autres paramètres de pagesetup resteront effectifs. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [ChartImageType](../../aspose.cells.rendering/imageorprintoptions/chartimagetype/) { get; set; } | (**Obsolete.**) Indiquer le type d’image du graphique lors de la conversion. Valeur par défaut : PNG. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont/) { get; set; } | Lorsque les caractères dans le classeur Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le PDF ou l’image. Réglez ceci sur true pour essayer d’utiliser la police par défaut du classeur afin d’afficher ces caractères en premier. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CssPrefix](../../aspose.cells.rendering/svgimageoptions/cssprefix/) { get; set; } | Obtient et définit le préfixe du nom CSS dans le SVG, la valeur par défaut est une chaîne vide. |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler/) { get; set; } | Le client peut effectuer une sortie spéciale vers l’imprimante lors de l’impression de chaque page en utilisant ce gestionnaire d’événement (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler/) { get; set; } | Le client peut contrôler les paramètres de page de l’imprimante lors de l’impression de chaque page en utilisant ce gestionnaire d’événement (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CustomRenderSettings](../../aspose.cells.rendering/imageorprintoptions/customrendersettings/) { get; set; } | Obtient ou définit les paramètres personnalisés pendant le rendu. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage/) { get; set; } | Obtient ou définit la langue d’édition par défaut. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont/) { get; set; } | Lorsque les caractères dans le classeur Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le PDF ou l’image. Définissez la propriété DefaultFont, par exemple MingLiu ou MS Gothic, pour afficher ces caractères. Si cette propriété n’est pas définie, Aspose.Cells utilisera la police par défaut du système pour afficher ces caractères Unicode. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler/) { get; set; } | Implémentez cette interface pour obtenir DrawObject et Bound lors du rendu. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmbeddedFontType](../../aspose.cells.rendering/svgimageoptions/embeddedfonttype/) { get; set; } | Obtient ou définit le type de police intégré dans le SVG. |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg/) { get; set; } | (**Obsolete.**) Indiquer le nom de fichier de l’image intégrée dans le SVG. Cela doit être un chemin complet avec le répertoire, par exemple "c:\\xpsEmbedded" (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmfRenderSetting](../../aspose.cells.rendering/imageorprintoptions/emfrendersetting/) { get; set; } | Paramètre pour le rendu des métafichiers EMF dans le fichier source. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype/) { get; set; } | Obtient ou définit un EmfType qui spécifie le format du métafile. La valeur par défaut est EmfPlusDual. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [FitToViewPort](../../aspose.cells.rendering/svgimageoptions/fittoviewport/) { get; set; } | Si cette propriété est vraie, le SVG généré s’ajustera à la zone d’affichage. |
| [GridlineColor](../../aspose.cells.rendering/imageorprintoptions/gridlinecolor/) { get; set; } | Obtient ou définit la couleur de la ligne de grille. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype/) { get; set; } | Obtient ou définit le type de ligne de grille. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution/) { get; set; } | Obtient ou définit la résolution horizontale des images générées, en points par pouce. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| override [ImageType](../../aspose.cells.rendering/svgimageoptions/imagetype/) { get; set; } | Obtient ou définit le format des images générées. Valeur par défaut : PNG. |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit/) { get; set; } | (**Obsolete.**) Indique si la largeur et la hauteur des cellules sont automatiquement ajustées en fonction de la valeur de la cellule. La valeur par défaut est false. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | Indique s’il faut uniquement substituer la police du caractère lorsque la police de la cellule n’est pas compatible. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized/) { get; set; } | Indique s’il faut optimiser les éléments de sortie. (Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet/) { get; set; } | Si OnePagePerSheet est vrai, tout le contenu d'une feuille sera exporté sur une seule page dans le résultat. La taille du papier du paramètre pagesetup sera invalide, et les autres paramètres de pagesetup resteront effectifs.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea/) { get; set; } | Si cette propriété est vraie, une zone sera exportée, et aucune échelle ne sera appliquée.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | Indique s'il faut exporter une page blanche lorsqu'il n'y a rien à imprimer.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount/) { get; set; } | Obtient ou définit le nombre de pages à enregistrer.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex/) { get; set; } | Obtient ou définit l'index basé sur zéro de la première page à enregistrer.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback/) { get; set; } | Contrôle/Indique la progression du processus d'enregistrement des pages.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat/) { get; set; } | Obtient ou définit le format de pixel pour les images générées.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage/) { get; set; } | Indique quelles pages ne seront pas imprimées.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog/) { get; set; } | Si PrintWithStatusDialog = true, une boîte de dialogue affichant l'état d'impression actuel sera présentée. Sinon aucune boîte de dialogue ne sera affichée.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality/) { get; set; } | Obtient ou définit une valeur déterminant la qualité des images générées à appliquer uniquement lors de l'enregistrement des pages au format `Jpeg`. La valeur par défaut est 100(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat/) { get; set; } | (**Obsolete.**) Obtient ou définit le type de format de fichier de sortie. Prise en charge Tiff/XPS(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SheetSet](../../aspose.cells.rendering/imageorprintoptions/sheetset/) { get; set; } | Obtient ou définit les feuilles à rendre. La valeur par défaut est toutes les feuilles visibles du classeur : [`Visible`](../sheetset/visible/).(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode/) { get; set; } | Spécifie si le lissage (antialiasing) est appliqué aux lignes, aux courbes et aux bords des zones remplies. La valeur par défaut est SmoothingMode.None(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SvgCssPrefix](../../aspose.cells.rendering/imageorprintoptions/svgcssprefix/) { get; set; } | (**Obsolete.**) Obtient et définit le préfixe du nom css dans le svg, la valeur par défaut est une chaîne vide.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport/) { get; set; } | (**Obsolete.**) si cette propriété est vraie, le svg généré s'adaptera à la fenêtre d'affichage.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype/) { get; set; } | Obtient ou définit le type d'affichage du texte lorsque la largeur du texte dépasse la largeur de la cellule.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint/) { get; set; } | Spécifie la qualité du rendu du texte. La valeur par défaut est TextRenderingHint.SystemDefault(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffBinarizationMethod](../../aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/) { get; set; } | Obtient ou définit la méthode utilisée lors de la conversion des images au format 1 bpp lorsque [`ImageType`](../imageorprintoptions/imagetype/) est Tiff et que [`TiffCompression`](../imageorprintoptions/tiffcompression/) est égal à Ccitt3 ou Ccitt4.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth/) { get; set; } | Obtient ou définit la profondeur de bits à appliquer uniquement lors de l'enregistrement des pages au format `Tiff`.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression/) { get; set; } | Obtient ou définit le type de compression à appliquer uniquement lors de l'enregistrement des pages au format `Tiff`.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent/) { get; set; } | Indique si l'arrière-plan de l'image générée doit être transparent.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution/) { get; set; } | Obtient ou définit la résolution verticale pour les images générées, en points par pouce.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback/) { get; set; } | Obtient ou définit le rappel d'avertissement.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/)(int, int) | (**Obsolete.**) Définit la largeur et la hauteur souhaitées de l'image.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/)(int, int, bool) | Définit la largeur et la hauteur souhaitées de l'image.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassSvgImageOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Remplir des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Q1");
            worksheet.Cells["A2"].PutValue(12000);
            worksheet.Cells["A3"].PutValue(16500);
            worksheet.Cells["B1"].PutValue("Q2");
            worksheet.Cells["B2"].PutValue(25500);
            worksheet.Cells["B3"].PutValue(10800);

            // Créer un graphique à colonnes
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A2:B3", true);
            chart.NSeries.CategoryData = "A1:B1";

            // Initialiser les options d'image SVG
            SvgImageOptions svgOptions = new SvgImageOptions();
            
            // Configurer les options de rendu SVG
            svgOptions.FitToViewPort = true;
            svgOptions.CssPrefix = "chart-";
            svgOptions.EmbeddedFontType = SvgEmbeddedFontType.Woff;
            svgOptions.ImageType = ImageType.Svg;

            // Définir la qualité d'impression et la résolution
            svgOptions.PrintWithStatusDialog = true;
            svgOptions.HorizontalResolution = 300;
            svgOptions.VerticalResolution = 300;

            // Rendre le graphique en SVG avec les options configurées
            chart.ToImage("chart_output.svg", svgOptions);

            // Démontrer l'intégration de l'enregistrement du classeur
            workbook.Save("SvgRenderingDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ImageOrPrintOptions](../imageorprintoptions/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


