---
title: "Classe HtmlSaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.HtmlSaveOptions. Représente les options pour enregistrer un fichier html"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/
---
## HtmlSaveOptions class

Représente les options pour enregistrer le fichier HTML.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions/#constructor)() | Crée des options pour enregistrer un fichier html. |
| [HtmlSaveOptions](htmlsaveoptions/#constructor_1)(SaveFormat) | Crée des options pour enregistrer un fichier htm. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AddGenericFont](../../aspose.cells/htmlsaveoptions/addgenericfont/) { get; set; } | Indique s'il faut ajouter une police générique à la propriété CSS font-family. La valeur par défaut est true |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext/) { get; set; } | Indique s'il faut ajouter du texte d'infobulle lorsque les données ne peuvent pas être affichées complètement. La valeur par défaut est false. |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory/) { get; set; } | Le répertoire où les fichiers joints seront enregistrés. Uniquement pour l'enregistrement dans un flux html. |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix/) { get; set; } | Spécifiez le préfixe d'URL des fichiers joints tels que les images dans le fichier html. Uniquement pour l'enregistrement dans un flux html. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Le dossier pour les fichiers temporaires qui peuvent être utilisés comme cache de données.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [CalculateFormula](../../aspose.cells/htmlsaveoptions/calculateformula/) { get; set; } | Indique s'il faut calculer les formules avant d'enregistrer le fichier html. |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix/) { get; set; } | Obtient et définit le préfixe du nom css, la valeur par défaut est "". |
| [CellNameAttribute](../../aspose.cells/htmlsaveoptions/cellnameattribute/) { get; set; } | Spécifie l'attribut qui indique le CellName à écrire. (par ex. Si la valeur est "id", alors pour la cellule "A1", la sortie sera :&lt;td id='A1'&gt;). La valeur par défaut est null. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Indique s’il faut vérifier les restrictions du fichier Excel lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n’autorise pas la saisie d’une chaîne de caractères supérieure à 32 K. Si vous saisissez une valeur supérieure à 32 K, elle sera tronquée.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Rendre le classeur vide après l’enregistrement du fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Si vrai et que le répertoire n’existe pas, le répertoire sera créé automatiquement avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [CssStyles](../../aspose.cells/htmlsaveoptions/cssstyles/) { get; set; } | Obtient ou définit les styles css supplémentaires pour le formatteur. Fonctionne uniquement lorsque [`SaveAsSingleFile`](./saveassinglefile/) est True.  CssStyles="body { padding: 5px }"; |
| [DataBarRenderMode](../../aspose.cells/htmlsaveoptions/databarrendermode/) { get; set; } | Représente le mode de rendu du DataBar lors de la conversion de fichiers Excel en fichiers html. La valeur par défaut est BackgroundColor. |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname/) { get; set; } | Spécifiez le nom de police par défaut pour l'exportation html, la police par défaut sera utilisée lorsque la police du style n'existe pas. Si cette propriété est null, Aspose.Cells utilisera une police universelle ayant la même famille que la police originale, la valeur par défaut est null. |
| [DisableCss](../../aspose.cells/htmlsaveoptions/disablecss/) { get; set; } | Indique si seuls les styles en ligne sont appliqués, sans dépendre du CSS. La valeur par défaut est false. |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/) { get; set; } | Indique s'il faut désactiver les commentaires conditionnels Downlevel-revealed lors de l'exportation du fichier en html, la valeur par défaut est false. |
| [EmbeddedFontType](../../aspose.cells/htmlsaveoptions/embeddedfonttype/) { get; set; } | Obtient ou définit le type d'intégration du fichier de police dans le fichier html. La valeur par défaut est None, ce qui indique qu'aucune police ne sera intégrée dans le html. |
| [EnableCssCustomProperties](../../aspose.cells/htmlsaveoptions/enablecsscustomproperties/) { get; set; } | Optimisez la sortie du html en utilisant des propriétés personnalisées CSS. Par exemple, dans le cas où il y a plusieurs occurrences d'une même image base64, avec une propriété personnalisée les données de l'image ne doivent être enregistrées qu'une fois, ce qui améliore les performances du html résultant. La valeur par défaut est false. |
| [EncodeEntityAsCode](../../aspose.cells/htmlsaveoptions/encodeentityascode/) { get; set; } | Indique si les entités de caractères html sont remplacées par un code décimal. (par ex. "&amp;nbsp;" est remplacé par "&amp;#160;"). La valeur par défaut est false. |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding/) { get; set; } | Si non défini, utilisez Encoding.UTF8 comme type d'encodage par défaut. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indique s’il faut chiffrer les propriétés du document lors de l’enregistrement au format .xls. La valeur par défaut est vraie.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles/) { get; set; } | Indique s'il faut exclure les styles inutilisés. Pour les fichiers html générés, exclure les styles inutilisés peut réduire la taille du fichier sans affecter les effets visuels. Ainsi, la valeur par défaut de cette propriété est true. Si l'utilisateur doit conserver tous les styles dans le classeur pour le html généré (par exemple dans le cas où l'utilisateur doit restaurer le classeur à partir du html généré ultérieurement), veuillez définir cette propriété sur false. |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly/) { get; set; } | Indique s'il faut n'exporter que la feuille de calcul active en fichier html. Si true, alors seule la feuille active sera exportée en html ; si false, tout le classeur sera exporté en html. La valeur par défaut est false. |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea/) { get; set; } | Obtient ou définit la CellArea d'exportation de la feuille de calcul active actuelle. Si vous définissez cet attribut, la zone d'impression de la feuille active sera omise. Seule la zone spécifiée sera exportée lors de l'enregistrement du fichier en html. |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata/) { get; set; } | Indiquant si l'exportation de données de ligne inférieure factices est activée. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans excel, veuillez conserver la valeur par défaut. |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate/) { get; set; } | Indique si l'exportation des coordonnées excel des cellules non vides lors de l'enregistrement du fichier en html est activée. La valeur par défaut est false. Si vous souhaitez importer le html généré dans excel, veuillez conserver la valeur par défaut. |
| [ExportCommentsType](../../aspose.cells/htmlsaveoptions/exportcommentstype/) { get; set; } | Représente le type d'exportation des commentaires vers les fichiers html. |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions/) { get; set; } | Indiquant la règle d'exportation des données du fichier html. La valeur par défaut est All. |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties/) { get; set; } | Indiquant si l'exportation des propriétés du document est activée. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans excel, veuillez conserver la valeur par défaut. |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings/) { get; set; } | Indique si l'exportation d'en-têtes supplémentaires est activée lorsque la longueur du texte dépasse la colonne d'affichage maximale. La valeur par défaut est false. Si vous souhaitez importer le fichier html dans excel, veuillez conserver la valeur par défaut. |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula/) { get; set; } | Indique si l'exportation des formules est activée lors de l'enregistrement du fichier en html. La valeur par défaut est true. Si vous souhaitez importer le html généré dans excel, veuillez conserver la valeur par défaut. |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties/) { get; set; } | Indiquant si l'exportation des scripts de cadre et des propriétés du document est activée. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans excel, veuillez conserver la valeur par défaut. |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines/) { get; set; } | Indiquant si l'exportation des quadrillages est activée. La valeur par défaut est false. |
| [ExportHeadings](../../aspose.cells/htmlsaveoptions/exportheadings/) { get; set; } | (**Obsolete.**) Indique si l'exportation des en-têtes de lignes et de colonnes de la feuille est activée lors de l'enregistrement en fichiers HTML. |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet/) { get; set; } | Indiquant si l'exportation du contenu de la feuille de calcul masquée est activée. La valeur par défaut est true. |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64/) { get; set; } | Spécifie si les images sont enregistrées au format Base64 vers HTML, MHTML ou EPUB. |
| [ExportNamedRangeAnchors](../../aspose.cells/htmlsaveoptions/exportnamedrangeanchors/) { get; set; } | Indique si l'exportation des éléments d'ancrage pour les plages nommées est activée lors de l'enregistrement en HTML. La valeur par défaut est true. |
| [ExportObjectListener](../../aspose.cells/htmlsaveoptions/exportobjectlistener/) { get; set; } | (**Obsolete.**) Obtient ou définit le ExportObjectListener pour l'exportation d'objets. |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters/) { get; set; } | Indique si l'exportation des en-têtes de page est activée. |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders/) { get; set; } | Indique si l'exportation des en-têtes de page est activée. |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly/) { get; set; } | Indique si seule la zone d'impression est exportée vers le fichier html. La valeur par défaut est false. |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings/) { get; set; } | Indique si l'exportation des en-têtes de lignes et de colonnes de la feuille est activée lors de l'enregistrement en fichiers HTML. |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle/) { get; set; } | Indiquant si l'exportation du style de bordure similaire est activée lorsque le style de bordure n'est pas pris en charge par les navigateurs. Si vous souhaitez importer le fichier html ou mht dans excel, veuillez conserver la valeur par défaut. La valeur par défaut est false. |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab/) { get; set; } | Indique si l'exportation d'un seul onglet est activée lorsque le fichier ne contient qu'une seule feuille de calcul. La valeur par défaut est false. |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties/) { get; set; } | Indiquant si l'exportation des propriétés du classeur est activée. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans excel, veuillez conserver la valeur par défaut. |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately/) { get; set; } | Indiquant si l'exportation du CSS de la feuille de calcul séparément est activée. La valeur par défaut est false. |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties/) { get; set; } | Indiquant si l'exportation des propriétés de la feuille de calcul est activée. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans excel, veuillez conserver la valeur par défaut. |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider/) { get; set; } | Obtient ou définit le IFilePathProvider pour l'exportation de la Worksheet en html séparément. |
| [FormatDataIgnoreColumnWidth](../../aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/) { get; set; } | Indiquant si l'affichage de l'intégralité des données formatées d'une cellule est activé lorsqu'elle dépasse la largeur de la colonne. Si true, la largeur de la colonne est ignorée et toutes les données de la cellule seront exportées. Si false, les données seront exportées comme dans Excel. La valeur par défaut est false. |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype/) { get; set; } | Colonne masquée (la largeur de cette colonne est 0) dans excel, avant de l'enregistrer au format html, si HtmlHiddenColDisplayType est "Remove", la colonne masquée ne sera pas sortie, si la valeur est "Hidden", la colonne sera sortie mais restera masquée, la valeur par défaut est "Hidden" |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/) { get; set; } | Ligne masquée (la hauteur de cette ligne est 0) dans Excel, avant de l’enregistrer au format HTML, si HtmlHiddenRowDisplayType est "Remove", la ligne masquée ne sera pas sortie, si la valeur est "Hidden", la ligne sera sortie mais masquée, la valeur par défaut est "Hidden" |
| [HideOverflowWrappedText](../../aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/) { get; set; } | Indique s’il faut masquer le texte débordant lorsque le format de la cellule est défini sur retour à la ligne. La valeur par défaut est false |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype/) { get; set; } | Indique si une chaîne traversant plusieurs cellules sera affichée de la même manière que MS Excel lors de l’enregistrement d’un fichier Excel au format HTML. Par défaut, la valeur est Default, ainsi, pour les chaînes traversant plusieurs cellules, il y a peu de différence entre les fichiers HTML créés par Aspose.Cells et MS Excel. Mais les performances pour créer de grands fichiers HTML, en définissant la valeur à Cross, seraient plusieurs fois plus rapides que de la définir à Default ou Fit2Cell. |
| [HtmlVersion](../../aspose.cells/htmlsaveoptions/htmlversion/) { get; set; } | Spécifie la version de la norme HTML qui doit être utilisée lors de l’enregistrement au format HTML. La valeur par défaut est HtmlVersion.Default. |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes/) { get; set; } | Indique s’il faut exporter les formes non visibles |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions/) { get; } | Obtenez l’objet ImageOrPrintOptions avant l’exportation |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable/) { get; set; } | Indique s’il faut utiliser une unité évolutive pour décrire la largeur de l’image lorsqu’on utilise une unité évolutive pour décrire la largeur de la colonne. La valeur par défaut est true. |
| [IsBorderCollapsed](../../aspose.cells/htmlsaveoptions/isbordercollapsed/) { get; set; } | Indique si les bordures du tableau sont fusionnées. La valeur par défaut est true. |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir/) { get; set; } | Indique s’il faut exporter les fichiers image vers un répertoire temporaire. Seulement lors de l’enregistrement dans un flux HTML. |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments/) { get; set; } | Indique s’il faut exporter les commentaires lors de l’enregistrement du fichier en HTML, la valeur par défaut est false. |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink/) { get; set; } | Indique s’il faut utiliser un lien avec chemin complet dans sheet00x.htm, filelist.xml et tabstrip.htm. La valeur par défaut est false. |
| [IsIECompatible](../../aspose.cells/htmlsaveoptions/isiecompatible/) { get; set; } | Indique si le HTML généré est compatible avec le navigateur IE. La valeur par défaut est false |
| [IsJsBrowserCompatible](../../aspose.cells/htmlsaveoptions/isjsbrowsercompatible/) { get; set; } | Indique si le JavaScript est compatible avec les navigateurs qui ne supportent pas JavaScript. La valeur par défaut est true. |
| [IsMobileCompatible](../../aspose.cells/htmlsaveoptions/ismobilecompatible/) { get; set; } | Indique si le HTML généré est compatible avec les appareils mobiles. La valeur par défaut est false. |
| [LayoutMode](../../aspose.cells/htmlsaveoptions/layoutmode/) { get; set; } | Obtient ou définit le mode de mise en page lors de l’enregistrement en HTML. La valeur par défaut est Normal |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype/) { get; set; } | Indique le type d’attribut target dans le lien `<a>`. La valeur par défaut est HtmlLinkTargetType.Parent. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indique s’il faut fusionner les zones de mise en forme conditionnelle et de validation avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely/) { get; set; } | (**Obsolete.**) Indique s’il faut fusionner les éléments TD vides de force lors de l’exportation du fichier en HTML. La taille du fichier HTML sera réduite de façon significative après avoir défini la valeur à true. La valeur par défaut est false. Si vous souhaitez importer le fichier HTML dans Excel ou exporter des lignes de grille parfaites lors de l’enregistrement du fichier en HTML, veuillez conserver la valeur par défaut. |
| [MergeEmptyTdType](../../aspose.cells/htmlsaveoptions/mergeemptytdtype/) { get; set; } | Option de fusion des cellules vides contiguës (éléments td vides). La valeur par défaut est MergeEmptyTdType.Default. |
| [OfficeMathOutputMode](../../aspose.cells/htmlsaveoptions/officemathoutputmode/) { get; set; } | Indique comment les objets OfficeMath sont exportés en HTML, la valeur par défaut est Image. |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle/) { get; set; } | Le titre de la page HTML. Seulement lors de l’enregistrement dans un flux HTML. |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell/) { get; set; } | Indique si les balises HTML (comme `<div></div>`) dans une cellule doivent être analysées comme valeur de cellule ou conservées telles quelles. La valeur par défaut est true. |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference/) { get; set; } | Indique si le fichier html ou mht est la préférence de présentation. La valeur par défaut est false. Si vous souhaitez obtenir une présentation plus esthétique, veuillez définir la valeur à true. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indique s’il faut mettre en cache les dernières données du graphique.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile/) { get; set; } | Indique s’il faut enregistrer le HTML en un seul fichier. La valeur par défaut est false. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Obtient le format du fichier enregistré.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [SheetSet](../../aspose.cells/htmlsaveoptions/sheetset/) { get; set; } | Obtient ou définit les feuilles à rendre. La valeur par défaut est toutes les feuilles visibles du classeur : [`Visible`](../../aspose.cells.rendering/sheetset/visible/). |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets/) { get; set; } | Indique s’il faut afficher toutes les feuilles lors de l’enregistrement en un seul fichier HTML. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indique s’il faut trier les noms définis externes avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indique s’il faut trier les noms définis avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [SpaceMode](../../aspose.cells/htmlsaveoptions/spacemode/) { get; set; } | Indique comment les espaces sont rendus dans la sortie HTML. Cette option est actuellement appliquée uniquement aux formats numériques (p. ex. format comptable). La valeur par défaut est Css. |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider/) { get; set; } | Obtient ou définit le IStreamProvider pour l'exportation d'objets. |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid/) { get; set; } | Obtient et définit le préfixe du nom CSS de type tel que tr, col, td, etc., ils sont contenus dans l'élément table qui possède l'attribut TableCssId spécifique. La valeur par défaut est "". |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indique s’il faut mettre à jour le paramètre smart art. La valeur par défaut est false.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indique s’il faut valider les cellules fusionnées avant d’enregistrer le fichier.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Obtient ou définit le rappel d'avertissement.(Hérité de [`SaveOptions`](../saveoptions/).) |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable/) { get; set; } | Indique si la largeur des colonnes est exportée en unité d'échelle vers HTML. La valeur par défaut est false. |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable/) { get; set; } | Indique si le zoom avant ou arrière du HTML via le niveau de zoom de la feuille de calcul lors de l'enregistrement du fichier en HTML, la valeur par défaut est false. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsDemo
    {
        public static void HtmlSaveOptionsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Créez une instance de HtmlSaveOptions
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                IgnoreInvisibleShapes = true,
                PageTitle = "Sample HTML Page",
                AttachedFilesDirectory = "attached_files",
                AttachedFilesUrlPrefix = "http://example.com/files/",
                DefaultFontName = "Arial",
                AddGenericFont = true,
                WorksheetScalable = false,
                IsExportComments = false,
                ExportCommentsType = PrintCommentsType.PrintNoComments,
                DisableDownlevelRevealedComments = false,
                IsExpImageToTempDir = false,
                ImageScalable = true,
                WidthScalable = false,
                ExportSingleTab = false,
                ExportImagesAsBase64 = false,
                ExportActiveWorksheetOnly = false,
                ExportPrintAreaOnly = false,
                ExportArea = new CellArea { StartRow = 0, EndRow = 1, StartColumn = 0, EndColumn = 1 },
                ParseHtmlTagInCell = true,
                HtmlCrossStringType = HtmlCrossType.Default,
                HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden,
                HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden,
                Encoding = System.Text.Encoding.UTF8,
                SaveAsSingleFile = false,
                ShowAllSheets = false,
                ExportPageHeaders = false,
                ExportPageFooters = false,
                ExportHiddenWorksheet = true,
                PresentationPreference = false,
                CellCssPrefix = "",
                TableCssId = "",
                IsFullPathLink = false,
                ExportWorksheetCSSSeparately = false,
                ExportSimilarBorderStyle = false,
                MergeEmptyTdForcely = false,
                MergeEmptyTdType = MergeEmptyTdType.Default,
                ExportCellCoordinate = false,
                ExportExtraHeadings = false,
                ExportHeadings = false,
                ExportRowColumnHeadings = false,
                ExportFormula = true,
                AddTooltipText = false,
                ExportGridLines = false,
                ExportBogusRowData = true,
                ExcludeUnusedStyles = true,
                ExportDocumentProperties = true,
                ExportWorksheetProperties = true,
                ExportWorkbookProperties = true,
                ExportFrameScriptsAndProperties = true,
                ExportDataOptions = HtmlExportDataOptions.All,
                LinkTargetType = HtmlLinkTargetType.Parent,
                IsIECompatible = false,
                FormatDataIgnoreColumnWidth = false,
                CalculateFormula = true,
                IsJsBrowserCompatible = true,
                IsMobileCompatible = false,
                CssStyles = "body { padding: 5px }",
                HideOverflowWrappedText = false,
                IsBorderCollapsed = true,
                ClearData = false,
                CachedFileFolder = "cache",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = true,
                SortExternalNames = true,
                RefreshChartCache = true,
                UpdateSmartArt = false
            };

            // Enregistrez le classeur au format HTML
            workbook.Save("HtmlSaveOptionsExample.html", saveOptions);

            return;
        }
    }
}
```

### Voir aussi

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


