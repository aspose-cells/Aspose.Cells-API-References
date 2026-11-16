---
title: "Classe HtmlSaveOptions"
linktitle: "HtmlSaveOptions"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe HtmlSaveOptions. Encapsule l'objet qui représente htmlsaveoptions en Go."
type: docs
weight: 200
url: /fr/go-cpp/htmlsaveoptions/
---

## HtmlSaveOptions class

Représente les options pour enregistrer le fichier HTML.

```go

type HtmlSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewHtmlSaveOptions](./newhtmlsaveoptions/) | Crée des options pour enregistrer un fichier html. |
| [NewHtmlSaveOptions_SaveFormat](./newhtmlsaveoptions_saveformat/) | Crée des options pour enregistrer un fichier htm. |
| [NewHtmlSaveOptions_SaveOptions](./newhtmlsaveoptions_saveoptions/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetIgnoreInvisibleShapes](./getignoreinvisibleshapes/) | Indique si l'exportation des formes non visibles est effectuée |
| [SetIgnoreInvisibleShapes](./setignoreinvisibleshapes/) | Indique si l'exportation des formes non visibles est effectuée |
| [GetPageTitle](./getpagetitle/) | Le titre de la page HTML. Seulement lors de l'enregistrement vers un flux HTML. |
| [SetPageTitle](./setpagetitle/) | Le titre de la page HTML. Seulement lors de l'enregistrement vers un flux HTML. |
| [GetAttachedFilesDirectory](./getattachedfilesdirectory/) | Le répertoire où les fichiers joints seront enregistrés. Seulement lors de l'enregistrement vers un flux HTML. |
| [SetAttachedFilesDirectory](./setattachedfilesdirectory/) | Le répertoire où les fichiers joints seront enregistrés. Seulement lors de l'enregistrement vers un flux HTML. |
| [GetAttachedFilesUrlPrefix](./getattachedfilesurlprefix/) | Spécifiez le préfixe URL des fichiers joints tels que les images dans le fichier HTML. Seulement lors de l'enregistrement vers un flux HTML. |
| [SetAttachedFilesUrlPrefix](./setattachedfilesurlprefix/) | Spécifiez le préfixe URL des fichiers joints tels que les images dans le fichier HTML. Seulement lors de l'enregistrement vers un flux HTML. |
| [GetDefaultFontName](./getdefaultfontname/) | Spécifiez le nom de police par défaut pour l'exportation HTML, la police par défaut sera utilisée lorsque la police du style n'existe pas. Si cette propriété est nulle, Aspose.Cells utilisera une police universelle ayant la même famille que la police originale, la valeur par défaut est nulle. |
| [SetDefaultFontName](./setdefaultfontname/) | Spécifiez le nom de police par défaut pour l'exportation HTML, la police par défaut sera utilisée lorsque la police du style n'existe pas. Si cette propriété est nulle, Aspose.Cells utilisera une police universelle ayant la même famille que la police originale, la valeur par défaut est nulle. |
| [GetAddGenericFont](./getaddgenericfont/) | Indique s'il faut ajouter une police générique à la propriété CSS font-family. La valeur par défaut est true |
| [SetAddGenericFont](./setaddgenericfont/) | Indique s'il faut ajouter une police générique à la propriété CSS font-family. La valeur par défaut est true |
| [GetWorksheetScalable](./getworksheetscalable/) | Indique si le zoom avant ou arrière du HTML via le niveau de zoom de la feuille de calcul lors de l'enregistrement du fichier au format HTML, la valeur par défaut est false. |
| [SetWorksheetScalable](./setworksheetscalable/) | Indique si le zoom avant ou arrière du HTML via le niveau de zoom de la feuille de calcul lors de l'enregistrement du fichier au format HTML, la valeur par défaut est false. |
| [IsExportComments](./isexportcomments/) | Indique si les commentaires sont exportés lors de l'enregistrement du fichier au format HTML, la valeur par défaut est false. |
| [SetIsExportComments](./setisexportcomments/) | Indique si les commentaires sont exportés lors de l'enregistrement du fichier au format HTML, la valeur par défaut est false. |
| [GetExportCommentsType](./getexportcommentstype/) | Représente le type d'exportation des commentaires vers les fichiers HTML. |
| [SetExportCommentsType](./setexportcommentstype/) | Représente le type d'exportation des commentaires vers les fichiers HTML. |
| [GetDisableDownlevelRevealedComments](./getdisabledownlevelrevealedcomments/) | Indique si la désactivation des commentaires conditionnels révélés de bas niveau lors de l'exportation du fichier au format HTML, la valeur par défaut est false. |
| [SetDisableDownlevelRevealedComments](./setdisabledownlevelrevealedcomments/) | Indique si la désactivation des commentaires conditionnels révélés de bas niveau lors de l'exportation du fichier au format HTML, la valeur par défaut est false. |
| [IsExpImageToTempDir](./isexpimagetotempdir/) | Indique si les fichiers image sont exportés vers le répertoire temporaire. Uniquement lors de l'enregistrement vers le flux HTML. |
| [SetIsExpImageToTempDir](./setisexpimagetotempdir/) | Indique si les fichiers image sont exportés vers le répertoire temporaire. Uniquement lors de l'enregistrement vers le flux HTML. |
| [GetImageScalable](./getimagescalable/) | Indique si l'unité évolutive est utilisée pour décrire la largeur de l'image lorsqu'on utilise l'unité évolutive pour décrire la largeur de la colonne. La valeur par défaut est true. |
| [SetImageScalable](./setimagescalable/) | Indique si l'unité évolutive est utilisée pour décrire la largeur de l'image lorsqu'on utilise l'unité évolutive pour décrire la largeur de la colonne. La valeur par défaut est true. |
| [GetWidthScalable](./getwidthscalable/) | Indique si la largeur des colonnes est exportée en unité d'échelle vers le HTML. La valeur par défaut est false. |
| [SetWidthScalable](./setwidthscalable/) | Indique si la largeur des colonnes est exportée en unité d'échelle vers le HTML. La valeur par défaut est false. |
| [GetExportSingleTab](./getexportsingletab/) | Indique si l'onglet unique est exporté lorsque le fichier ne contient qu'une seule feuille de calcul. La valeur par défaut est false. |
| [SetExportSingleTab](./setexportsingletab/) | Indique si l'onglet unique est exporté lorsque le fichier ne contient qu'une seule feuille de calcul. La valeur par défaut est false. |
| [GetExportImagesAsBase64](./getexportimagesasbase64/) | Spécifie si les images sont enregistrées au format Base64 vers HTML, MHTML ou EPUB. |
| [SetExportImagesAsBase64](./setexportimagesasbase64/) | Spécifie si les images sont enregistrées au format Base64 vers HTML, MHTML ou EPUB. |
| [GetExportActiveWorksheetOnly](./getexportactiveworksheetonly/) | Indique si seul la feuille de calcul active est exportée vers le fichier HTML. Si true, alors seule la feuille active sera exportée vers le fichier HTML ; si false, l'ensemble du classeur sera exporté vers le fichier HTML. La valeur par défaut est false. |
| [SetExportActiveWorksheetOnly](./setexportactiveworksheetonly/) | Indique si seul la feuille de calcul active est exportée vers le fichier HTML. Si true, alors seule la feuille active sera exportée vers le fichier HTML ; si false, l'ensemble du classeur sera exporté vers le fichier HTML. La valeur par défaut est false. |
| [GetExportPrintAreaOnly](./getexportprintareaonly/) | Indique si seule la zone d'impression est exportée vers le fichier HTML. La valeur par défaut est false. |
| [SetExportPrintAreaOnly](./setexportprintareaonly/) | Indique si seule la zone d'impression est exportée vers le fichier HTML. La valeur par défaut est false. |
| [GetExportArea](./getexportarea/) | Obtient ou définit la zone de cellules (CellArea) à exporter de la feuille de calcul active actuelle. Si vous définissez cet attribut, la zone d'impression de la feuille active sera omise. Seule la zone spécifiée sera exportée lors de l'enregistrement du fichier au format HTML. |
| [SetExportArea](./setexportarea/) | Obtient ou définit la zone de cellules (CellArea) à exporter de la feuille de calcul active actuelle. Si vous définissez cet attribut, la zone d'impression de la feuille active sera omise. Seule la zone spécifiée sera exportée lors de l'enregistrement du fichier au format HTML. |
| [GetParseHtmlTagInCell](./getparsehtmltagincell/) | Indique si les balises HTML (comme <c>&lt;div&gt;&lt;/div&gt;</c>) dans la cellule doivent être analysées comme valeur de cellule ou conservées telles quelles. La valeur par défaut est true. |
| [SetParseHtmlTagInCell](./setparsehtmltagincell/) | Indique si les balises HTML (comme <c>&lt;div&gt;&lt;/div&gt;</c>) dans la cellule doivent être analysées comme valeur de cellule ou conservées telles quelles. La valeur par défaut est true. |
| [GetHtmlCrossStringType](./gethtmlcrossstringtype/) | Indique si une chaîne s'étendant sur plusieurs cellules sera affichée de la même manière que MS Excel lors de l'enregistrement d'un fichier Excel au format HTML. Par défaut, la valeur est Default, ainsi, pour les chaînes multi‑cellules, il y a peu de différence entre les fichiers HTML créés par Aspose.Cells et MS Excel. Mais les performances pour créer de gros fichiers HTML, en définissant la valeur à Cross, seraient plusieurs fois plus rapides que de la définir à Default ou Fit2Cell. |
| [SetHtmlCrossStringType](./sethtmlcrossstringtype/) | Indique si une chaîne s'étendant sur plusieurs cellules sera affichée de la même manière que MS Excel lors de l'enregistrement d'un fichier Excel au format HTML. Par défaut, la valeur est Default, ainsi, pour les chaînes multi‑cellules, il y a peu de différence entre les fichiers HTML créés par Aspose.Cells et MS Excel. Mais les performances pour créer de gros fichiers HTML, en définissant la valeur à Cross, seraient plusieurs fois plus rapides que de la définir à Default ou Fit2Cell. |
| [GetHiddenColDisplayType](./gethiddencoldisplaytype/) | Colonne masquée (la largeur de cette colonne est 0) dans Excel, avant de l'enregistrer au format HTML, si HtmlHiddenColDisplayType est "Remove", la colonne masquée ne sera pas sortie ; si la valeur est "Hidden", la colonne sera sortie mais restera masquée, la valeur par défaut est "Hidden". |
| [SetHiddenColDisplayType](./sethiddencoldisplaytype/) | Colonne masquée (la largeur de cette colonne est 0) dans Excel, avant de l'enregistrer au format HTML, si HtmlHiddenColDisplayType est "Remove", la colonne masquée ne sera pas sortie ; si la valeur est "Hidden", la colonne sera sortie mais restera masquée, la valeur par défaut est "Hidden". |
| [GetHiddenRowDisplayType](./gethiddenrowdisplaytype/) | Ligne masquée (la hauteur de cette ligne est 0) dans Excel, avant de l'enregistrer au format HTML, si HtmlHiddenRowDisplayType est "Remove", la ligne masquée ne sera pas sortie ; si la valeur est "Hidden", la ligne sera sortie mais restera masquée, la valeur par défaut est "Hidden". |
| [SetHiddenRowDisplayType](./sethiddenrowdisplaytype/) | Ligne masquée (la hauteur de cette ligne est 0) dans Excel, avant de l'enregistrer au format HTML, si HtmlHiddenRowDisplayType est "Remove", la ligne masquée ne sera pas sortie ; si la valeur est "Hidden", la ligne sera sortie mais restera masquée, la valeur par défaut est "Hidden". |
| [GetEncoding](./getencoding/) | Si non défini, utilise Encoding.UTF8 comme type d'encodage par défaut. |
| [SetEncoding](./setencoding/) | Si non défini, utilise Encoding.UTF8 comme type d'encodage par défaut. |
| [GetImageOptions](./getimageoptions/) | Obtenez l'objet ImageOrPrintOptions avant l'exportation. |
| [GetSaveAsSingleFile](./getsaveassinglefile/) | Indique si le HTML est enregistré comme fichier unique. La valeur par défaut est false. |
| [SetSaveAsSingleFile](./setsaveassinglefile/) | Indique si le HTML est enregistré comme fichier unique. La valeur par défaut est false. |
| [GetShowAllSheets](./getshowallsheets/) | Indique si toutes les feuilles sont affichées lors de l'enregistrement en un seul fichier HTML. |
| [SetShowAllSheets](./setshowallsheets/) | Indique si toutes les feuilles sont affichées lors de l'enregistrement en un seul fichier HTML. |
| [GetExportPageHeaders](./getexportpageheaders/) | Indique si les en-têtes de page sont exportés. |
| [SetExportPageHeaders](./setexportpageheaders/) | Indique si les en-têtes de page sont exportés. |
| [GetExportPageFooters](./getexportpagefooters/) | Indique si les en-têtes de page sont exportés. |
| [SetExportPageFooters](./setexportpagefooters/) | Indique si les en-têtes de page sont exportés. |
| [GetExportHiddenWorksheet](./getexporthiddenworksheet/) | Indique si le contenu des feuilles de calcul masquées est exporté. La valeur par défaut est true. |
| [SetExportHiddenWorksheet](./setexporthiddenworksheet/) | Indique si le contenu des feuilles de calcul masquées est exporté. La valeur par défaut est true. |
| [GetPresentationPreference](./getpresentationpreference/) | Indique si le fichier HTML ou MHT est la préférence de présentation. La valeur par défaut est false. Si vous souhaitez obtenir une présentation plus esthétique, veuillez définir la valeur sur true. |
| [SetPresentationPreference](./setpresentationpreference/) | Indique si le fichier HTML ou MHT est la préférence de présentation. La valeur par défaut est false. Si vous souhaitez obtenir une présentation plus esthétique, veuillez définir la valeur sur true. |
| [GetCellCssPrefix](./getcellcssprefix/) | Obtient et définit le préfixe du nom CSS, la valeur par défaut est "". |
| [SetCellCssPrefix](./setcellcssprefix/) | Obtient et définit le préfixe du nom CSS, la valeur par défaut est "". |
| [GetTableCssId](./gettablecssid/) | Obtient et définit le préfixe du type de nom CSS tel que tr, col, td, etc., ils sont contenus dans l'élément table qui possède l'attribut spécifique TableCssId. La valeur par défaut est "". |
| [SetTableCssId](./settablecssid/) | Obtient et définit le préfixe du type de nom CSS tel que tr, col, td, etc., ils sont contenus dans l'élément table qui possède l'attribut spécifique TableCssId. La valeur par défaut est "". |
| [IsFullPathLink](./isfullpathlink/) | Indique si l'utilisation d'un lien avec le chemin complet dans sheet00x.htm, filelist.xml et tabstrip.htm. La valeur par défaut est false. |
| [SetIsFullPathLink](./setisfullpathlink/) | Indique si l'utilisation d'un lien avec le chemin complet dans sheet00x.htm, filelist.xml et tabstrip.htm. La valeur par défaut est false. |
| [GetExportWorksheetCSSSeparately](./getexportworksheetcssseparately/) | Indique si l'exportation du CSS de la feuille de calcul séparément. La valeur par défaut est false. |
| [SetExportWorksheetCSSSeparately](./setexportworksheetcssseparately/) | Indique si l'exportation du CSS de la feuille de calcul séparément. La valeur par défaut est false. |
| [GetExportSimilarBorderStyle](./getexportsimilarborderstyle/) | Indique si l'exportation du style de bordure similaire lorsque le style de bordure n'est pas pris en charge par les navigateurs. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut. La valeur par défaut est false. |
| [SetExportSimilarBorderStyle](./setexportsimilarborderstyle/) | Indique si l'exportation du style de bordure similaire lorsque le style de bordure n'est pas pris en charge par les navigateurs. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut. La valeur par défaut est false. |
| [GetMergeEmptyTdType](./getmergeemptytdtype/) | Option de fusion des cellules vides contiguës (éléments td vides). La valeur par défaut est MergeEmptyTdType.Default. |
| [SetMergeEmptyTdType](./setmergeemptytdtype/) | Option de fusion des cellules vides contiguës (éléments td vides). La valeur par défaut est MergeEmptyTdType.Default. |
| [GetExportCellCoordinate](./getexportcellcoordinate/) | Indique si l'exportation des coordonnées Excel des cellules non vides lors de l'enregistrement du fichier au format html. La valeur par défaut est false. Si vous souhaitez importer le html généré dans Excel, veuillez conserver la valeur par défaut. |
| [SetExportCellCoordinate](./setexportcellcoordinate/) | Indique si l'exportation des coordonnées Excel des cellules non vides lors de l'enregistrement du fichier au format html. La valeur par défaut est false. Si vous souhaitez importer le html généré dans Excel, veuillez conserver la valeur par défaut. |
| [GetExportExtraHeadings](./getexportextraheadings/) | Indique si l'exportation d'en-têtes supplémentaires lorsque la longueur du texte dépasse la colonne d'affichage maximale. La valeur par défaut est false. Si vous souhaitez importer le fichier html dans Excel, veuillez conserver la valeur par défaut. |
| [SetExportExtraHeadings](./setexportextraheadings/) | Indique si l'exportation d'en-têtes supplémentaires lorsque la longueur du texte dépasse la colonne d'affichage maximale. La valeur par défaut est false. Si vous souhaitez importer le fichier html dans Excel, veuillez conserver la valeur par défaut. |
| [GetExportRowColumnHeadings](./getexportrowcolumnheadings/) | Indique si les en-têtes de lignes et de colonnes de la feuille sont exportés lors de l'enregistrement au format HTML. |
| [SetExportRowColumnHeadings](./setexportrowcolumnheadings/) | Indique si les en-têtes de lignes et de colonnes de la feuille sont exportés lors de l'enregistrement au format HTML. |
| [GetExportFormula](./getexportformula/) | Indique si les formules sont exportées lors de l'enregistrement du fichier au format html. La valeur par défaut est true. Si vous souhaitez importer le html généré dans Excel, veuillez conserver la valeur par défaut. |
| [SetExportFormula](./setexportformula/) | Indique si les formules sont exportées lors de l'enregistrement du fichier au format html. La valeur par défaut est true. Si vous souhaitez importer le html généré dans Excel, veuillez conserver la valeur par défaut. |
| [GetAddTooltipText](./getaddtooltiptext/) | Indique si un texte d'infobulle est ajouté lorsque les données ne peuvent pas être affichées entièrement. La valeur par défaut est false. |
| [SetAddTooltipText](./setaddtooltiptext/) | Indique si un texte d'infobulle est ajouté lorsque les données ne peuvent pas être affichées entièrement. La valeur par défaut est false. |
| [GetExportGridLines](./getexportgridlines/) | Indique si les lignes de grille sont exportées. La valeur par défaut est false. |
| [SetExportGridLines](./setexportgridlines/) | Indique si les lignes de grille sont exportées. La valeur par défaut est false. |
| [GetExportBogusRowData](./getexportbogusrowdata/) | Indique si les données de la dernière ligne factices sont exportées. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut. |
| [SetExportBogusRowData](./setexportbogusrowdata/) | Indique si les données de la dernière ligne factices sont exportées. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut. |
| [GetExcludeUnusedStyles](./getexcludeunusedstyles/) | Indique si les styles inutilisés sont exclus. Pour les fichiers html générés, exclure les styles inutilisés peut réduire la taille du fichier sans affecter les effets visuels. Ainsi, la valeur par défaut de cette propriété est true. Si l'utilisateur doit conserver tous les styles dans le classeur pour le html généré (par exemple dans le cas où l'utilisateur doit restaurer le classeur à partir du html généré ultérieurement), veuillez définir cette propriété sur false. |
| [SetExcludeUnusedStyles](./setexcludeunusedstyles/) | Indique si les styles inutilisés sont exclus. Pour les fichiers html générés, exclure les styles inutilisés peut réduire la taille du fichier sans affecter les effets visuels. Ainsi, la valeur par défaut de cette propriété est true. Si l'utilisateur doit conserver tous les styles dans le classeur pour le html généré (par exemple dans le cas où l'utilisateur doit restaurer le classeur à partir du html généré ultérieurement), veuillez définir cette propriété sur false. |
| [GetExportDocumentProperties](./getexportdocumentproperties/) | Indique si les propriétés du document sont exportées. La valeur par défaut est true. Si vous souhaitez importer le html ou le fichier mht dans Excel, veuillez conserver la valeur par défaut. |
| [SetExportDocumentProperties](./setexportdocumentproperties/) | Indique si les propriétés du document sont exportées. La valeur par défaut est true. Si vous souhaitez importer le html ou le fichier mht dans Excel, veuillez conserver la valeur par défaut. |
| [GetExportWorksheetProperties](./getexportworksheetproperties/) | Indique si les propriétés de la feuille de calcul sont exportées. La valeur par défaut est true. Si vous souhaitez importer le html ou le fichier mht dans Excel, veuillez conserver la valeur par défaut. |
| [SetExportWorksheetProperties](./setexportworksheetproperties/) | Indique si les propriétés de la feuille de calcul sont exportées. La valeur par défaut est true. Si vous souhaitez importer le html ou le fichier mht dans Excel, veuillez conserver la valeur par défaut. |
| [GetExportWorkbookProperties](./getexportworkbookproperties/) | Indique si les propriétés du classeur sont exportées. La valeur par défaut est true. Si vous souhaitez importer le html ou le fichier mht dans Excel, veuillez conserver la valeur par défaut. |
| [SetExportWorkbookProperties](./setexportworkbookproperties/) | Indique si les propriétés du classeur sont exportées. La valeur par défaut est true. Si vous souhaitez importer le html ou le fichier mht dans Excel, veuillez conserver la valeur par défaut. |
| [GetExportFrameScriptsAndProperties](./getexportframescriptsandproperties/) | Indique si les scripts d'iframe et les propriétés du document sont exportés. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut. |
| [SetExportFrameScriptsAndProperties](./setexportframescriptsandproperties/) | Indique si les scripts d'iframe et les propriétés du document sont exportés. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut. |
| [GetExportDataOptions](./getexportdataoptions/) | Indique la règle d'exportation des données du fichier html. La valeur par défaut est All. |
| [SetExportDataOptions](./setexportdataoptions/) | Indique la règle d'exportation des données du fichier html. La valeur par défaut est All. |
| [GetLinkTargetType](./getlinktargettype/) | Indique le type d'attribut target dans le lien <c>&lt;a&gt;</c>. La valeur par défaut est HtmlLinkTargetType.Parent. |
| [SetLinkTargetType](./setlinktargettype/) | Indique le type d'attribut target dans le lien <c>&lt;a&gt;</c>. La valeur par défaut est HtmlLinkTargetType.Parent. |
| [IsIECompatible](./isiecompatible/) | Indique si le HTML de sortie est compatible avec le navigateur IE. La valeur par défaut est false |
| [SetIsIECompatible](./setisiecompatible/) | Indique si le HTML de sortie est compatible avec le navigateur IE. La valeur par défaut est false |
| [GetFormatDataIgnoreColumnWidth](./getformatdataignorecolumnwidth/) | Indique si l'intégralité des données formatées d'une cellule doit être affichée lorsqu'elle déborde de la colonne. Si true, la largeur de la colonne est ignorée et toutes les données de la cellule seront exportées. Si false, les données seront exportées comme dans Excel. La valeur par défaut est false. |
| [SetFormatDataIgnoreColumnWidth](./setformatdataignorecolumnwidth/) | Indique si l'intégralité des données formatées d'une cellule doit être affichée lorsqu'elle déborde de la colonne. Si true, la largeur de la colonne est ignorée et toutes les données de la cellule seront exportées. Si false, les données seront exportées comme dans Excel. La valeur par défaut est false. |
| [GetCalculateFormula](./getcalculateformula/) | Indique si les formules doivent être calculées avant d'enregistrer le fichier html. |
| [SetCalculateFormula](./setcalculateformula/) | Indique si les formules doivent être calculées avant d'enregistrer le fichier html. |
| [IsJsBrowserCompatible](./isjsbrowsercompatible/) | Indique si le JavaScript est compatible avec les navigateurs qui ne supportent pas JavaScript. La valeur par défaut est true. |
| [SetIsJsBrowserCompatible](./setisjsbrowsercompatible/) | Indique si le JavaScript est compatible avec les navigateurs qui ne supportent pas JavaScript. La valeur par défaut est true. |
| [IsMobileCompatible](./ismobilecompatible/) | Indique si le HTML de sortie est compatible avec les appareils mobiles. La valeur par défaut est false. |
| [SetIsMobileCompatible](./setismobilecompatible/) | Indique si le HTML de sortie est compatible avec les appareils mobiles. La valeur par défaut est false. |
| [GetCssStyles](./getcssstyles/) | Obtient ou définit les styles CSS supplémentaires pour le formateur. Fonctionne uniquement lorsque SaveAsSingleFile est True. |
| [SetCssStyles](./setcssstyles/) | Obtient ou définit les styles CSS supplémentaires pour le formateur. Fonctionne uniquement lorsque SaveAsSingleFile est True. |
| [GetHideOverflowWrappedText](./gethideoverflowwrappedtext/) | Indique si le texte débordant doit être masqué lorsque le format de la cellule est réglé sur retour à la ligne. La valeur par défaut est false |
| [SetHideOverflowWrappedText](./sethideoverflowwrappedtext/) | Indique si le texte débordant doit être masqué lorsque le format de la cellule est réglé sur retour à la ligne. La valeur par défaut est false |
| [IsBorderCollapsed](./isbordercollapsed/) | Indique si les bordures du tableau sont réduites. La valeur par défaut est true. |
| [SetIsBorderCollapsed](./setisbordercollapsed/) | Indique si les bordures du tableau sont réduites. La valeur par défaut est true. |
| [GetEncodeEntityAsCode](./getencodeentityascode/) | Indique si les entités de caractères html sont remplacées par le code décimal. (par ex. "&amp;nbsp;" est remplacé par "&amp;#160;"). La valeur par défaut est false. |
| [SetEncodeEntityAsCode](./setencodeentityascode/) | Indique si les entités de caractères html sont remplacées par le code décimal. (par ex. "&amp;nbsp;" est remplacé par "&amp;#160;"). La valeur par défaut est false. |
| [GetOfficeMathOutputMode](./getofficemathoutputmode/) | Indique comment les objets OfficeMath sont exportés vers HTML. La valeur par défaut est Image. |
| [SetOfficeMathOutputMode](./setofficemathoutputmode/) | Indique comment les objets OfficeMath sont exportés vers HTML. La valeur par défaut est Image. |
| [GetCellNameAttribute](./getcellnameattribute/) | Spécifie l'attribut qui indique le CellName à écrire. (par ex. Si la valeur est "id", alors pour la cellule "A1", la sortie sera :&lt;td id='A1'&gt;). La valeur par défaut est null. |
| [SetCellNameAttribute](./setcellnameattribute/) | Spécifie l'attribut qui indique le CellName à écrire. (par ex. Si la valeur est "id", alors pour la cellule "A1", la sortie sera :&lt;td id='A1'&gt;). La valeur par défaut est null. |
| [GetDisableCss](./getdisablecss/) | Indique si seules les styles en ligne sont appliqués, sans dépendre du CSS. La valeur par défaut est false. |
| [SetDisableCss](./setdisablecss/) | Indique si seules les styles en ligne sont appliqués, sans dépendre du CSS. La valeur par défaut est false. |
| [GetEnableCssCustomProperties](./getenablecsscustomproperties/) | Optimise la sortie du html en utilisant des propriétés personnalisées CSS. Par exemple, dans le cas où il y a plusieurs occurrences d'une même image base64, avec une propriété personnalisée les données de l'image n'ont besoin d'être enregistrées qu'une fois, ce qui améliore les performances du html résultant. La valeur par défaut est false. |
| [SetEnableCssCustomProperties](./setenablecsscustomproperties/) | Optimise la sortie du html en utilisant des propriétés personnalisées CSS. Par exemple, dans le cas où il y a plusieurs occurrences d'une même image base64, avec une propriété personnalisée les données de l'image n'ont besoin d'être enregistrées qu'une fois, ce qui améliore les performances du html résultant. La valeur par défaut est false. |
| [GetHtmlVersion](./gethtmlversion/) | Spécifie la version de la norme HTML à utiliser lors de l'enregistrement du format HTML. La valeur par défaut est HtmlVersion.Default. |
| [SetHtmlVersion](./sethtmlversion/) | Spécifie la version de la norme HTML à utiliser lors de l'enregistrement du format HTML. La valeur par défaut est HtmlVersion.Default. |
| [GetSheetSet](./getsheetset/) | Obtient ou définit les feuilles à rendre. La valeur par défaut est toutes les feuilles visibles du classeur : Aspose.Cells.Rendering.SheetSet.Visible. |
| [SetSheetSet](./setsheetset/) | Obtient ou définit les feuilles à rendre. La valeur par défaut est toutes les feuilles visibles du classeur : Aspose.Cells.Rendering.SheetSet.Visible. |
| [GetLayoutMode](./getlayoutmode/) | Obtient ou définit le mode de mise en page lors de l'enregistrement en HTML. La valeur par défaut est HtmlLayoutMode.Normal |
| [SetLayoutMode](./setlayoutmode/) | Obtient ou définit le mode de mise en page lors de l'enregistrement en HTML. La valeur par défaut est HtmlLayoutMode.Normal |
| [GetEmbeddedFontType](./getembeddedfonttype/) | Obtient ou définit le type d'incorporation du fichier de police dans le fichier html. La valeur par défaut est HtmlEmbeddedFontType.None qui indique qu'aucune police ne sera incorporée dans le html. |
| [SetEmbeddedFontType](./setembeddedfonttype/) | Obtient ou définit le type d'incorporation du fichier de police dans le fichier html. La valeur par défaut est HtmlEmbeddedFontType.None qui indique qu'aucune police ne sera incorporée dans le html. |
| [GetExportNamedRangeAnchors](./getexportnamedrangeanchors/) | Indique s'il faut exporter les éléments d'ancre pour les plages nommées lors de l'enregistrement en HTML. La valeur par défaut est true. |
| [SetExportNamedRangeAnchors](./setexportnamedrangeanchors/) | Indique s'il faut exporter les éléments d'ancre pour les plages nommées lors de l'enregistrement en HTML. La valeur par défaut est true. |
| [GetDataBarRenderMode](./getdatabarrendermode/) | Représente le mode de rendu du DataBar lors de la conversion de fichiers Excel en fichiers html. La valeur par défaut est DataBarRenderMode.BackgroundColor. |
| [SetDataBarRenderMode](./setdatabarrendermode/) | Représente le mode de rendu du DataBar lors de la conversion de fichiers Excel en fichiers html. La valeur par défaut est DataBarRenderMode.BackgroundColor. |
| [GetSpaceMode](./getspacemode/) | Indique comment les espaces sont rendus dans la sortie HTML. Cette option s'applique actuellement uniquement aux formats numériques (par ex. format comptable). La valeur par défaut est HtmlSpaceMode.Css. |
| [SetSpaceMode](./setspacemode/) | Indique comment les espaces sont rendus dans la sortie HTML. Cette option s'applique actuellement uniquement aux formats numériques (par ex. format comptable). La valeur par défaut est HtmlSpaceMode.Css. |
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
