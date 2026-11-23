---
title: "Classe PdfSaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.PdfSaveOptions. Représente les options pour enregistrer un fichier pdf"
type: docs
url: /fr/net/aspose.cells/pdfsaveoptions/
---
## PdfSaveOptions class

Représente les options d'enregistrement d'un fichier PDF.

```csharp
public class PdfSaveOptions : PaginatedSaveOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions/)() | Crée les options pour enregistrer le fichier pdf. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/) { get; set; } | Si AllColumnsInOnePagePerSheet est vrai, tout le contenu des colonnes d’une feuille sera exporté sur une seule page dans le résultat. La largeur du format de papier du paramètre pagesetup sera ignorée, et les autres paramètres de pagesetup resteront effectifs. (Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [Bookmark](../../aspose.cells/pdfsaveoptions/bookmark/) { get; set; } | Obtient et définit l'objet [`PdfBookmarkEntry`](../../aspose.cells.rendering/pdfbookmarkentry/). |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Le dossier pour les fichiers temporaires qui peuvent être utilisés comme cache de données.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [CalculateFormula](../../aspose.cells/pdfsaveoptions/calculateformula/) { get; set; } | Indique s'il faut calculer les formules avant d'enregistrer le fichier pdf. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Indique s’il faut vérifier les restrictions du fichier Excel lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n’autorise pas la saisie d’une chaîne de caractères supérieure à 32 K. Si vous saisissez une valeur supérieure à 32 K, elle sera tronquée.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [CheckFontCompatibility](../../aspose.cells/paginatedsaveoptions/checkfontcompatibility/) { get; set; } | Indique s’il faut vérifier la compatibilité des polices pour chaque caractère du texte. (Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [CheckWorkbookDefaultFont](../../aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/) { get; set; } | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le PDF, l’image. Réglez ceci sur true pour essayer d’utiliser d’abord la police par défaut du classeur afin d’afficher ces caractères. (Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Rendre le classeur vide après l’enregistrement du fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [Compliance](../../aspose.cells/pdfsaveoptions/compliance/) { get; set; } | Obtient ou définit le niveau de conformité aux normes PDF pour les documents de sortie. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Si vrai et que le répertoire n’existe pas, le répertoire sera créé automatiquement avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [CreatedTime](../../aspose.cells/pdfsaveoptions/createdtime/) { get; set; } | Obtient et définit l'heure de génération du document pdf. |
| [CustomPropertiesExport](../../aspose.cells/pdfsaveoptions/custompropertiesexport/) { get; set; } | Obtient ou définit une valeur déterminant la façon dont [`CustomDocumentPropertyCollection`](../../aspose.cells.properties/customdocumentpropertycollection/) sont exportées vers le fichier PDF. La valeur par défaut est None. |
| [CustomRenderSettings](../../aspose.cells/paginatedsaveoptions/customrendersettings/) { get; set; } | Obtient ou définit les paramètres personnalisés pendant le rendu. (Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DefaultEditLanguage](../../aspose.cells/paginatedsaveoptions/defaulteditlanguage/) { get; set; } | Obtient ou définit la langue d’édition par défaut. (Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DefaultFont](../../aspose.cells/paginatedsaveoptions/defaultfont/) { get; set; } | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le PDF ou l’image. Définissez la propriété DefaultFont, par exemple MingLiu ou MS Gothic, pour afficher ces caractères. Si cette propriété n’est pas définie, Aspose.Cells utilisera la police système par défaut pour afficher ces caractères Unicode. (Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DisplayDocTitle](../../aspose.cells/pdfsaveoptions/displaydoctitle/) { get; set; } | Indique si la barre de titre de la fenêtre doit afficher le titre du document. |
| [DrawObjectEventHandler](../../aspose.cells/paginatedsaveoptions/drawobjecteventhandler/) { get; set; } | Implémente cette interface pour obtenir DrawObject et Bound lors du rendu. (Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EmbedAttachments](../../aspose.cells/pdfsaveoptions/embedattachments/) { get; set; } | Indique s'il faut intégrer les pièces jointes pour les objets Ole dans Excel. |
| [EmbedStandardWindowsFonts](../../aspose.cells/pdfsaveoptions/embedstandardwindowsfonts/) { get; set; } | True pour intégrer les polices TrueType. N'affecte que les caractères ASCII 32-127. Les polices pour les codes de caractères supérieurs à 127 sont toujours intégrées. Les polices sont toujours intégrées pour les normes PDF/A-1a, PDF/A-1b. La valeur par défaut est true. |
| [EmfRenderSetting](../../aspose.cells/paginatedsaveoptions/emfrendersetting/) { get; set; } | Paramètre pour le rendu du métafichier Emf. (Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indique s’il faut chiffrer les propriétés du document lors de l’enregistrement au format .xls. La valeur par défaut est vraie.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [ExportDocumentStructure](../../aspose.cells/pdfsaveoptions/exportdocumentstructure/) { get; set; } | Indique s'il faut exporter la structure du document. |
| [FontEncoding](../../aspose.cells/pdfsaveoptions/fontencoding/) { get; set; } | Obtient ou définit l'encodage des polices intégrées dans le pdf. |
| [GridlineColor](../../aspose.cells/paginatedsaveoptions/gridlinecolor/) { get; set; } | Obtient ou définit la couleur des lignes de grille. (Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [GridlineType](../../aspose.cells/paginatedsaveoptions/gridlinetype/) { get; set; } | Obtient ou définit le type de ligne de grille.(Hérité de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [IgnoreError](../../aspose.cells/paginatedsaveoptions/ignoreerror/) { get; set; } | Indique si vous devez masquer l'erreur lors du rendu. L'erreur peut être une erreur de forme, d'image, de rendu de graphique, etc.(Hérité de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [ImageType](../../aspose.cells/pdfsaveoptions/imagetype/) { get; set; } | (**Obsolète.**) Représente le type d'image lors de la conversion du graphique et de la forme. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/paginatedsaveoptions/isfontsubstitutionchargranularity/) { get; set; } | Indique s'il faut uniquement substituer la police du caractère lorsque la police de la cellule n'est pas compatible avec celle-ci.(Hérité de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indique s’il faut fusionner les zones de mise en forme conditionnelle et de validation avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [OnePagePerSheet](../../aspose.cells/paginatedsaveoptions/onepagepersheet/) { get; set; } | Si OnePagePerSheet est vrai , tout le contenu d'une feuille sera exporté sur une seule page dans le résultat. La taille du papier du paramètre pagesetup sera invalide, et les autres paramètres de pagesetup resteront effectifs.(Hérité de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [OptimizationType](../../aspose.cells/pdfsaveoptions/optimizationtype/) { get; set; } | Obtient et définit le type d'optimisation du pdf. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/) { get; set; } | Indique s'il faut générer une page blanche lorsqu'il n'y a rien à imprimer.(Hérité de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageCount](../../aspose.cells/paginatedsaveoptions/pagecount/) { get; set; } | Obtient ou définit le nombre de pages à enregistrer.(Hérité de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageIndex](../../aspose.cells/paginatedsaveoptions/pageindex/) { get; set; } | Obtient ou définit l'index basé sur 0 de la première page à enregistrer.(Hérité de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageSavingCallback](../../aspose.cells/paginatedsaveoptions/pagesavingcallback/) { get; set; } | Contrôle/Indique la progression du processus d'enregistrement des pages.(Hérité de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PdfCompression](../../aspose.cells/pdfsaveoptions/pdfcompression/) { get; set; } | Indique l'algorithme de compression |
| [PrintingPageType](../../aspose.cells/paginatedsaveoptions/printingpagetype/) { get; set; } | Indique quelles pages ne seront pas imprimées.(Hérité de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [Producer](../../aspose.cells/pdfsaveoptions/producer/) { get; set; } | Obtient et définit le producteur du document pdf généré. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indique s’il faut mettre en cache les dernières données du graphique.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [RenderingBehavior](../../aspose.cells/paginatedsaveoptions/renderingbehavior/) { get; set; } | Obtient ou définit les comportements de rendu spécifiques à Excel à appliquer.(Hérité de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Obtient le format du fichier enregistré.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [SecurityOptions](../../aspose.cells/pdfsaveoptions/securityoptions/) { get; set; } | Définissez ces options, lorsque la sécurité est requise dans le résultat xls2pdf. |
| [SheetSet](../../aspose.cells/paginatedsaveoptions/sheetset/) { get; set; } | Obtient ou définit les feuilles à rendre. La valeur par défaut est toutes les feuilles visibles du classeur : [`Visible`](../../aspose.cells.rendering/sheetset/visible/).(Hérité de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indique s’il faut trier les noms définis externes avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indique s’il faut trier les noms définis avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [TextCrossType](../../aspose.cells/paginatedsaveoptions/textcrosstype/) { get; set; } | Obtient ou définit le type d'affichage du texte lorsque la largeur du texte dépasse celle de la cellule.(Hérité de [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indique s’il faut mettre à jour le paramètre smart art. La valeur par défaut est false.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indique s’il faut valider les cellules fusionnées avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Obtient ou définit le rappel d'avertissement.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [Watermark](../../aspose.cells/pdfsaveoptions/watermark/) { get; set; } | Obtient ou définit le filigrane à la sortie. |
| [ZoomBehavior](../../aspose.cells/pdfsaveoptions/zoombehavior/) { get; set; } | Obtient ou définit le mode de vue initial lorsque le document PDF généré est ouvert. La valeur par défaut est None. |
| [ZoomFactor](../../aspose.cells/pdfsaveoptions/zoomfactor/) { get; set; } | Obtient ou définit le pourcentage de zoom utilisé lorsque [`ZoomBehavior`](./zoombehavior/) est ZoomFactor. |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetImageResample](../../aspose.cells/pdfsaveoptions/setimageresample/)(int, int) | Définit le PPI (pixels par pouce) souhaité pour le rééchantillonnage des images et la qualité JPEG. Toutes les images seront converties en JPEG avec le paramètre de qualité spécifié, et les images dont le PPI dépasse le PPI spécifié (pixels par pouce) seront rééchantillonnées. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Rendering.PdfSecurity;
    using System;
    using System.Drawing;

    public class PdfSaveOptionsDemo
    {
        public static void PdfSaveOptionsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF Save Options Example");

            // Créer une instance de PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Définir diverses propriétés
            pdfSaveOptions.EmbedStandardWindowsFonts = true;
            pdfSaveOptions.Compliance = PdfCompliance.PdfA1b;
            pdfSaveOptions.CalculateFormula = true;
            pdfSaveOptions.PdfCompression = PdfCompressionCore.Flate;
            pdfSaveOptions.CreatedTime = DateTime.Now;
            pdfSaveOptions.Producer = "Aspose.Cells";
            pdfSaveOptions.OptimizationType = PdfOptimizationType.MinimumSize;
            pdfSaveOptions.CustomPropertiesExport = PdfCustomPropertiesExport.Standard;
            pdfSaveOptions.ExportDocumentStructure = true;
            pdfSaveOptions.DisplayDocTitle = true;
            pdfSaveOptions.FontEncoding = PdfFontEncoding.Identity;
            pdfSaveOptions.EmbedAttachments = true;
            pdfSaveOptions.DefaultFont = "Arial";
            pdfSaveOptions.CheckWorkbookDefaultFont = true;
            pdfSaveOptions.CheckFontCompatibility = true;
            pdfSaveOptions.IsFontSubstitutionCharGranularity = true;
            pdfSaveOptions.OnePagePerSheet = true;
            pdfSaveOptions.AllColumnsInOnePagePerSheet = true;
            pdfSaveOptions.IgnoreError = true;
            pdfSaveOptions.OutputBlankPageWhenNothingToPrint = true;
            pdfSaveOptions.PageIndex = 0;
            pdfSaveOptions.PageCount = 1;
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;
            pdfSaveOptions.GridlineType = GridlineType.Dotted;
            pdfSaveOptions.TextCrossType = TextCrossType.CrossKeep;
            pdfSaveOptions.DefaultEditLanguage = DefaultEditLanguage.English;
            pdfSaveOptions.SheetSet = SheetSet.Visible;
            pdfSaveOptions.ClearData = true;
            pdfSaveOptions.CachedFileFolder = "C:\\Temp";
            pdfSaveOptions.ValidateMergedAreas = true;
            pdfSaveOptions.MergeAreas = true;
            pdfSaveOptions.SortNames = true;
            pdfSaveOptions.SortExternalNames = true;
            pdfSaveOptions.RefreshChartCache = true;

            // Définir les options de sécurité
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions
            {
                OwnerPassword = "OwnerPassword",
                UserPassword = "UserPassword",
                PrintPermission = true,
                FullQualityPrintPermission = true
            };
            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;

            // Définir le filigrane
            RenderingFont font = new RenderingFont("Calibri", 68)
            {
                Italic = true,
                Bold = true,
                Color = Color.Blue
            };
            RenderingWatermark watermark = new RenderingWatermark("Watermark", font)
            {
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                Rotation = 30,
                Opacity = 0.6f,
                ScaleToPagePercent = 50
            };
            pdfSaveOptions.Watermark = watermark;

            // Enregistrer le classeur au format PDF
            workbook.Save("PdfSaveOptionsExample.pdf", pdfSaveOptions);
        }
    }
}
```

### Voir aussi

* class [PaginatedSaveOptions](../paginatedsaveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


