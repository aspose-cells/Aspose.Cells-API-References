---
title: "Class EbookSaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Saving.EbookSaveOptions. Représente les options pour enregistrer un fichier ebook"
type: docs
url: /fr/net/aspose.cells.saving/ebooksaveoptions/
---
## EbookSaveOptions class

Représente les options d'enregistrement du fichier ebook.

```csharp
public class EbookSaveOptions : HtmlSaveOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [EbookSaveOptions](ebooksaveoptions/#constructor)() | Crée des options pour enregistrer le fichier ebook. |
| [EbookSaveOptions](ebooksaveoptions/#constructor_1)(SaveFormat) | Crée des options pour enregistrer le fichier ebook. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AddGenericFont](../../aspose.cells/htmlsaveoptions/addgenericfont/) { get; set; } | Indique s'il faut ajouter une police générique à la famille de polices CSS. La valeur par défaut est true (Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext/) { get; set; } | Indique s'il faut ajouter du texte d'infobulle lorsque les données ne peuvent pas être affichées entièrement. La valeur par défaut est false (Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory/) { get; set; } | Le répertoire où les fichiers joints seront enregistrés. Seulement pour l'enregistrement vers un flux html (Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix/) { get; set; } | Spécifiez le préfixe d'URL des fichiers joints tels que les images dans le fichier html. Seulement pour l'enregistrement vers un flux html (Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Le dossier pour les fichiers temporaires qui peuvent être utilisés comme cache de données (Hérité de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CalculateFormula](../../aspose.cells/htmlsaveoptions/calculateformula/) { get; set; } | Indique s'il faut calculer les formules avant d'enregistrer le fichier html (Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix/) { get; set; } | Obtient et définit le préfixe du nom CSS, la valeur par défaut est "" (Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CellNameAttribute](../../aspose.cells/htmlsaveoptions/cellnameattribute/) { get; set; } | Spécifie l'attribut qui indique le CellName à écrire. (par ex. si la valeur est "id", alors pour la cellule "A1", la sortie sera : &lt;td id='A1'&gt;). La valeur par défaut est null (Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Indique s'il faut vérifier les restrictions du fichier Excel lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Si vous saisissez une valeur supérieure à 32 K, elle sera tronquée (Hérité de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Vide le classeur après l'enregistrement du fichier (Hérité de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Si true et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier (Hérité de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CssStyles](../../aspose.cells/htmlsaveoptions/cssstyles/) { get; set; } | Obtient ou définit les styles CSS supplémentaires pour le formateur. Fonctionne uniquement lorsque [`SaveAsSingleFile`](../../aspose.cells/htmlsaveoptions/saveassinglefile/) est True. CssStyles="body { padding: 5px }" (Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DataBarRenderMode](../../aspose.cells/htmlsaveoptions/databarrendermode/) { get; set; } | Représente le mode de rendu du DataBar lors de la conversion de fichiers Excel en fichiers html. La valeur par défaut est BackgroundColor (Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname/) { get; set; } | Spécifiez le nom de police par défaut pour l'exportation html, la police par défaut sera utilisée lorsque la police du style n'existe pas. Si cette propriété est null, Aspose.Cells utilisera une police universelle ayant la même famille que la police originale, la valeur par défaut est null (Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DisableCss](../../aspose.cells/htmlsaveoptions/disablecss/) { get; set; } | Indique si seuls les styles en ligne sont appliqués, sans dépendre du CSS. La valeur par défaut est false (Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/) { get; set; } | Indique s'il faut désactiver les commentaires conditionnels Downlevel-revealed lors de l'exportation du fichier vers html, la valeur par défaut est false (Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EmbeddedFontType](../../aspose.cells/htmlsaveoptions/embeddedfonttype/) { get; set; } | Obtient ou définit le type d'intégration du fichier de police dans le fichier html. La valeur par défaut est None, ce qui indique qu'aucune police ne sera intégrée dans le html (Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EnableCssCustomProperties](../../aspose.cells/htmlsaveoptions/enablecsscustomproperties/) { get; set; } | Optimise la sortie du html en utilisant des propriétés personnalisées CSS. Par exemple, dans le cas où il y a plusieurs occurrences d'une même image base64, avec une propriété personnalisée les données de l'image n'ont besoin d'être enregistrées qu'une seule fois, ce qui améliore les performances du html résultant. La valeur par défaut est false (Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EncodeEntityAsCode](../../aspose.cells/htmlsaveoptions/encodeentityascode/) { get; set; } | Indique si les entités de caractères html sont remplacées par leur code décimal. (par ex. "&amp;nbsp;" est remplacé par "&amp;#160;"). La valeur par défaut est false (Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding/) { get; set; } | Si non défini, utilisez Encoding.UTF8 comme type d'encodage par défaut.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indique s'il faut chiffrer les propriétés du document lors de l'enregistrement au format .xls. La valeur par défaut est true.(Hérité de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles/) { get; set; } | Indique s'il faut exclure les styles inutilisés. Pour les fichiers html générés, exclure les styles inutilisés peut réduire la taille du fichier sans affecter l'aspect visuel. Ainsi, la valeur par défaut de cette propriété est true. Si l'utilisateur doit conserver tous les styles du classeur pour le html généré (par exemple dans le cas où il doit restaurer le classeur à partir du html généré plus tard), veuillez définir cette propriété sur false.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly/) { get; set; } | Indique si l'exportation ne concerne que la feuille de calcul active vers le fichier html. Si true, seule la feuille active sera exportée vers le fichier html ; si false, tout le classeur sera exporté vers le fichier html. La valeur par défaut est false.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea/) { get; set; } | Obtient ou définit la zone de cellules à exporter de la feuille de calcul active actuelle. Si vous définissez cet attribut, la zone d’impression de la feuille active sera omise. Seule la zone spécifiée sera exportée lors de l’enregistrement du fichier au format html.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata/) { get; set; } | Indique s'il faut exporter des données de ligne inférieure factices. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate/) { get; set; } | Indique s'il faut exporter les coordonnées Excel des cellules non vides lors de l’enregistrement du fichier au format html. La valeur par défaut est false. Si vous souhaitez importer le html généré dans Excel, veuillez conserver la valeur par défaut.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportCommentsType](../../aspose.cells/htmlsaveoptions/exportcommentstype/) { get; set; } | Représente le type d'exportation des commentaires vers les fichiers html.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions/) { get; set; } | Indique la règle d'exportation des données du fichier html. La valeur par défaut est All.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties/) { get; set; } | Indique s'il faut exporter les propriétés du document. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings/) { get; set; } | Indique s'il faut exporter des en-têtes supplémentaires lorsque la longueur du texte dépasse la colonne d'affichage maximale. La valeur par défaut est false. Si vous souhaitez importer le fichier html dans Excel, veuillez conserver la valeur par défaut.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula/) { get; set; } | Indique s'il faut exporter les formules lors de l’enregistrement du fichier au format html. La valeur par défaut est true. Si vous souhaitez importer le html généré dans Excel, veuillez conserver la valeur par défaut.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties/) { get; set; } | Indique s'il faut exporter les scripts d'encadré et les propriétés du document. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines/) { get; set; } | Indique s'il faut exporter les quadrillages. La valeur par défaut est false.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportHeadings](../../aspose.cells/htmlsaveoptions/exportheadings/) { get; set; } | (**Obsolète.**) Indique s'il faut exporter les en-têtes de lignes et de colonnes de la feuille lors de l'enregistrement au format HTML.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet/) { get; set; } | Indique s'il faut exporter le contenu des feuilles de calcul masquées. La valeur par défaut est true.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64/) { get; set; } | Spécifie si les images sont enregistrées au format Base64 dans HTML, MHTML ou EPUB.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportNamedRangeAnchors](../../aspose.cells/htmlsaveoptions/exportnamedrangeanchors/) { get; set; } | Indique s'il faut exporter les éléments d'ancre pour les plages nommées lors de l’enregistrement au format HTML. La valeur par défaut est true.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportObjectListener](../../aspose.cells/htmlsaveoptions/exportobjectlistener/) { get; set; } | (**Obsolète.**) Obtient ou définit le ExportObjectListener pour l'exportation d'objets.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters/) { get; set; } | Indique si les en-têtes de page sont exportés.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders/) { get; set; } | Indique si les en-têtes de page sont exportés.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly/) { get; set; } | Indique si seule la zone d'impression est exportée vers le fichier HTML. La valeur par défaut est false.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings/) { get; set; } | Indique si les en-têtes de lignes et de colonnes de la feuille sont exportés lors de l'enregistrement au format HTML.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle/) { get; set; } | Indique si le style de bordure similaire est exporté lorsque le style de bordure n'est pas pris en charge par les navigateurs. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut. La valeur par défaut est false.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab/) { get; set; } | Indique si l'onglet unique est exporté lorsque le fichier ne contient qu'une seule feuille de calcul. La valeur par défaut est false.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties/) { get; set; } | Indique si les propriétés du classeur sont exportées. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately/) { get; set; } | Indique si le CSS de la feuille de calcul est exporté séparément. La valeur par défaut est false.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties/) { get; set; } | Indique si les propriétés de la feuille de calcul sont exportées. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider/) { get; set; } | Obtient ou définit le IFilePathProvider pour l'exportation de la feuille de calcul vers HTML séparément.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [FormatDataIgnoreColumnWidth](../../aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/) { get; set; } | Indique si l'intégralité des données formatées d'une cellule est affichée lorsqu'elle déborde de la colonne. Si true, la largeur de colonne est ignorée et toutes les données de la cellule seront exportées. Si false, les données seront exportées comme dans Excel. La valeur par défaut est false.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype/) { get; set; } | Colonne masquée (la largeur de cette colonne est 0) dans Excel, avant de l'enregistrer au format HTML, si HtmlHiddenColDisplayType est "Remove", la colonne masquée ne sera pas générée, si la valeur est "Hidden", la colonne sera générée mais restera masquée, la valeur par défaut est "Hidden"(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/) { get; set; } | Ligne masquée (la hauteur de cette ligne est 0) dans Excel, avant de l'enregistrer au format HTML, si HtmlHiddenRowDisplayType est "Remove", la ligne masquée ne sera pas générée, si la valeur est "Hidden", la ligne sera générée mais restera masquée, la valeur par défaut est "Hidden"(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HideOverflowWrappedText](../../aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/) { get; set; } | Indique si le texte débordant doit être masqué lorsque le format de la cellule est défini sur retour à la ligne. La valeur par défaut est false(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype/) { get; set; } | Indique si une chaîne traversant plusieurs cellules sera affichée de la même manière que MS Excel lors de l'enregistrement d'un fichier Excel au format HTML. Par défaut, la valeur est Default, ainsi, pour les chaînes traversant plusieurs cellules, il y a peu de différence entre les fichiers HTML créés par Aspose.Cells et MS Excel. Cependant, les performances pour la création de gros fichiers HTML, en définissant la valeur à Cross, seront plusieurs fois plus rapides que lorsqu'elle est définie à Default ou Fit2Cell.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HtmlVersion](../../aspose.cells/htmlsaveoptions/htmlversion/) { get; set; } | Spécifie la version de la norme HTML à utiliser lors de l'enregistrement au format HTML. La valeur par défaut est HtmlVersion.Default.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes/) { get; set; } | Indique si les formes non visibles sont exportées(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions/) { get; } | Obtient l'objet ImageOrPrintOptions avant l'exportation(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable/) { get; set; } | Indique si l’on utilise l’unité évolutive pour décrire la largeur de l’image lors de l’utilisation de l’unité évolutive pour décrire la largeur de la colonne. La valeur par défaut est true.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsBorderCollapsed](../../aspose.cells/htmlsaveoptions/isbordercollapsed/) { get; set; } | Indique si les bordures du tableau sont fusionnées. La valeur par défaut est true.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir/) { get; set; } | Indique si l’exportation des fichiers image vers le répertoire temporaire est activée. Seulement lors de l’enregistrement vers un flux html.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments/) { get; set; } | Indique si les commentaires sont exportés lors de l’enregistrement du fichier au format html, la valeur par défaut est false.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink/) { get; set; } | Indique si l’on utilise un lien avec chemin complet dans sheet00x.htm, filelist.xml et tabstrip.htm. La valeur par défaut est false.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsIECompatible](../../aspose.cells/htmlsaveoptions/isiecompatible/) { get; set; } | Indique si le HTML généré est compatible avec le navigateur IE. La valeur par défaut est false(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsJsBrowserCompatible](../../aspose.cells/htmlsaveoptions/isjsbrowsercompatible/) { get; set; } | Indique si le JavaScript est compatible avec les navigateurs qui ne supportent pas JavaScript. La valeur par défaut est true.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsMobileCompatible](../../aspose.cells/htmlsaveoptions/ismobilecompatible/) { get; set; } | Indique si le HTML généré est compatible avec les appareils mobiles. La valeur par défaut est false.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [LayoutMode](../../aspose.cells/htmlsaveoptions/layoutmode/) { get; set; } | Obtient ou définit le mode de mise en page lors de l’enregistrement au format HTML. La valeur par défaut est Normal(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype/) { get; set; } | Indique le type d’attribut target dans le lien `<a>`. La valeur par défaut est HtmlLinkTargetType.Parent.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indique si les zones de mise en forme conditionnelle et de validation sont fusionnées avant l’enregistrement du fichier.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely/) { get; set; } | (**Obsolete.**) Indique si la fusion des éléments TD vides est forcée lors de l’exportation du fichier au format html. La taille du fichier html sera considérablement réduite après avoir défini la valeur sur true. La valeur par défaut est false. Si vous souhaitez importer le fichier html dans Excel ou exporter des lignes de grille parfaites lors de l’enregistrement du fichier au format html, veuillez conserver la valeur par défaut.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [MergeEmptyTdType](../../aspose.cells/htmlsaveoptions/mergeemptytdtype/) { get; set; } | L’option de fusion des cellules vides contiguës (éléments td vides). La valeur par défaut est MergeEmptyTdType.Default.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [OfficeMathOutputMode](../../aspose.cells/htmlsaveoptions/officemathoutputmode/) { get; set; } | Indique comment les objets OfficeMath sont exportés vers HTML, la valeur par défaut est Image.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle/) { get; set; } | Le titre de la page html. Seulement lors de l’enregistrement vers un flux html.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell/) { get; set; } | Indique si les balises html (comme `<div></div>`) dans la cellule doivent être analysées comme valeur de cellule ou conservées telles quelles. La valeur par défaut est true.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference/) { get; set; } | Indique si le fichier html ou mht est la préférence de présentation. La valeur par défaut est false. Si vous souhaitez obtenir une présentation plus esthétique, veuillez définir la valeur sur true.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indique si les dernières données du graphique doivent être mises en cache.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile/) { get; set; } | Indique si le html doit être enregistré en un seul fichier. La valeur par défaut est false.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Obtient le format de fichier d’enregistrement.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SheetSet](../../aspose.cells/htmlsaveoptions/sheetset/) { get; set; } | Obtient ou définit les feuilles à rendre. Par défaut, toutes les feuilles visibles du classeur : [`Visible`](../../aspose.cells.rendering/sheetset/visible/).(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets/) { get; set; } | Indique si toutes les feuilles sont affichées lors de l’enregistrement en un seul fichier html.(Inherited from [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indique si le tri des noms définis externes est effectué avant l'enregistrement du fichier.(Hérité de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indique si le tri des noms définis est effectué avant l'enregistrement du fichier.(Hérité de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SpaceMode](../../aspose.cells/htmlsaveoptions/spacemode/) { get; set; } | Indique comment les espaces sont rendus dans la sortie HTML. Cette option est actuellement appliquée uniquement aux formats numériques (p. ex. format comptable). La valeur par défaut est Css.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider/) { get; set; } | Obtient ou définit le IStreamProvider pour l'exportation des objets.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid/) { get; set; } | Obtient et définit le préfixe du nom CSS de type tel que tr, col, td, etc., ils sont contenus dans l'élément table qui possède l'attribut TableCssId spécifique. La valeur par défaut est "\"\"".(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indique si la mise à jour du paramètre SmartArt est activée. La valeur par défaut est false.(Hérité de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indique si la validation des cellules fusionnées est effectuée avant d'enregistrer le fichier.(Hérité de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Obtient ou définit le rappel d'avertissement.(Hérité de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable/) { get; set; } | Indique si l'exportation de la largeur des colonnes en unité d'échelle vers HTML est activée. La valeur par défaut est false.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable/) { get; set; } | Indique si le zoom avant ou arrière du HTML via le niveau de zoom de la feuille de calcul est appliqué lors de l'enregistrement du fichier en HTML, la valeur par défaut est false.(Hérité de [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class EbookSaveOptionsDemo
    {
        public static void EbookSaveOptionsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello World");

            // Créez une instance de EbookSaveOptions
            EbookSaveOptions saveOptions = new EbookSaveOptions();

            // Définition des propriétés
            saveOptions.IgnoreInvisibleShapes = true;
            saveOptions.PageTitle = "Sample Page Title";
            saveOptions.AttachedFilesDirectory = "attached_files";
            saveOptions.AttachedFilesUrlPrefix = "http://example.com/files/";
            saveOptions.DefaultFontName = "Arial";
            saveOptions.AddGenericFont = true;
            saveOptions.WorksheetScalable = false;
            saveOptions.IsExportComments = false;
            saveOptions.ExportCommentsType = PrintCommentsType.PrintNoComments;
            saveOptions.DisableDownlevelRevealedComments = false;
            saveOptions.IsExpImageToTempDir = false;
            saveOptions.ImageScalable = true;
            saveOptions.WidthScalable = false;
            saveOptions.ExportSingleTab = false;
            saveOptions.ExportImagesAsBase64 = false;
            saveOptions.ExportActiveWorksheetOnly = false;
            saveOptions.ExportPrintAreaOnly = false;
            saveOptions.ExportArea = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            saveOptions.ParseHtmlTagInCell = true;
            saveOptions.HtmlCrossStringType = HtmlCrossType.Default;
            saveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden;
            saveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;
            saveOptions.Encoding = System.Text.Encoding.UTF8;
            saveOptions.SaveAsSingleFile = false;
            saveOptions.ShowAllSheets = true;
            saveOptions.ExportPageHeaders = true;
            saveOptions.ExportPageFooters = true;
            saveOptions.ExportHiddenWorksheet = true;
            saveOptions.PresentationPreference = false;
            saveOptions.CellCssPrefix = "cell_";
            saveOptions.TableCssId = "table_";
            saveOptions.IsFullPathLink = false;
            saveOptions.ExportWorksheetCSSSeparately = false;
            saveOptions.ExportSimilarBorderStyle = false;
            saveOptions.MergeEmptyTdForcely = false;
            saveOptions.MergeEmptyTdType = MergeEmptyTdType.Default;
            saveOptions.ExportCellCoordinate = false;
            saveOptions.ExportExtraHeadings = false;
            saveOptions.ExportHeadings = true;
            saveOptions.ExportRowColumnHeadings = true;
            saveOptions.ExportFormula = true;
            saveOptions.AddTooltipText = false;
            saveOptions.ExportGridLines = false;
            saveOptions.ExportBogusRowData = true;
            saveOptions.ExcludeUnusedStyles = true;
            saveOptions.ExportDocumentProperties = true;
            saveOptions.ExportWorksheetProperties = true;
            saveOptions.ExportWorkbookProperties = true;
            saveOptions.ExportFrameScriptsAndProperties = true;
            saveOptions.ExportDataOptions = HtmlExportDataOptions.All;
            saveOptions.LinkTargetType = HtmlLinkTargetType.Parent;
            saveOptions.IsIECompatible = false;
            saveOptions.FormatDataIgnoreColumnWidth = false;
            saveOptions.CalculateFormula = true;
            saveOptions.IsJsBrowserCompatible = true;
            saveOptions.IsMobileCompatible = false;
            saveOptions.CssStyles = "body { padding: 5px }";
            saveOptions.HideOverflowWrappedText = false;
            saveOptions.IsBorderCollapsed = true;
            saveOptions.ClearData = true;
            saveOptions.CachedFileFolder = "cache";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = true;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = true;
            saveOptions.RefreshChartCache = true;
            saveOptions.WarningCallback = null;
            saveOptions.UpdateSmartArt = true;

            // Enregistrez le classeur dans un fichier HTML avec les options spécifiées
            workbook.Save("EbookSaveOptionsExample.html", saveOptions);

            return;
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../../aspose.cells/htmlsaveoptions/)
* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


