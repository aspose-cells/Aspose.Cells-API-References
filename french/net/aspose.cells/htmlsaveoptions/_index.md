---
title: HtmlSaveOptions
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente les options denregistrement du fichier html.
type: docs
weight: 3740
url: /fr/net/aspose.cells/htmlsaveoptions/
---
## HtmlSaveOptions class

Représente les options d'enregistrement du fichier html.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions#constructor)() | Crée des options pour enregistrer le fichier html. |
| [HtmlSaveOptions](htmlsaveoptions#constructor_1)(SaveFormat) | Crée des options pour enregistrer le fichier htm. |

## Propriétés

| Nom | La description |
| --- | --- |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext) { get; set; } | Indique s'il faut ajouter un texte d'info-bulle lorsque les données ne peuvent pas être entièrement affichées. La valeur par défaut est false. |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory) { get; set; } | Le répertoire dans lequel les fichiers joints seront enregistrés. Uniquement pour l'enregistrement dans le flux html. |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix) { get; set; } | Spécifiez le préfixe d'URL des fichiers joints tels que l'image dans le fichier html. Uniquement pour l'enregistrement dans le flux html. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder) { get; set; } | Le dossier de fichiers mis en cache est utilisé pour stocker des données volumineuses. |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix) { get; set; } | Obtient et définit le préfixe du nom CSS, la valeur par défaut est "". |
| [ClearData](../../aspose.cells/saveoptions/cleardata) { get; set; } | Videz le classeur après avoir enregistré le fichier. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory) { get; set; } | Si vrai et que le répertoire n'existe pas, le répertoire sera automatiquement créé avant d'enregistrer le fichier. |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname) { get; set; } | Spécifiez le nom de la police par défaut pour l'exportation html, la police par défaut sera utilisée lorsque la police de style n'existe pas, Si cette propriété est nulle, Aspose.Cells utilisera une police universelle qui a la même famille que la police d'origine, la valeur par défaut est null. |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments) { get; set; } | Indique si désactiver les commentaires conditionnels révélés par le niveau inférieur lors de l'exportation du fichier au format HTML, la valeur par défaut est false. |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding) { get; set; } | Si non défini, utilisez Encoding.UTF8 comme type d'encodage par défaut. |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles) { get; set; } | Indique si les styles inutilisés sont exclus. Pour les fichiers html générés, l'exclusion des styles inutilisés peut réduire la taille du fichier sans affecter les effets visuels. Ainsi, la valeur par défaut de cette propriété est true. Si l'utilisateur doit conserver tous les styles dans le classeur pour le html généré (comme le scénario dont user a besoin pour restaurer le classeur à partir du html généré plus tard), veuillez définir cette propriété sur false . |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly) { get; set; } | Indique si l'intégralité du classeur est exportée vers un fichier html. |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea) { get; set; } | Obtient ou définit la CellArea d'exportation de la feuille de calcul active actuelle. Si vous définissez cet attribut, la zone d'impression de la feuille de calcul active actuelle sera omise. Seule la zone spécifiée sera exportée lors de l'enregistrement du fichier au format html. |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata) { get; set; } | Indique si l'exportation de fausses données de la ligne inférieure. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht vers Excel, veuillez conserver la valeur par défaut. |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate) { get; set; } | Indique si l'exportation des coordonnées Excel des cellules non vides lors de l'enregistrement du fichier au format HTML. La valeur par défaut est false. Si vous souhaitez importer la sortie html vers Excel, veuillez conserver la valeur par défaut. |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions) { get; set; } | Indique la règle d'exportation des données du fichier html. La valeur par défaut est Tout. |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties) { get; set; } | Indique si les propriétés du document sont exportées. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht vers Excel, veuillez conserver la valeur par défaut. |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings) { get; set; } | Indique si des en-têtes supplémentaires sont exportés lorsque la longueur du texte dépasse la colonne d'affichage maximale. La valeur par défaut est false. Si vous souhaitez importer le fichier html vers Excel, veuillez conserver la valeur par défaut. |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula) { get; set; } | Indique si la formule est exportée lors de l'enregistrement du fichier au format HTML. La valeur par défaut est true. Si vous souhaitez importer la sortie html vers Excel, veuillez conserver la valeur par défaut. |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties) { get; set; } | Indique si l'exportation des scripts de cadre et des propriétés du document. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht vers Excel, veuillez conserver la valeur par défaut. |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines) { get; set; } | Indique si le quadrillage est exporté. La valeur par défaut est false. |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet) { get; set; } | Indique si le contenu masqué de la feuille de calcul est exporté. La valeur par défaut est true. |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64) { get; set; } | Spécifie si les images sont enregistrées au format Base64 au format HTML, MHTML ou EPUB. |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters) { get; set; } | Indique si l'exportation des en-têtes de page. |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders) { get; set; } | Indique si l'exportation des en-têtes de page. |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly) { get; set; } | Indique s'il s'agit d'exporter uniquement la zone d'impression vers un fichier html. La valeur par défaut est false. |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings) { get; set; } | Indique si les en-têtes de ligne et de colonne de la feuille sont exportés lors de l'enregistrement dans des fichiers HTML. |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle) { get; set; } | Indique si vous exportez le style de bordure similaire lorsque le style de bordure n'est pas pris en charge par les navigateurs. Si vous souhaitez importer le fichier html ou mht vers Excel, veuillez conserver la valeur par défaut. La valeur par défaut est false. |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab) { get; set; } | Indique s'il faut exporter l'onglet unique lorsque le fichier ne contient qu'une seule feuille de calcul. La valeur par défaut est false. |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties) { get; set; } | Indique si les propriétés du classeur sont exportées. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht vers Excel, veuillez conserver la valeur par défaut. |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately) { get; set; } | Indique si vous exportez la feuille de calcul CSS séparément. La valeur par défaut est false. |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties) { get; set; } | Indique si les propriétés de la feuille de calcul sont exportées. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht vers Excel, veuillez conserver la valeur par défaut. |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider) { get; set; } | Obtient ou définit le IFilePathProvider pour exporter la feuille de calcul au format HTML séparément. |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype) { get; set; } | Colonne masquée (la largeur de cette colonne est 0) dans Excel, avant de l'enregistrer au format html, si HtmlHiddenColDisplayType est "Supprimer", la colonne masquée ne serait pas sortie, si la valeur est "Masqué", la colonne serait été sortie, mais était masquée, la valeur par défaut est "Caché" |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype) { get; set; } | Ligne masquée (la hauteur de cette ligne est 0) dans Excel, avant de l'enregistrer au format html, si HtmlHiddenRowDisplayType est "Supprimer", la ligne masquée ne serait pas sortie, si la valeur est "Masqué", la ligne serait été sortie, mais était masquée, la valeur par défaut est "Caché" |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype) { get; set; } | Indique si une chaîne intercellulaire sera affichée de la même manière que MS Excel lors de l'enregistrement d'un fichier Excel au format html. Par défaut, la valeur est Default, donc, pour les chaînes intercellulaires, il y a peu de différence entre le format html fichiers créés par Aspose.Cells et MS Excel. Mais les performances de création de fichiers html volumineux, définir la valeur sur Cross seraient plusieurs fois plus rapides que de la définir sur Default ou Fit2Cell. |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes) { get; set; } | Indiquez si vous exportez ces formes non visibles |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions) { get; } | Obtenez l'objet ImageOrPrintOptions avant d'exporter |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable) { get; set; } | Indique si l'unité évolutive est utilisée pour décrire la largeur de l'image lors de l'utilisation d'une unité évolutive pour décrire la largeur de la colonne. La valeur par défaut est true. |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir) { get; set; } | Indique si les fichiers image sont exportés vers le répertoire temporaire. Uniquement pour l'enregistrement dans le flux html. |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments) { get; set; } | Indique si l'exportation des commentaires lors de l'enregistrement du fichier au format HTML, la valeur par défaut est false. |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink) { get; set; } | Indique si le lien de chemin d'accès complet est utilisé dans sheet00x.htm,filelist.xml et tabstrip.htm. La valeur par défaut est false. |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype) { get; set; } | indiquant le type d'attribut cible dans le lien &lt;a&gt;, la valeur par défaut est HtmlLinkTargetType.Parent. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas) { get; set; } | Indique si fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely) { get; set; } | Indique si la fusion forcée d'un élément TD vide lors de l'exportation du fichier au format HTML. La taille du fichier html sera considérablement réduite après avoir défini la valeur sur true. La valeur par défaut est faux. Si vous souhaitez importer le fichier html vers Excel ou exporter des lignes de grille parfaites lors de l'enregistrement du fichier au format html, veuillez conserver la valeur par défaut. |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle) { get; set; } | Le titre de la page html. Uniquement pour l'enregistrement dans le flux html. |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell) { get; set; } | Analyser la balise html dans la cellule, comme , en tant que valeur de cellule ou en tant que balise html, la valeur par défaut est true |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference) { get; set; } | Indique si le fichier html ou mht est la préférence de présentation. La valeur par défaut est false.if you want to get plus belle présentation, veuillez définir la valeur sur true. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache) { get; set; } | Indique si l'actualisation des données du cache du graphique |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile) { get; set; } | Indique si enregistrer le HTML en tant que fichier unique. La valeur par défaut est false. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat) { get; } | Obtient le format du fichier de sauvegarde. |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets) { get; set; } | Indique si toutes les feuilles sont affichées lors de l'enregistrement en un seul fichier html. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames) { get; set; } | Indique si le tri des noms définis externes avant d'enregistrer le fichier. |
| [SortNames](../../aspose.cells/saveoptions/sortnames) { get; set; } | Indique si le tri des noms définis avant d'enregistrer le fichier. |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider) { get; set; } | Obtient ou définit le IStreamProvider pour l'exportation d'objets. |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid) { get; set; } | Obtient et définit le préfixe du nom de type css tel que tr, col, td et ainsi de suite, ils sont contenus dans l'élément de table qui a l'attribut TableCssId spécifique. La valeur par défaut est "". |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart) { get; set; } | Indique si la mise à jour du paramètre Smart Art. La valeur par défaut est false. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas) { get; set; } | Indique si valider les cellules fusionnées avant d'enregistrer le fichier. |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback) { get; set; } | Obtient ou définit un rappel d'avertissement. |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable) { get; set; } | Indique si l'unité évolutive est utilisée pour décrire la largeur de la colonne lors de l'exportation du fichier au format html. La valeur par défaut est false. |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable) { get; set; } | Indique si un zoom avant ou arrière sur le HTML via le niveau de zoom de la feuille de calcul lors de l'enregistrement du fichier au format HTML, la valeur par défaut est false. |

### Voir également

* class [SaveOptions](../saveoptions)
* espace de noms [Aspose.Cells](../../aspose.cells)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
