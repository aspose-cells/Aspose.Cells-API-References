---
title: "HtmlSaveOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les options d'enregistrement du fichier html."
type: docs
url: /fr/java/com.aspose.cells/htmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class HtmlSaveOptions extends SaveOptions
```

Représente les options d'enregistrement du fichier html.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [HtmlSaveOptions()](#HtmlSaveOptions--) | Crée des options pour enregistrer un fichier html. |
| [HtmlSaveOptions(int saveFormat)](#HtmlSaveOptions-int-) | Crée des options pour enregistrer un fichier htm. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddGenericFont()](#getAddGenericFont--) | Indique s'il faut ajouter une police générique à la propriété CSS font-family. |
| [getAddTooltipText()](#getAddTooltipText--) | Indique s'il faut ajouter du texte d'infobulle lorsque les données ne peuvent pas être affichées complètement. |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | Le répertoire où les fichiers joints seront enregistrés. |
| [getAttachedFilesUrlPrefix()](#getAttachedFilesUrlPrefix--) | Spécifie le préfixe d'URL des fichiers joints tels que les images dans le fichier HTML. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |
| [getCalculateFormula()](#getCalculateFormula--) | Indique s'il faut calculer les formules avant d'enregistrer le fichier HTML. |
| [getCellCssPrefix()](#getCellCssPrefix--) | Obtient le préfixe du nom CSS, la valeur par défaut est "". |
| [getCellNameAttribute()](#getCellNameAttribute--) | Spécifie l'attribut qui indique le CellName à écrire. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Rendre le classeur vide après l'enregistrement du fichier. |
| [getCreateDirectory()](#getCreateDirectory--) | Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier. |
| [getCssStyles()](#getCssStyles--) | Obtient les styles CSS supplémentaires pour le formateur. |
| [getDataBarRenderMode()](#getDataBarRenderMode--) | Représente le mode de rendu du DataBar lors de la conversion de fichiers Excel en fichiers HTML. |
| [getDefaultFontName()](#getDefaultFontName--) | Spécifie le nom de police par défaut pour l'exportation HTML, la police par défaut sera utilisée lorsque la police du style n'existe pas. Si cette propriété est null, Aspose.Cells utilisera une police universelle ayant la même famille que la police originale, la valeur par défaut est null. |
| [getDisableCss()](#getDisableCss--) | Indique si seules les styles en ligne sont appliqués, sans dépendre du CSS. |
| [getDisableDownlevelRevealedComments()](#getDisableDownlevelRevealedComments--) | Indique s'il faut désactiver les commentaires conditionnels Downlevel-revealed lors de l'exportation du fichier en HTML, la valeur par défaut est false. |
| [getEmbeddedFontType()](#getEmbeddedFontType--) | Obtient le type d'intégration du fichier de police dans le fichier HTML. |
| [getEnableCssCustomProperties()](#getEnableCssCustomProperties--) | Optimise la sortie HTML en utilisant des propriétés personnalisées CSS. |
| [getEncodeEntityAsCode()](#getEncodeEntityAsCode--) | Indique si les entités de caractères HTML sont remplacées par des codes décimaux. |
| [getEncoding()](#getEncoding--) | Si non défini, utilise Encoding.UTF8 comme type d'encodage par défaut. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indique s'il faut chiffrer les propriétés du document lors de l'enregistrement au format .xls. |
| [getExcludeUnusedStyles()](#getExcludeUnusedStyles--) | Indiquant s'il faut exclure les styles inutilisés. |
| [getExportActiveWorksheetOnly()](#getExportActiveWorksheetOnly--) | Indique si seul la feuille de calcul active est exportée vers le fichier HTML. |
| [getExportArea()](#getExportArea--) | Obtient la zone de cellules (CellArea) exportée de la feuille de calcul active actuelle. |
| [getExportBogusRowData()](#getExportBogusRowData--) | Indiquant s'il faut exporter des données de ligne inférieure factices. |
| [getExportCellCoordinate()](#getExportCellCoordinate--) | Indique s'il faut exporter les coordonnées Excel des cellules non vides lors de l'enregistrement du fichier en HTML. |
| [getExportCommentsType()](#getExportCommentsType--) | Représente le type d'exportation des commentaires vers les fichiers HTML. |
| [getExportDataOptions()](#getExportDataOptions--) | Indiquant la règle d'exportation des données du fichier HTML. La valeur par défaut est All. |
| [getExportDocumentProperties()](#getExportDocumentProperties--) | Indiquant s'il faut exporter les propriétés du document. La valeur par défaut est true. Si vous souhaitez importer le fichier HTML ou MHT dans Excel, veuillez conserver la valeur par défaut. |
| [getExportExtraHeadings()](#getExportExtraHeadings--) | Indique s'il faut exporter des en-têtes supplémentaires lorsque la longueur du texte dépasse la colonne d'affichage maximale. |
| [getExportFormula()](#getExportFormula--) | Indique s'il faut exporter les formules lors de l'enregistrement du fichier en HTML. |
| [getExportFrameScriptsAndProperties()](#getExportFrameScriptsAndProperties--) | Indique si l'exportation des scripts d'images et des propriétés du document. |
| [getExportGridLines()](#getExportGridLines--) | Indique si l'exportation des quadrillages. La valeur par défaut est false. |
| [getExportHeadings()](#getExportHeadings--) | Indique si l'exportation des en-têtes de lignes et de colonnes de la feuille lors de l'enregistrement au format HTML. |
| [getExportHiddenWorksheet()](#getExportHiddenWorksheet--) | Indique si le contenu de la feuille de calcul masqué est exporté. La valeur par défaut est true. |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--) | Spécifie si les images sont enregistrées au format Base64 dans HTML, MHTML ou EPUB. |
| [getExportNamedRangeAnchors()](#getExportNamedRangeAnchors--) | Indique si les éléments d'ancrage pour les plages nommées sont exportés lors de l'enregistrement au format HTML. |
| [getExportObjectListener()](#getExportObjectListener--) | Obtient le ExportObjectListener pour l'exportation des objets. |
| [getExportPageFooters()](#getExportPageFooters--) | Indique si les en-têtes de page sont exportés. |
| [getExportPageHeaders()](#getExportPageHeaders--) | Indique si les en-têtes de page sont exportés. |
| [getExportPrintAreaOnly()](#getExportPrintAreaOnly--) | Indique si seule la zone d'impression est exportée vers le fichier HTML. |
| [getExportRowColumnHeadings()](#getExportRowColumnHeadings--) | Indique si l'exportation des en-têtes de lignes et de colonnes de la feuille lors de l'enregistrement au format HTML. |
| [getExportSimilarBorderStyle()](#getExportSimilarBorderStyle--) | Indique si le style de bordure similaire est exporté lorsque le style de bordure n'est pas pris en charge par les navigateurs. |
| [getExportSingleTab()](#getExportSingleTab--) | Indique si l'onglet unique est exporté lorsque le fichier ne contient qu'une seule feuille de calcul. |
| [getExportWorkbookProperties()](#getExportWorkbookProperties--) | Indique si les propriétés du classeur sont exportées. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut. |
| [getExportWorksheetCSSSeparately()](#getExportWorksheetCSSSeparately--) | Indique si le CSS de la feuille de calcul est exporté séparément. La valeur par défaut est false. |
| [getExportWorksheetProperties()](#getExportWorksheetProperties--) | Indique si les propriétés de la feuille de calcul sont exportées. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut. |
| [getFilePathProvider()](#getFilePathProvider--) | Obtient le IFilePathProvider pour l'exportation de la feuille de calcul au format HTML séparément. |
| [getFormatDataIgnoreColumnWidth()](#getFormatDataIgnoreColumnWidth--) | Indique si l'intégralité des données formatées d'une cellule est affichée lorsqu'elle dépasse la colonne. |
| [getHiddenColDisplayType()](#getHiddenColDisplayType--) | Colonne masquée (la largeur de cette colonne est 0) dans Excel, avant de l'enregistrer au format HTML, si HtmlHiddenColDisplayType est "Remove", la colonne masquée ne sera pas sortie, si la valeur est "Hidden", la colonne sera sortie mais restera masquée, la valeur par défaut est "Hidden". |
| [getHiddenRowDisplayType()](#getHiddenRowDisplayType--) | Ligne masquée (la hauteur de cette ligne est 0) dans Excel, avant de l'enregistrer au format HTML, si HtmlHiddenRowDisplayType est "Remove", la ligne masquée ne sera pas sortie, si la valeur est "Hidden", la ligne sera sortie mais restera masquée, la valeur par défaut est "Hidden". |
| [getHideOverflowWrappedText()](#getHideOverflowWrappedText--) | Indique si le texte débordant doit être masqué lorsque le format de la cellule est réglé sur retour à la ligne. |
| [getHtmlCrossStringType()](#getHtmlCrossStringType--) | Indique si une chaîne traversant plusieurs cellules sera affichée de la même manière que MS Excel lors de l'enregistrement d'un fichier Excel au format HTML. |
| [getHtmlVersion()](#getHtmlVersion--) | Spécifie la version de la norme HTML qui doit être utilisée lors de l'enregistrement au format HTML. |
| [getIgnoreInvisibleShapes()](#getIgnoreInvisibleShapes--) | Indique si les formes non visibles sont exportées |
| [getImageOptions()](#getImageOptions--) | Obtenez l'objet ImageOrPrintOptions avant l'exportation |
| [getImageScalable()](#getImageScalable--) | Indique si l'unité évolutive est utilisée pour décrire la largeur de l'image lorsqu'on utilise l'unité évolutive pour décrire la largeur de la colonne. |
| [getLayoutMode()](#getLayoutMode--) | Obtient le mode de mise en page lors de l'enregistrement au format HTML. |
| [getLinkTargetType()](#getLinkTargetType--) | Indication du type d'attribut cible dans le lien `<a>`. |
| [getMergeAreas()](#getMergeAreas--) | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. |
| [getMergeEmptyTdForcely()](#getMergeEmptyTdForcely--) | Indique si la fusion des éléments TD vides est forcée lors de l'exportation du fichier en HTML. |
| [getMergeEmptyTdType()](#getMergeEmptyTdType--) | L'option de fusion des cellules vides contiguës (éléments td vides). La valeur par défaut est MergeEmptyTdType.Default. |
| [getOfficeMathOutputMode()](#getOfficeMathOutputMode--) | Indique comment les objets OfficeMath sont exportés en HTML, la valeur par défaut est Image. |
| [getPageTitle()](#getPageTitle--) | Le titre de la page HTML. |
| [getParseHtmlTagInCell()](#getParseHtmlTagInCell--) | Indique si les balises HTML (comme `<div></div>`) dans la cellule doivent être analysées comme valeur de cellule ou conservées telles quelles. |
| [getPresentationPreference()](#getPresentationPreference--) | Indication si le fichier html ou mht est la préférence de présentation. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indique s'il faut mettre en cache les dernières données du graphique. |
| [getSaveAsSingleFile()](#getSaveAsSingleFile--) | Indique si le HTML doit être enregistré en tant que fichier unique. |
| [getSaveFormat()](#getSaveFormat--) | Obtient le format de fichier d'enregistrement. |
| [getSheetSet()](#getSheetSet--) | Obtient les feuilles à rendre. |
| [getShowAllSheets()](#getShowAllSheets--) | Indique si toutes les feuilles sont affichées lors de l'enregistrement en un seul fichier HTML. |
| [getSortExternalNames()](#getSortExternalNames--) | Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier. |
| [getSortNames()](#getSortNames--) | Indique s'il faut trier les noms définis avant d'enregistrer le fichier. |
| [getSpaceMode()](#getSpaceMode--) | Indique comment les espaces sont rendus dans la sortie HTML. |
| [getStreamProvider()](#getStreamProvider--) | Obtient le IStreamProvider pour l'exportation des objets. |
| [getTableCssId()](#getTableCssId--) | Obtient le préfixe du nom CSS de type tel que tr, col, td, etc., ils sont contenus dans l'élément table qui possède l'attribut TableCssId spécifique. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indique s'il faut mettre à jour le paramètre SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier. |
| [getWarningCallback()](#getWarningCallback--) | Obtient le rappel d'avertissement. |
| [getWidthScalable()](#getWidthScalable--) | Indique si la largeur des colonnes est exportée en unité d'échelle vers le HTML. |
| [getWorksheetScalable()](#getWorksheetScalable--) | Indique si le zoom avant ou arrière du HTML via le niveau de zoom de la feuille de calcul est appliqué lors de l'enregistrement du fichier en HTML, la valeur par défaut est false. |
| [hashCode()](#hashCode--) |  |
| [isBorderCollapsed()](#isBorderCollapsed--) | Indique si les bordures du tableau sont fusionnées. |
| [isExpImageToTempDir()](#isExpImageToTempDir--) | Indique si les fichiers image sont exportés vers le répertoire temporaire. |
| [isExportComments()](#isExportComments--) | Indique si les commentaires sont exportés lors de l'enregistrement du fichier en HTML, la valeur par défaut est false. |
| [isFullPathLink()](#isFullPathLink--) | Indication si l'on utilise un lien avec le chemin complet dans sheet00x.htm, filelist.xml et tabstrip.htm. |
| [isIECompatible()](#isIECompatible--) | Indication si le HTML de sortie est compatible avec le navigateur IE. |
| [isJsBrowserCompatible()](#isJsBrowserCompatible--) | Indique si le JavaScript est compatible avec les navigateurs qui ne supportent pas JavaScript. |
| [isMobileCompatible()](#isMobileCompatible--) | Indique si le HTML de sortie est compatible avec les appareils mobiles. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddGenericFont(boolean value)](#setAddGenericFont-boolean-) | Indique s'il faut ajouter une police générique à la propriété CSS font-family. |
| [setAddTooltipText(boolean value)](#setAddTooltipText-boolean-) | Indique s'il faut ajouter du texte d'infobulle lorsque les données ne peuvent pas être affichées complètement. |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | Le répertoire où les fichiers joints seront enregistrés. |
| [setAttachedFilesUrlPrefix(String value)](#setAttachedFilesUrlPrefix-java.lang.String-) | Spécifie le préfixe d'URL des fichiers joints tels que les images dans le fichier HTML. |
| [setBorderCollapsed(boolean value)](#setBorderCollapsed-boolean-) | Indique si les bordures du tableau sont fusionnées. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Indique s'il faut calculer les formules avant d'enregistrer le fichier HTML. |
| [setCellCssPrefix(String value)](#setCellCssPrefix-java.lang.String-) | Définit le préfixe du nom CSS, la valeur par défaut est "". |
| [setCellNameAttribute(String value)](#setCellNameAttribute-java.lang.String-) | Spécifie l'attribut qui indique le CellName à écrire. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indique si la vérification des restrictions du fichier Excel est effectuée lorsque l'utilisateur modifie les objets liés aux cellules. |
| [setClearData(boolean value)](#setClearData-boolean-) | Rendre le classeur vide après l'enregistrement du fichier. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier. |
| [setCssStyles(String value)](#setCssStyles-java.lang.String-) | Définit les styles CSS supplémentaires pour le formateur. |
| [setDataBarRenderMode(int value)](#setDataBarRenderMode-int-) | Représente le mode de rendu du DataBar lors de la conversion de fichiers Excel en fichiers HTML. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Spécifie le nom de police par défaut pour l'exportation HTML, la police par défaut sera utilisée lorsque la police du style n'existe pas. Si cette propriété est null, Aspose.Cells utilisera une police universelle ayant la même famille que la police originale, la valeur par défaut est null. |
| [setDisableCss(boolean value)](#setDisableCss-boolean-) | Indique si seules les styles en ligne sont appliqués, sans dépendre du CSS. |
| [setDisableDownlevelRevealedComments(boolean value)](#setDisableDownlevelRevealedComments-boolean-) | Indique s'il faut désactiver les commentaires conditionnels Downlevel-revealed lors de l'exportation du fichier en HTML, la valeur par défaut est false. |
| [setEmbeddedFontType(int value)](#setEmbeddedFontType-int-) | Définit le type d'intégration du fichier de police dans le fichier HTML. |
| [setEnableCssCustomProperties(boolean value)](#setEnableCssCustomProperties-boolean-) | Optimise la sortie HTML en utilisant des propriétés personnalisées CSS. |
| [setEncodeEntityAsCode(boolean value)](#setEncodeEntityAsCode-boolean-) | Indique si les entités de caractères HTML sont remplacées par des codes décimaux. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Si non défini, utilise Encoding.UTF8 comme type d'encodage par défaut. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indique s'il faut chiffrer les propriétés du document lors de l'enregistrement au format .xls. |
| [setExcludeUnusedStyles(boolean value)](#setExcludeUnusedStyles-boolean-) | Indiquant s'il faut exclure les styles inutilisés. |
| [setExpImageToTempDir(boolean value)](#setExpImageToTempDir-boolean-) | Indique si les fichiers image sont exportés vers le répertoire temporaire. |
| [setExportActiveWorksheetOnly(boolean value)](#setExportActiveWorksheetOnly-boolean-) | Indique si seul la feuille de calcul active est exportée vers le fichier HTML. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | Définit la CellArea d'exportation de la Worksheet active actuelle. |
| [setExportBogusRowData(boolean value)](#setExportBogusRowData-boolean-) | Indiquant s'il faut exporter des données de ligne inférieure factices. |
| [setExportCellCoordinate(boolean value)](#setExportCellCoordinate-boolean-) | Indique s'il faut exporter les coordonnées Excel des cellules non vides lors de l'enregistrement du fichier en HTML. |
| [setExportComments(boolean value)](#setExportComments-boolean-) | Indique si les commentaires sont exportés lors de l'enregistrement du fichier en HTML, la valeur par défaut est false. |
| [setExportCommentsType(int value)](#setExportCommentsType-int-) | Représente le type d'exportation des commentaires vers les fichiers HTML. |
| [setExportDataOptions(int value)](#setExportDataOptions-int-) | Indiquant la règle d'exportation des données du fichier HTML. La valeur par défaut est All. |
| [setExportDocumentProperties(boolean value)](#setExportDocumentProperties-boolean-) | Indiquant s'il faut exporter les propriétés du document. La valeur par défaut est true. Si vous souhaitez importer le fichier HTML ou MHT dans Excel, veuillez conserver la valeur par défaut. |
| [setExportExtraHeadings(boolean value)](#setExportExtraHeadings-boolean-) | Indique s'il faut exporter des en-têtes supplémentaires lorsque la longueur du texte dépasse la colonne d'affichage maximale. |
| [setExportFormula(boolean value)](#setExportFormula-boolean-) | Indique s'il faut exporter les formules lors de l'enregistrement du fichier en HTML. |
| [setExportFrameScriptsAndProperties(boolean value)](#setExportFrameScriptsAndProperties-boolean-) | Indique si l'exportation des scripts d'images et des propriétés du document. |
| [setExportGridLines(boolean value)](#setExportGridLines-boolean-) | Indique si l'exportation des quadrillages. La valeur par défaut est false. |
| [setExportHeadings(boolean value)](#setExportHeadings-boolean-) | Indique si l'exportation des en-têtes de lignes et de colonnes de la feuille lors de l'enregistrement au format HTML. |
| [setExportHiddenWorksheet(boolean value)](#setExportHiddenWorksheet-boolean-) | Indique si le contenu de la feuille de calcul masqué est exporté. La valeur par défaut est true. |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | Spécifie si les images sont enregistrées au format Base64 dans HTML, MHTML ou EPUB. |
| [setExportNamedRangeAnchors(boolean value)](#setExportNamedRangeAnchors-boolean-) | Indique si les éléments d'ancrage pour les plages nommées sont exportés lors de l'enregistrement au format HTML. |
| [setExportObjectListener(IExportObjectListener value)](#setExportObjectListener-com.aspose.cells.IExportObjectListener-) | Définit le ExportObjectListener pour l'exportation des objets. |
| [setExportPageFooters(boolean value)](#setExportPageFooters-boolean-) | Indique si les en-têtes de page sont exportés. |
| [setExportPageHeaders(boolean value)](#setExportPageHeaders-boolean-) | Indique si les en-têtes de page sont exportés. |
| [setExportPrintAreaOnly(boolean value)](#setExportPrintAreaOnly-boolean-) | Indique si seule la zone d'impression est exportée vers le fichier HTML. |
| [setExportRowColumnHeadings(boolean value)](#setExportRowColumnHeadings-boolean-) | Indique si l'exportation des en-têtes de lignes et de colonnes de la feuille lors de l'enregistrement au format HTML. |
| [setExportSimilarBorderStyle(boolean value)](#setExportSimilarBorderStyle-boolean-) | Indique si le style de bordure similaire est exporté lorsque le style de bordure n'est pas pris en charge par les navigateurs. |
| [setExportSingleTab(boolean value)](#setExportSingleTab-boolean-) | Indique si l'onglet unique est exporté lorsque le fichier ne contient qu'une seule feuille de calcul. |
| [setExportWorkbookProperties(boolean value)](#setExportWorkbookProperties-boolean-) | Indique si les propriétés du classeur sont exportées. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut. |
| [setExportWorksheetCSSSeparately(boolean value)](#setExportWorksheetCSSSeparately-boolean-) | Indique si le CSS de la feuille de calcul est exporté séparément. La valeur par défaut est false. |
| [setExportWorksheetProperties(boolean value)](#setExportWorksheetProperties-boolean-) | Indique si les propriétés de la feuille de calcul sont exportées. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut. |
| [setFilePathProvider(IFilePathProvider value)](#setFilePathProvider-com.aspose.cells.IFilePathProvider-) | Définit le IFilePathProvider pour exporter la Worksheet en html séparément. |
| [setFormatDataIgnoreColumnWidth(boolean value)](#setFormatDataIgnoreColumnWidth-boolean-) | Indique si l'intégralité des données formatées d'une cellule est affichée lorsqu'elle dépasse la colonne. |
| [setFullPathLink(boolean value)](#setFullPathLink-boolean-) | Indication si l'on utilise un lien avec le chemin complet dans sheet00x.htm, filelist.xml et tabstrip.htm. |
| [setHiddenColDisplayType(int value)](#setHiddenColDisplayType-int-) | Colonne masquée (la largeur de cette colonne est 0) dans Excel, avant de l'enregistrer au format HTML, si HtmlHiddenColDisplayType est "Remove", la colonne masquée ne sera pas sortie, si la valeur est "Hidden", la colonne sera sortie mais restera masquée, la valeur par défaut est "Hidden". |
| [setHiddenRowDisplayType(int value)](#setHiddenRowDisplayType-int-) | Ligne masquée (la hauteur de cette ligne est 0) dans Excel, avant de l'enregistrer au format HTML, si HtmlHiddenRowDisplayType est "Remove", la ligne masquée ne sera pas sortie, si la valeur est "Hidden", la ligne sera sortie mais restera masquée, la valeur par défaut est "Hidden". |
| [setHideOverflowWrappedText(boolean value)](#setHideOverflowWrappedText-boolean-) | Indique si le texte débordant doit être masqué lorsque le format de la cellule est réglé sur retour à la ligne. |
| [setHtmlCrossStringType(int value)](#setHtmlCrossStringType-int-) | Indique si une chaîne traversant plusieurs cellules sera affichée de la même manière que MS Excel lors de l'enregistrement d'un fichier Excel au format HTML. |
| [setHtmlVersion(int value)](#setHtmlVersion-int-) | Spécifie la version de la norme HTML qui doit être utilisée lors de l'enregistrement au format HTML. |
| [setIECompatible(boolean value)](#setIECompatible-boolean-) | Indication si le HTML de sortie est compatible avec le navigateur IE. |
| [setIgnoreInvisibleShapes(boolean value)](#setIgnoreInvisibleShapes-boolean-) | Indique si les formes non visibles sont exportées |
| [setImageScalable(boolean value)](#setImageScalable-boolean-) | Indique si l'unité évolutive est utilisée pour décrire la largeur de l'image lorsqu'on utilise l'unité évolutive pour décrire la largeur de la colonne. |
| [setJsBrowserCompatible(boolean value)](#setJsBrowserCompatible-boolean-) | Indique si le JavaScript est compatible avec les navigateurs qui ne supportent pas JavaScript. |
| [setLayoutMode(int value)](#setLayoutMode-int-) | Définit le mode de mise en page lors de l'enregistrement en HTML. |
| [setLinkTargetType(int value)](#setLinkTargetType-int-) | Indication du type d'attribut cible dans le lien `<a>`. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier. |
| [setMergeEmptyTdForcely(boolean value)](#setMergeEmptyTdForcely-boolean-) | Indique si la fusion des éléments TD vides est forcée lors de l'exportation du fichier en HTML. |
| [setMergeEmptyTdType(int value)](#setMergeEmptyTdType-int-) | L'option de fusion des cellules vides contiguës (éléments td vides). La valeur par défaut est MergeEmptyTdType.Default. |
| [setMobileCompatible(boolean value)](#setMobileCompatible-boolean-) | Indique si le HTML de sortie est compatible avec les appareils mobiles. |
| [setOfficeMathOutputMode(int value)](#setOfficeMathOutputMode-int-) | Indique comment les objets OfficeMath sont exportés en HTML, la valeur par défaut est Image. |
| [setPageTitle(String value)](#setPageTitle-java.lang.String-) | Le titre de la page HTML. |
| [setParseHtmlTagInCell(boolean value)](#setParseHtmlTagInCell-boolean-) | Indique si les balises HTML (comme `<div></div>`) dans la cellule doivent être analysées comme valeur de cellule ou conservées telles quelles. |
| [setPresentationPreference(boolean value)](#setPresentationPreference-boolean-) | Indication si le fichier html ou mht est la préférence de présentation. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indique s'il faut mettre en cache les dernières données du graphique. |
| [setSaveAsSingleFile(boolean value)](#setSaveAsSingleFile-boolean-) | Indique si le HTML doit être enregistré en tant que fichier unique. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Définit les feuilles à rendre. |
| [setShowAllSheets(boolean value)](#setShowAllSheets-boolean-) | Indique si toutes les feuilles sont affichées lors de l'enregistrement en un seul fichier HTML. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indique s'il faut trier les noms définis avant d'enregistrer le fichier. |
| [setSpaceMode(int value)](#setSpaceMode-int-) | Indique comment les espaces sont rendus dans la sortie HTML. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Définit le IStreamProvider pour l'exportation des objets. |
| [setTableCssId(String value)](#setTableCssId-java.lang.String-) | Définit le préfixe du type de nom CSS tel que tr, col, td, etc., ils sont contenus dans l'élément table qui possède l'attribut TableCssId spécifique. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indique s'il faut mettre à jour le paramètre SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Définit le rappel d’avertissement. |
| [setWidthScalable(boolean value)](#setWidthScalable-boolean-) | Indique si la largeur des colonnes est exportée en unité d'échelle vers le HTML. |
| [setWorksheetScalable(boolean value)](#setWorksheetScalable-boolean-) | Indique si le zoom avant ou arrière du HTML via le niveau de zoom de la feuille de calcul est appliqué lors de l'enregistrement du fichier en HTML, la valeur par défaut est false. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### HtmlSaveOptions() {#HtmlSaveOptions--}
```
public HtmlSaveOptions()
```


Crée des options pour enregistrer un fichier html.

### HtmlSaveOptions(int saveFormat) {#HtmlSaveOptions-int-}
```
public HtmlSaveOptions(int saveFormat)
```


Crée des options pour enregistrer un fichier htm.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Le format de fichier. Il doit être l'un des types suivants : [SaveFormat.HTML](../../com.aspose.cells/saveformat\#HTML) ou [SaveFormat.M\_HTML](../../com.aspose.cells/saveformat\#M-HTML), sinon le format enregistré sera automatiquement défini sur [SaveFormat.HTML](../../com.aspose.cells/saveformat\#HTML). |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAddGenericFont() {#getAddGenericFont--}
```
public boolean getAddGenericFont()
```


Indique s'il faut ajouter une police générique à la propriété CSS font-family. La valeur par défaut est true.

**Returns:**
boolean
### getAddTooltipText() {#getAddTooltipText--}
```
public boolean getAddTooltipText()
```


Indique s'il faut ajouter du texte d'infobulle lorsque les données ne peuvent pas être affichées entièrement. La valeur par défaut est false.

**Returns:**
boolean
### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}
```
public String getAttachedFilesDirectory()
```


Le répertoire où les fichiers joints seront enregistrés. Seulement pour l'enregistrement dans un flux html.

**Returns:**
java.lang.String
### getAttachedFilesUrlPrefix() {#getAttachedFilesUrlPrefix--}
```
public String getAttachedFilesUrlPrefix()
```


Spécifiez le préfixe Url des fichiers joints tels que les images dans le fichier html. Seulement pour l'enregistrement dans un flux html.

**Returns:**
java.lang.String
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données.

**Remarks**

Si le dossier n'a pas été spécifié, la valeur par défaut est [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Si sa valeur par défaut est nulle ou vide, ou a été spécifiée comme nulle ou vide, aucun fichier de cache ne sera utilisé lors de l'enregistrement du classeur.

**Returns:**
java.lang.String
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```


Indique s'il faut calculer les formules avant d'enregistrer le fichier HTML.

**Remarks**

La valeur par défaut est false.

**Returns:**
boolean
### getCellCssPrefix() {#getCellCssPrefix--}
```
public String getCellCssPrefix()
```


Obtient le préfixe du nom CSS, la valeur par défaut est "".

**Returns:**
java.lang.String
### getCellNameAttribute() {#getCellNameAttribute--}
```
public String getCellNameAttribute()
```


Spécifie l'attribut qui indique le CellName à écrire. (par ex. Si la valeur est "id", alors pour la cellule "A1", la sortie sera : <td id='A1'>). La valeur par défaut est null.

**Returns:**
java.lang.String
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Vérifie la restriction du fichier Excel lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, elle sera tronquée.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClearData() {#getClearData--}
```
public boolean getClearData()
```


Rendre le classeur vide après l'enregistrement du fichier.

**Returns:**
boolean
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier.

**Remarks**

La valeur par défaut est false.

**Returns:**
boolean
### getCssStyles() {#getCssStyles--}
```
public String getCssStyles()
```


Obtient les styles CSS supplémentaires pour le formateur. Fonctionne uniquement lorsque [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) est True. CssStyles="body \{ padding: 5px \}";

**Returns:**
java.lang.String
### getDataBarRenderMode() {#getDataBarRenderMode--}
```
public int getDataBarRenderMode()
```


Représente le mode de rendu du DataBar lors de la conversion de fichiers Excel en fichiers html. La valeur par défaut est [DataBarRenderMode.BACKGROUND\_COLOR](../../com.aspose.cells/databarrendermode\#BACKGROUND-COLOR).

Voir [DataBarRenderMode](../../com.aspose.cells/databarrendermode).

**Returns:**
int
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Spécifie le nom de police par défaut pour l'exportation HTML, la police par défaut sera utilisée lorsque la police du style n'existe pas. Si cette propriété est null, Aspose.Cells utilisera une police universelle ayant la même famille que la police originale, la valeur par défaut est null.

**Returns:**
java.lang.String
### getDisableCss() {#getDisableCss--}
```
public boolean getDisableCss()
```


Indique si seuls les styles en ligne sont appliqués, sans dépendre du CSS. La valeur par défaut est false.

**Returns:**
boolean
### getDisableDownlevelRevealedComments() {#getDisableDownlevelRevealedComments--}
```
public boolean getDisableDownlevelRevealedComments()
```


Indique s'il faut désactiver les commentaires conditionnels Downlevel-revealed lors de l'exportation du fichier en HTML, la valeur par défaut est false.

**Returns:**
boolean
### getEmbeddedFontType() {#getEmbeddedFontType--}
```
public int getEmbeddedFontType()
```


Obtient le type d'intégration du fichier de police dans le fichier html. La valeur par défaut est [HtmlEmbeddedFontType.NONE](../../com.aspose.cells/htmlembeddedfonttype\#NONE) qui indique qu'aucune police ne sera intégrée dans le html.

Voir [HtmlEmbeddedFontType](../../com.aspose.cells/htmlembeddedfonttype).

**Returns:**
int
### getEnableCssCustomProperties() {#getEnableCssCustomProperties--}
```
public boolean getEnableCssCustomProperties()
```


Optimise la sortie du html en utilisant des propriétés personnalisées CSS. Par exemple, dans le cas où une image base64 apparaît plusieurs fois, avec une propriété personnalisée les données de l'image ne doivent être enregistrées qu'une seule fois, ce qui améliore les performances du html résultant. La valeur par défaut est false.

**Returns:**
boolean
### getEncodeEntityAsCode() {#getEncodeEntityAsCode--}
```
public boolean getEncodeEntityAsCode()
```


Indique si les entités de caractères html sont remplacées par leur code décimal. (par ex. "&nbsp;" est remplacé par "&\#160;"). La valeur par défaut est false.

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Si non défini, utilise Encoding.UTF8 comme type d'encodage par défaut.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Indique si les propriétés du document sont chiffrées lors de l'enregistrement au format .xls. La valeur par défaut est true.

**Remarks**

Uniquement pour les fichiers .xls, .xlsx, .xlsb et .xlsm.

**Returns:**
boolean
### getExcludeUnusedStyles() {#getExcludeUnusedStyles--}
```
public boolean getExcludeUnusedStyles()
```


Indique si les styles inutilisés sont exclus. Pour les fichiers html générés, exclure les styles inutilisés peut réduire la taille du fichier sans affecter les effets visuels. Ainsi, la valeur par défaut de cette propriété est true. Si l'utilisateur doit conserver tous les styles dans le classeur pour le html généré (par exemple, si l'utilisateur doit restaurer le classeur à partir du html généré ultérieurement), veuillez définir cette propriété sur false.

**Returns:**
boolean
### getExportActiveWorksheetOnly() {#getExportActiveWorksheetOnly--}
```
public boolean getExportActiveWorksheetOnly()
```


Indique si seul la feuille de calcul active est exportée vers un fichier html. Si true, alors seule la feuille active sera exportée vers le fichier html ; si false, tout le classeur sera exporté vers le fichier html. La valeur par défaut est false.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


Obtient la CellArea d'exportation de la Worksheet active actuelle. Si vous définissez cet attribut, la zone d'impression de la Worksheet active actuelle sera omise. Seule la zone spécifiée sera exportée lors de l'enregistrement du fichier en html.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getExportBogusRowData() {#getExportBogusRowData--}
```
public boolean getExportBogusRowData()
```


Indique si les données de ligne inférieure factices sont exportées. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut.

**Returns:**
boolean
### getExportCellCoordinate() {#getExportCellCoordinate--}
```
public boolean getExportCellCoordinate()
```


Indique si l'exportation des coordonnées Excel des cellules non vides lors de l'enregistrement du fichier au format html. La valeur par défaut est false. Si vous souhaitez importer le html généré dans Excel, veuillez conserver la valeur par défaut.

**Returns:**
boolean
### getExportCommentsType() {#getExportCommentsType--}
```
public int getExportCommentsType()
```


Représente le type d'exportation des commentaires vers les fichiers HTML.

Voir [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Returns:**
int
### getExportDataOptions() {#getExportDataOptions--}
```
public int getExportDataOptions()
```


Indiquant la règle d'exportation des données du fichier HTML. La valeur par défaut est All.

Voir [HtmlExportDataOptions](../../com.aspose.cells/htmlexportdataoptions).

**Returns:**
int
### getExportDocumentProperties() {#getExportDocumentProperties--}
```
public boolean getExportDocumentProperties()
```


Indiquant s'il faut exporter les propriétés du document. La valeur par défaut est true. Si vous souhaitez importer le fichier HTML ou MHT dans Excel, veuillez conserver la valeur par défaut.

**Returns:**
boolean
### getExportExtraHeadings() {#getExportExtraHeadings--}
```
public boolean getExportExtraHeadings()
```


Indique si l'exportation d'en-têtes supplémentaires lorsque la longueur du texte dépasse la colonne d'affichage maximale. La valeur par défaut est false. Si vous souhaitez importer le fichier html dans Excel, veuillez conserver la valeur par défaut.

**Returns:**
boolean
### getExportFormula() {#getExportFormula--}
```
public boolean getExportFormula()
```


Indique si l'exportation des formules lors de l'enregistrement du fichier au format html. La valeur par défaut est true. Si vous souhaitez importer le html généré dans Excel, veuillez conserver la valeur par défaut.

**Returns:**
boolean
### getExportFrameScriptsAndProperties() {#getExportFrameScriptsAndProperties--}
```
public boolean getExportFrameScriptsAndProperties()
```


Indique si l'exportation des scripts de cadre et des propriétés du document. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut.

**Returns:**
boolean
### getExportGridLines() {#getExportGridLines--}
```
public boolean getExportGridLines()
```


Indique si l'exportation des quadrillages. La valeur par défaut est false.

**Returns:**
boolean
### getExportHeadings() {#getExportHeadings--}
```
public boolean getExportHeadings()
```


Indique si l'exportation des en-têtes de lignes et de colonnes de la feuille lors de l'enregistrement au format HTML.

**Remarks**

NOTE: Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété HtmlSaveOptions.ExportRowColumnHeadings. Cette propriété sera supprimée 12 mois plus tard, depuis juin 2022. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
boolean
### getExportHiddenWorksheet() {#getExportHiddenWorksheet--}
```
public boolean getExportHiddenWorksheet()
```


Indique si le contenu de la feuille de calcul masqué est exporté. La valeur par défaut est true.

**Returns:**
boolean
### getExportImagesAsBase64() {#getExportImagesAsBase64--}
```
public boolean getExportImagesAsBase64()
```


Spécifie si les images sont enregistrées au format Base64 dans HTML, MHTML ou EPUB.

**Remarks**

Lorsque cette propriété est définie sur true, les données d'image sont exportées directement dans les éléments img et aucun fichier séparé n'est créé.

**Returns:**
boolean
### getExportNamedRangeAnchors() {#getExportNamedRangeAnchors--}
```
public boolean getExportNamedRangeAnchors()
```


Indique si les éléments d'ancrage pour les plages nommées doivent être exportés lors de l'enregistrement au format HTML. La valeur par défaut est true.

**Returns:**
boolean
### getExportObjectListener() {#getExportObjectListener--}
```
public IExportObjectListener getExportObjectListener()
```


Obtient le ExportObjectListener pour l'exportation des objets.

**Remarks**

NOTE: Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété HtmlSaveOptions.IStreamProvider. Cette propriété sera supprimée 12 mois plus tard, depuis août 2015. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
[IExportObjectListener](../../com.aspose.cells/iexportobjectlistener)
### getExportPageFooters() {#getExportPageFooters--}
```
public boolean getExportPageFooters()
```


Indique si les en-têtes de page sont exportés.

**Remarks**

Ne fonctionne que lorsque [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) est True.

**Returns:**
boolean
### getExportPageHeaders() {#getExportPageHeaders--}
```
public boolean getExportPageHeaders()
```


Indique si les en-têtes de page sont exportés.

**Remarks**

Ne fonctionne que lorsque [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) est True.

**Returns:**
boolean
### getExportPrintAreaOnly() {#getExportPrintAreaOnly--}
```
public boolean getExportPrintAreaOnly()
```


Indique si seule la zone d'impression doit être exportée vers le fichier html. La valeur par défaut est false.

**Returns:**
boolean
### getExportRowColumnHeadings() {#getExportRowColumnHeadings--}
```
public boolean getExportRowColumnHeadings()
```


Indique si l'exportation des en-têtes de lignes et de colonnes de la feuille lors de l'enregistrement au format HTML.

**Remarks**

La valeur par défaut est false.

**Returns:**
boolean
### getExportSimilarBorderStyle() {#getExportSimilarBorderStyle--}
```
public boolean getExportSimilarBorderStyle()
```


Indique si l'exportation du style de bordure similaire doit être effectuée lorsque le style de bordure n'est pas pris en charge par les navigateurs. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut. La valeur par défaut est false.

**Returns:**
boolean
### getExportSingleTab() {#getExportSingleTab--}
```
public boolean getExportSingleTab()
```


Indique si l'exportation de l'onglet unique doit être effectuée lorsque le fichier ne contient qu'une seule feuille de calcul. La valeur par défaut est false.

**Returns:**
boolean
### getExportWorkbookProperties() {#getExportWorkbookProperties--}
```
public boolean getExportWorkbookProperties()
```


Indique si les propriétés du classeur sont exportées. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut.

**Returns:**
boolean
### getExportWorksheetCSSSeparately() {#getExportWorksheetCSSSeparately--}
```
public boolean getExportWorksheetCSSSeparately()
```


Indique si le CSS de la feuille de calcul est exporté séparément. La valeur par défaut est false.

**Returns:**
boolean
### getExportWorksheetProperties() {#getExportWorksheetProperties--}
```
public boolean getExportWorksheetProperties()
```


Indique si les propriétés de la feuille de calcul sont exportées. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut.

**Returns:**
boolean
### getFilePathProvider() {#getFilePathProvider--}
```
public IFilePathProvider getFilePathProvider()
```


Obtient le IFilePathProvider pour l'exportation de la feuille de calcul au format HTML séparément.

**Returns:**
[IFilePathProvider](../../com.aspose.cells/ifilepathprovider)
### getFormatDataIgnoreColumnWidth() {#getFormatDataIgnoreColumnWidth--}
```
public boolean getFormatDataIgnoreColumnWidth()
```


Indique si l'intégralité des données formatées d'une cellule doit être affichée lorsque le contenu déborde de la colonne. Si true, la largeur de la colonne est ignorée et toutes les données de la cellule sont exportées. Si false, les données sont exportées comme dans Excel. La valeur par défaut est false.

**Returns:**
boolean
### getHiddenColDisplayType() {#getHiddenColDisplayType--}
```
public int getHiddenColDisplayType()
```


Colonne masquée (la largeur de cette colonne est 0) dans Excel, avant de l'enregistrer au format HTML, si HtmlHiddenColDisplayType est "Remove", la colonne masquée ne sera pas sortie, si la valeur est "Hidden", la colonne sera sortie mais restera masquée, la valeur par défaut est "Hidden".

Voir [HtmlHiddenColDisplayType](../../com.aspose.cells/htmlhiddencoldisplaytype).

**Returns:**
int
### getHiddenRowDisplayType() {#getHiddenRowDisplayType--}
```
public int getHiddenRowDisplayType()
```


Ligne masquée (la hauteur de cette ligne est 0) dans Excel, avant de l'enregistrer au format HTML, si HtmlHiddenRowDisplayType est "Remove", la ligne masquée ne sera pas sortie, si la valeur est "Hidden", la ligne sera sortie mais restera masquée, la valeur par défaut est "Hidden".

Voir [HtmlHiddenRowDisplayType](../../com.aspose.cells/htmlhiddenrowdisplaytype).

**Returns:**
int
### getHideOverflowWrappedText() {#getHideOverflowWrappedText--}
```
public boolean getHideOverflowWrappedText()
```


Indique si le texte débordant doit être masqué lorsque le format de la cellule est défini sur retour à la ligne. La valeur par défaut est false

**Returns:**
boolean
### getHtmlCrossStringType() {#getHtmlCrossStringType--}
```
public int getHtmlCrossStringType()
```


Indique si une chaîne traversant plusieurs cellules sera affichée de la même manière que MS Excel lors de l'enregistrement d'un fichier Excel au format html. Par défaut, la valeur est Default, ainsi, pour les chaînes traversant plusieurs cellules, il y a peu de différence entre les fichiers html créés par Aspose.Cells et MS Excel. Cependant, les performances pour créer de gros fichiers html, en définissant la valeur sur Cross, seraient plusieurs fois plus rapides que de la définir sur Default ou Fit2Cell.

Voir [HtmlCrossType](../../com.aspose.cells/htmlcrosstype).

**Returns:**
int
### getHtmlVersion() {#getHtmlVersion--}
```
public int getHtmlVersion()
```


Spécifie la version de la norme HTML qui doit être utilisée lors de l'enregistrement au format HTML. La valeur par défaut est HtmlVersion.Default.

Voir [HtmlVersion](../../com.aspose.cells/htmlversion).

**Returns:**
int
### getIgnoreInvisibleShapes() {#getIgnoreInvisibleShapes--}
```
public boolean getIgnoreInvisibleShapes()
```


Indique si les formes non visibles sont exportées

**Remarks**

La valeur par défaut est false.

**Returns:**
boolean
### getImageOptions() {#getImageOptions--}
```
public ImageOrPrintOptions getImageOptions()
```


Obtenez l'objet ImageOrPrintOptions avant l'exportation

**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
### getImageScalable() {#getImageScalable--}
```
public boolean getImageScalable()
```


Indique si l'unité évolutive est utilisée pour décrire la largeur de l'image lorsqu'elle est également utilisée pour décrire la largeur de la colonne. La valeur par défaut est true.

**Returns:**
boolean
### getLayoutMode() {#getLayoutMode--}
```
public int getLayoutMode()
```


Obtient le mode de mise en page lors de l'enregistrement au format HTML. La valeur par défaut est [HtmlLayoutMode.NORMAL](../../com.aspose.cells/htmllayoutmode\#NORMAL)

Voir [HtmlLayoutMode](../../com.aspose.cells/htmllayoutmode).

**Returns:**
int
### getLinkTargetType() {#getLinkTargetType--}
```
public int getLinkTargetType()
```


Indique le type d'attribut target dans le lien `<a>`. La valeur par défaut est HtmlLinkTargetType.Parent.

Voir [HtmlLinkTargetType](../../com.aspose.cells/htmllinktargettype).

**Returns:**
int
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier.

**Remarks**

La valeur par défaut est false.

**Returns:**
boolean
### getMergeEmptyTdForcely() {#getMergeEmptyTdForcely--}
```
public boolean getMergeEmptyTdForcely()
```


Indique si la fusion des éléments TD vides est forcée lors de l'exportation du fichier en html. La taille du fichier html sera considérablement réduite après avoir défini la valeur sur true. La valeur par défaut est false. Si vous souhaitez importer le fichier html dans Excel ou exporter des lignes de grille parfaites lors de l'enregistrement du fichier en html, veuillez conserver la valeur par défaut.

**Returns:**
boolean
### getMergeEmptyTdType() {#getMergeEmptyTdType--}
```
public int getMergeEmptyTdType()
```


L'option de fusion des cellules vides contiguës (éléments td vides). La valeur par défaut est MergeEmptyTdType.Default.

Voir [MergeEmptyTdType](../../com.aspose.cells/mergeemptytdtype).

**Returns:**
int
### getOfficeMathOutputMode() {#getOfficeMathOutputMode--}
```
public int getOfficeMathOutputMode()
```


Indique comment les objets OfficeMath sont exportés en HTML, la valeur par défaut est Image.

Voir [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype).

**Returns:**
int
### getPageTitle() {#getPageTitle--}
```
public String getPageTitle()
```


Le titre de la page html. Uniquement pour l'enregistrement dans un flux html.

**Returns:**
java.lang.String
### getParseHtmlTagInCell() {#getParseHtmlTagInCell--}
```
public boolean getParseHtmlTagInCell()
```


Indique si la balise html (comme `<div></div>`) dans la cellule doit être analysée comme valeur de cellule ou conservée telle quelle. La valeur par défaut est true.

**Returns:**
boolean
### getPresentationPreference() {#getPresentationPreference--}
```
public boolean getPresentationPreference()
```


Indique si le fichier html ou mht est la préférence de présentation. La valeur par défaut est false. Si vous souhaitez obtenir une présentation plus esthétique, veuillez définir la valeur sur true.

**Returns:**
boolean
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Indique s'il faut mettre en cache les dernières données du graphique.

**Returns:**
boolean
### getSaveAsSingleFile() {#getSaveAsSingleFile--}
```
public boolean getSaveAsSingleFile()
```


Indique si le html doit être enregistré en fichier unique. La valeur par défaut est false.

**Remarks**

S'il y a plusieurs feuilles de calcul ou d'autres ressources nécessaires comme des images dans le classeur, ces feuilles et ressources doivent généralement être enregistrées dans des fichiers séparés. Dans certains scénarios, l'utilisateur peut avoir besoin d'obtenir un seul fichier résultant pour faciliter le transfert. Dans ce cas, l'utilisateur peut définir cette propriété sur true.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Obtient le format de fichier d'enregistrement.

Voir [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


Obtient les feuilles à rendre. La valeur par défaut est toutes les feuilles visibles du classeur : [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getShowAllSheets() {#getShowAllSheets--}
```
public boolean getShowAllSheets()
```


Indique si toutes les feuilles sont affichées lors de l'enregistrement en un seul fichier HTML.

**Remarks**

Ne fonctionne que lorsque [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) est True.

**Returns:**
boolean
### getSortExternalNames() {#getSortExternalNames--}
```
public boolean getSortExternalNames()
```


Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier.

**Returns:**
boolean
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


Indique s'il faut trier les noms définis avant d'enregistrer le fichier.

**Returns:**
boolean
### getSpaceMode() {#getSpaceMode--}
```
public int getSpaceMode()
```


Indique comment les espaces sont rendus dans la sortie HTML. Cette option s'applique actuellement uniquement aux formats numériques (par ex. format comptable). La valeur par défaut est [HtmlSpaceMode.CSS](../../com.aspose.cells/htmlspacemode\#CSS).

Voir [HtmlSpaceMode](../../com.aspose.cells/htmlspacemode).

**Returns:**
int
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


Obtient le IStreamProvider pour l'exportation des objets.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getTableCssId() {#getTableCssId--}
```
public String getTableCssId()
```


Obtient le préfixe du nom CSS de type tel que tr, col, td, etc., qui sont contenus dans l'élément table possédant l'attribut TableCssId spécifique. La valeur par défaut est "".

**Returns:**
java.lang.String
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


Indique si la mise à jour du paramètre smart art est activée. La valeur par défaut est false.

**Remarks**

N'affecte que après l'appel de la méthode Shape.GetResultOfSmartArt() et lorsque les formes mises en cache existent dans le fichier modèle.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier.

**Remarks**

La valeur par défaut est false.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Obtient le rappel d'avertissement.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### getWidthScalable() {#getWidthScalable--}
```
public boolean getWidthScalable()
```


Indique si la largeur des colonnes est exportée en unité d'échelle vers le html. La valeur par défaut est false.

**Returns:**
boolean
### getWorksheetScalable() {#getWorksheetScalable--}
```
public boolean getWorksheetScalable()
```


Indique si le zoom avant ou arrière du HTML via le niveau de zoom de la feuille de calcul est appliqué lors de l'enregistrement du fichier en HTML, la valeur par défaut est false.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBorderCollapsed() {#isBorderCollapsed--}
```
public boolean isBorderCollapsed()
```


Indique si les bordures du tableau sont fusionnées. La valeur par défaut est true.

**Returns:**
boolean
### isExpImageToTempDir() {#isExpImageToTempDir--}
```
public boolean isExpImageToTempDir()
```


Indique si les fichiers image sont exportés vers un répertoire temporaire. Uniquement pour l'enregistrement dans un flux html.

**Returns:**
boolean
### isExportComments() {#isExportComments--}
```
public boolean isExportComments()
```


Indique si les commentaires sont exportés lors de l'enregistrement du fichier en HTML, la valeur par défaut est false.

**Returns:**
boolean
### isFullPathLink() {#isFullPathLink--}
```
public boolean isFullPathLink()
```


Indique si l'on utilise des liens avec le chemin complet dans sheet00x.htm, filelist.xml et tabstrip.htm. La valeur par défaut est false.

**Returns:**
boolean
### isIECompatible() {#isIECompatible--}
```
public boolean isIECompatible()
```


Indique si le HTML de sortie est compatible avec le navigateur IE. La valeur par défaut est false.

**Returns:**
boolean
### isJsBrowserCompatible() {#isJsBrowserCompatible--}
```
public boolean isJsBrowserCompatible()
```


Indique si JavaScript est compatible avec les navigateurs qui ne supportent pas JavaScript. La valeur par défaut est true.

**Returns:**
boolean
### isMobileCompatible() {#isMobileCompatible--}
```
public boolean isMobileCompatible()
```


Indique si le HTML de sortie est compatible avec les appareils mobiles. La valeur par défaut est false.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAddGenericFont(boolean value) {#setAddGenericFont-boolean-}
```
public void setAddGenericFont(boolean value)
```


Indique s'il faut ajouter une police générique à la propriété CSS font-family. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAddTooltipText(boolean value) {#setAddTooltipText-boolean-}
```
public void setAddTooltipText(boolean value)
```


Indique s'il faut ajouter du texte d'infobulle lorsque les données ne peuvent pas être affichées entièrement. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAttachedFilesDirectory(String value) {#setAttachedFilesDirectory-java.lang.String-}
```
public void setAttachedFilesDirectory(String value)
```


Le répertoire où les fichiers joints seront enregistrés. Seulement pour l'enregistrement dans un flux html.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setAttachedFilesUrlPrefix(String value) {#setAttachedFilesUrlPrefix-java.lang.String-}
```
public void setAttachedFilesUrlPrefix(String value)
```


Spécifiez le préfixe Url des fichiers joints tels que les images dans le fichier html. Seulement pour l'enregistrement dans un flux html.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setBorderCollapsed(boolean value) {#setBorderCollapsed-boolean-}
```
public void setBorderCollapsed(boolean value)
```


Indique si les bordures du tableau sont fusionnées. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données.

**Remarks**

Si le dossier n'a pas été spécifié, la valeur par défaut est [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Si sa valeur par défaut est nulle ou vide, ou a été spécifiée comme nulle ou vide, aucun fichier de cache ne sera utilisé lors de l'enregistrement du classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


Indique s'il faut calculer les formules avant d'enregistrer le fichier HTML.

**Remarks**

La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCellCssPrefix(String value) {#setCellCssPrefix-java.lang.String-}
```
public void setCellCssPrefix(String value)
```


Définit le préfixe du nom CSS, la valeur par défaut est "".

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCellNameAttribute(String value) {#setCellNameAttribute-java.lang.String-}
```
public void setCellNameAttribute(String value)
```


Spécifie l'attribut qui indique le CellName à écrire. (par ex. Si la valeur est "id", alors pour la cellule "A1", la sortie sera : <td id='A1'>). La valeur par défaut est null.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Vérifie la restriction du fichier Excel lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, elle sera tronquée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


Rendre le classeur vide après l'enregistrement du fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier.

**Remarks**

La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCssStyles(String value) {#setCssStyles-java.lang.String-}
```
public void setCssStyles(String value)
```


Définit les styles CSS supplémentaires pour le formateur. Fonctionne uniquement lorsque [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) est True.  CssStyles=\"body \{ padding: 5px \}\";

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setDataBarRenderMode(int value) {#setDataBarRenderMode-int-}
```
public void setDataBarRenderMode(int value)
```


Représente le mode de rendu du DataBar lors de la conversion de fichiers Excel en fichiers html. La valeur par défaut est [DataBarRenderMode.BACKGROUND\_COLOR](../../com.aspose.cells/databarrendermode\#BACKGROUND-COLOR).

Voir [DataBarRenderMode](../../com.aspose.cells/databarrendermode).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Spécifie le nom de police par défaut pour l'exportation HTML, la police par défaut sera utilisée lorsque la police du style n'existe pas. Si cette propriété est null, Aspose.Cells utilisera une police universelle ayant la même famille que la police originale, la valeur par défaut est null.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setDisableCss(boolean value) {#setDisableCss-boolean-}
```
public void setDisableCss(boolean value)
```


Indique si seuls les styles en ligne sont appliqués, sans dépendre du CSS. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDisableDownlevelRevealedComments(boolean value) {#setDisableDownlevelRevealedComments-boolean-}
```
public void setDisableDownlevelRevealedComments(boolean value)
```


Indique s'il faut désactiver les commentaires conditionnels Downlevel-revealed lors de l'exportation du fichier en HTML, la valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEmbeddedFontType(int value) {#setEmbeddedFontType-int-}
```
public void setEmbeddedFontType(int value)
```


Définit le type d'incorporation du fichier de police dans le fichier html. La valeur par défaut est [HtmlEmbeddedFontType.NONE](../../com.aspose.cells/htmlembeddedfonttype\#NONE) qui indique qu'aucune police ne sera incorporée dans le html.

Voir [HtmlEmbeddedFontType](../../com.aspose.cells/htmlembeddedfonttype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setEnableCssCustomProperties(boolean value) {#setEnableCssCustomProperties-boolean-}
```
public void setEnableCssCustomProperties(boolean value)
```


Optimise la sortie du html en utilisant des propriétés personnalisées CSS. Par exemple, dans le cas où une image base64 apparaît plusieurs fois, avec une propriété personnalisée les données de l'image ne doivent être enregistrées qu'une seule fois, ce qui améliore les performances du html résultant. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEncodeEntityAsCode(boolean value) {#setEncodeEntityAsCode-boolean-}
```
public void setEncodeEntityAsCode(boolean value)
```


Indique si les entités de caractères html sont remplacées par leur code décimal. (par ex. "&nbsp;" est remplacé par "&\#160;"). La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Si non défini, utilise Encoding.UTF8 comme type d'encodage par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setEncryptDocumentProperties(boolean value) {#setEncryptDocumentProperties-boolean-}
```
public void setEncryptDocumentProperties(boolean value)
```


Indique si les propriétés du document sont chiffrées lors de l'enregistrement au format .xls. La valeur par défaut est true.

**Remarks**

Uniquement pour les fichiers .xls, .xlsx, .xlsb et .xlsm.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExcludeUnusedStyles(boolean value) {#setExcludeUnusedStyles-boolean-}
```
public void setExcludeUnusedStyles(boolean value)
```


Indique si les styles inutilisés sont exclus. Pour les fichiers html générés, exclure les styles inutilisés peut réduire la taille du fichier sans affecter les effets visuels. Ainsi, la valeur par défaut de cette propriété est true. Si l'utilisateur doit conserver tous les styles dans le classeur pour le html généré (par exemple, si l'utilisateur doit restaurer le classeur à partir du html généré ultérieurement), veuillez définir cette propriété sur false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExpImageToTempDir(boolean value) {#setExpImageToTempDir-boolean-}
```
public void setExpImageToTempDir(boolean value)
```


Indique si les fichiers image sont exportés vers un répertoire temporaire. Uniquement pour l'enregistrement dans un flux html.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportActiveWorksheetOnly(boolean value) {#setExportActiveWorksheetOnly-boolean-}
```
public void setExportActiveWorksheetOnly(boolean value)
```


Indique si seul la feuille de calcul active est exportée vers un fichier html. Si true, alors seule la feuille active sera exportée vers le fichier html ; si false, tout le classeur sera exporté vers le fichier html. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


Définit la zone de cellules (CellArea) à exporter de la feuille de calcul active actuelle. Si vous définissez cet attribut, la zone d'impression de la feuille active sera omise. Seule la zone spécifiée sera exportée lors de l'enregistrement du fichier en html.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportBogusRowData(boolean value) {#setExportBogusRowData-boolean-}
```
public void setExportBogusRowData(boolean value)
```


Indique si les données de ligne inférieure factices sont exportées. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportCellCoordinate(boolean value) {#setExportCellCoordinate-boolean-}
```
public void setExportCellCoordinate(boolean value)
```


Indique si l'exportation des coordonnées Excel des cellules non vides lors de l'enregistrement du fichier au format html. La valeur par défaut est false. Si vous souhaitez importer le html généré dans Excel, veuillez conserver la valeur par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportComments(boolean value) {#setExportComments-boolean-}
```
public void setExportComments(boolean value)
```


Indique si les commentaires sont exportés lors de l'enregistrement du fichier en HTML, la valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportCommentsType(int value) {#setExportCommentsType-int-}
```
public void setExportCommentsType(int value)
```


Représente le type d'exportation des commentaires vers les fichiers HTML.

Voir [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setExportDataOptions(int value) {#setExportDataOptions-int-}
```
public void setExportDataOptions(int value)
```


Indiquant la règle d'exportation des données du fichier HTML. La valeur par défaut est All.

Voir [HtmlExportDataOptions](../../com.aspose.cells/htmlexportdataoptions).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setExportDocumentProperties(boolean value) {#setExportDocumentProperties-boolean-}
```
public void setExportDocumentProperties(boolean value)
```


Indiquant s'il faut exporter les propriétés du document. La valeur par défaut est true. Si vous souhaitez importer le fichier HTML ou MHT dans Excel, veuillez conserver la valeur par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportExtraHeadings(boolean value) {#setExportExtraHeadings-boolean-}
```
public void setExportExtraHeadings(boolean value)
```


Indique si l'exportation d'en-têtes supplémentaires lorsque la longueur du texte dépasse la colonne d'affichage maximale. La valeur par défaut est false. Si vous souhaitez importer le fichier html dans Excel, veuillez conserver la valeur par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportFormula(boolean value) {#setExportFormula-boolean-}
```
public void setExportFormula(boolean value)
```


Indique si l'exportation des formules lors de l'enregistrement du fichier au format html. La valeur par défaut est true. Si vous souhaitez importer le html généré dans Excel, veuillez conserver la valeur par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportFrameScriptsAndProperties(boolean value) {#setExportFrameScriptsAndProperties-boolean-}
```
public void setExportFrameScriptsAndProperties(boolean value)
```


Indique si l'exportation des scripts de cadre et des propriétés du document. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportGridLines(boolean value) {#setExportGridLines-boolean-}
```
public void setExportGridLines(boolean value)
```


Indique si l'exportation des quadrillages. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportHeadings(boolean value) {#setExportHeadings-boolean-}
```
public void setExportHeadings(boolean value)
```


Indique si l'exportation des en-têtes de lignes et de colonnes de la feuille lors de l'enregistrement au format HTML.

**Remarks**

NOTE: Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété HtmlSaveOptions.ExportRowColumnHeadings. Cette propriété sera supprimée 12 mois plus tard, depuis juin 2022. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportHiddenWorksheet(boolean value) {#setExportHiddenWorksheet-boolean-}
```
public void setExportHiddenWorksheet(boolean value)
```


Indique si le contenu de la feuille de calcul masqué est exporté. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportImagesAsBase64(boolean value) {#setExportImagesAsBase64-boolean-}
```
public void setExportImagesAsBase64(boolean value)
```


Spécifie si les images sont enregistrées au format Base64 dans HTML, MHTML ou EPUB.

**Remarks**

Lorsque cette propriété est définie sur true, les données d'image sont exportées directement dans les éléments img et aucun fichier séparé n'est créé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportNamedRangeAnchors(boolean value) {#setExportNamedRangeAnchors-boolean-}
```
public void setExportNamedRangeAnchors(boolean value)
```


Indique si les éléments d'ancrage pour les plages nommées doivent être exportés lors de l'enregistrement au format HTML. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportObjectListener(IExportObjectListener value) {#setExportObjectListener-com.aspose.cells.IExportObjectListener-}
```
public void setExportObjectListener(IExportObjectListener value)
```


Définit le ExportObjectListener pour l'exportation des objets.

**Remarks**

NOTE: Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété HtmlSaveOptions.IStreamProvider. Cette propriété sera supprimée 12 mois plus tard, depuis août 2015. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [IExportObjectListener](../../com.aspose.cells/iexportobjectlistener) |  |

### setExportPageFooters(boolean value) {#setExportPageFooters-boolean-}
```
public void setExportPageFooters(boolean value)
```


Indique si les en-têtes de page sont exportés.

**Remarks**

Ne fonctionne que lorsque [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) est True.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportPageHeaders(boolean value) {#setExportPageHeaders-boolean-}
```
public void setExportPageHeaders(boolean value)
```


Indique si les en-têtes de page sont exportés.

**Remarks**

Ne fonctionne que lorsque [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) est True.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportPrintAreaOnly(boolean value) {#setExportPrintAreaOnly-boolean-}
```
public void setExportPrintAreaOnly(boolean value)
```


Indique si seule la zone d'impression doit être exportée vers le fichier html. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportRowColumnHeadings(boolean value) {#setExportRowColumnHeadings-boolean-}
```
public void setExportRowColumnHeadings(boolean value)
```


Indique si l'exportation des en-têtes de lignes et de colonnes de la feuille lors de l'enregistrement au format HTML.

**Remarks**

La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportSimilarBorderStyle(boolean value) {#setExportSimilarBorderStyle-boolean-}
```
public void setExportSimilarBorderStyle(boolean value)
```


Indique si l'exportation du style de bordure similaire doit être effectuée lorsque le style de bordure n'est pas pris en charge par les navigateurs. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportSingleTab(boolean value) {#setExportSingleTab-boolean-}
```
public void setExportSingleTab(boolean value)
```


Indique si l'exportation de l'onglet unique doit être effectuée lorsque le fichier ne contient qu'une seule feuille de calcul. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportWorkbookProperties(boolean value) {#setExportWorkbookProperties-boolean-}
```
public void setExportWorkbookProperties(boolean value)
```


Indique si les propriétés du classeur sont exportées. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportWorksheetCSSSeparately(boolean value) {#setExportWorksheetCSSSeparately-boolean-}
```
public void setExportWorksheetCSSSeparately(boolean value)
```


Indique si le CSS de la feuille de calcul est exporté séparément. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExportWorksheetProperties(boolean value) {#setExportWorksheetProperties-boolean-}
```
public void setExportWorksheetProperties(boolean value)
```


Indique si les propriétés de la feuille de calcul sont exportées. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFilePathProvider(IFilePathProvider value) {#setFilePathProvider-com.aspose.cells.IFilePathProvider-}
```
public void setFilePathProvider(IFilePathProvider value)
```


Définit le IFilePathProvider pour exporter la Worksheet en html séparément.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [IFilePathProvider](../../com.aspose.cells/ifilepathprovider) |  |

### setFormatDataIgnoreColumnWidth(boolean value) {#setFormatDataIgnoreColumnWidth-boolean-}
```
public void setFormatDataIgnoreColumnWidth(boolean value)
```


Indique si l'intégralité des données formatées d'une cellule doit être affichée lorsque le contenu déborde de la colonne. Si true, la largeur de la colonne est ignorée et toutes les données de la cellule sont exportées. Si false, les données sont exportées comme dans Excel. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFullPathLink(boolean value) {#setFullPathLink-boolean-}
```
public void setFullPathLink(boolean value)
```


Indique si l'on utilise des liens avec le chemin complet dans sheet00x.htm, filelist.xml et tabstrip.htm. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHiddenColDisplayType(int value) {#setHiddenColDisplayType-int-}
```
public void setHiddenColDisplayType(int value)
```


Colonne masquée (la largeur de cette colonne est 0) dans Excel, avant de l'enregistrer au format HTML, si HtmlHiddenColDisplayType est "Remove", la colonne masquée ne sera pas sortie, si la valeur est "Hidden", la colonne sera sortie mais restera masquée, la valeur par défaut est "Hidden".

Voir [HtmlHiddenColDisplayType](../../com.aspose.cells/htmlhiddencoldisplaytype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setHiddenRowDisplayType(int value) {#setHiddenRowDisplayType-int-}
```
public void setHiddenRowDisplayType(int value)
```


Ligne masquée (la hauteur de cette ligne est 0) dans Excel, avant de l'enregistrer au format HTML, si HtmlHiddenRowDisplayType est "Remove", la ligne masquée ne sera pas sortie, si la valeur est "Hidden", la ligne sera sortie mais restera masquée, la valeur par défaut est "Hidden".

Voir [HtmlHiddenRowDisplayType](../../com.aspose.cells/htmlhiddenrowdisplaytype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setHideOverflowWrappedText(boolean value) {#setHideOverflowWrappedText-boolean-}
```
public void setHideOverflowWrappedText(boolean value)
```


Indique si le texte débordant doit être masqué lorsque le format de la cellule est défini sur retour à la ligne. La valeur par défaut est false

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHtmlCrossStringType(int value) {#setHtmlCrossStringType-int-}
```
public void setHtmlCrossStringType(int value)
```


Indique si une chaîne traversant plusieurs cellules sera affichée de la même manière que MS Excel lors de l'enregistrement d'un fichier Excel au format html. Par défaut, la valeur est Default, ainsi, pour les chaînes traversant plusieurs cellules, il y a peu de différence entre les fichiers html créés par Aspose.Cells et MS Excel. Cependant, les performances pour créer de gros fichiers html, en définissant la valeur sur Cross, seraient plusieurs fois plus rapides que de la définir sur Default ou Fit2Cell.

Voir [HtmlCrossType](../../com.aspose.cells/htmlcrosstype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setHtmlVersion(int value) {#setHtmlVersion-int-}
```
public void setHtmlVersion(int value)
```


Spécifie la version de la norme HTML qui doit être utilisée lors de l'enregistrement au format HTML. La valeur par défaut est HtmlVersion.Default.

Voir [HtmlVersion](../../com.aspose.cells/htmlversion).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setIECompatible(boolean value) {#setIECompatible-boolean-}
```
public void setIECompatible(boolean value)
```


Indique si le HTML de sortie est compatible avec le navigateur IE. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setIgnoreInvisibleShapes(boolean value) {#setIgnoreInvisibleShapes-boolean-}
```
public void setIgnoreInvisibleShapes(boolean value)
```


Indique si les formes non visibles sont exportées

**Remarks**

La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setImageScalable(boolean value) {#setImageScalable-boolean-}
```
public void setImageScalable(boolean value)
```


Indique si l'unité évolutive est utilisée pour décrire la largeur de l'image lorsqu'elle est également utilisée pour décrire la largeur de la colonne. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setJsBrowserCompatible(boolean value) {#setJsBrowserCompatible-boolean-}
```
public void setJsBrowserCompatible(boolean value)
```


Indique si JavaScript est compatible avec les navigateurs qui ne supportent pas JavaScript. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setLayoutMode(int value) {#setLayoutMode-int-}
```
public void setLayoutMode(int value)
```


Définit le mode de mise en page lors de l'enregistrement en HTML. La valeur par défaut est [HtmlLayoutMode.NORMAL](../../com.aspose.cells/htmllayoutmode\#NORMAL)

Voir [HtmlLayoutMode](../../com.aspose.cells/htmllayoutmode).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setLinkTargetType(int value) {#setLinkTargetType-int-}
```
public void setLinkTargetType(int value)
```


Indique le type d'attribut target dans le lien `<a>`. La valeur par défaut est HtmlLinkTargetType.Parent.

Voir [HtmlLinkTargetType](../../com.aspose.cells/htmllinktargettype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier.

**Remarks**

La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setMergeEmptyTdForcely(boolean value) {#setMergeEmptyTdForcely-boolean-}
```
public void setMergeEmptyTdForcely(boolean value)
```


Indique si la fusion des éléments TD vides est forcée lors de l'exportation du fichier en html. La taille du fichier html sera considérablement réduite après avoir défini la valeur sur true. La valeur par défaut est false. Si vous souhaitez importer le fichier html dans Excel ou exporter des lignes de grille parfaites lors de l'enregistrement du fichier en html, veuillez conserver la valeur par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setMergeEmptyTdType(int value) {#setMergeEmptyTdType-int-}
```
public void setMergeEmptyTdType(int value)
```


L'option de fusion des cellules vides contiguës (éléments td vides). La valeur par défaut est MergeEmptyTdType.Default.

Voir [MergeEmptyTdType](../../com.aspose.cells/mergeemptytdtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setMobileCompatible(boolean value) {#setMobileCompatible-boolean-}
```
public void setMobileCompatible(boolean value)
```


Indique si le HTML de sortie est compatible avec les appareils mobiles. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setOfficeMathOutputMode(int value) {#setOfficeMathOutputMode-int-}
```
public void setOfficeMathOutputMode(int value)
```


Indique comment les objets OfficeMath sont exportés en HTML, la valeur par défaut est Image.

Voir [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPageTitle(String value) {#setPageTitle-java.lang.String-}
```
public void setPageTitle(String value)
```


Le titre de la page html. Uniquement pour l'enregistrement dans un flux html.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setParseHtmlTagInCell(boolean value) {#setParseHtmlTagInCell-boolean-}
```
public void setParseHtmlTagInCell(boolean value)
```


Indique si la balise html (comme `<div></div>`) dans la cellule doit être analysée comme valeur de cellule ou conservée telle quelle. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPresentationPreference(boolean value) {#setPresentationPreference-boolean-}
```
public void setPresentationPreference(boolean value)
```


Indique si le fichier html ou mht est la préférence de présentation. La valeur par défaut est false. Si vous souhaitez obtenir une présentation plus esthétique, veuillez définir la valeur sur true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Indique s'il faut mettre en cache les dernières données du graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSaveAsSingleFile(boolean value) {#setSaveAsSingleFile-boolean-}
```
public void setSaveAsSingleFile(boolean value)
```


Indique si le html doit être enregistré en fichier unique. La valeur par défaut est false.

**Remarks**

S'il y a plusieurs feuilles de calcul ou d'autres ressources nécessaires comme des images dans le classeur, ces feuilles et ressources doivent généralement être enregistrées dans des fichiers séparés. Dans certains scénarios, l'utilisateur peut avoir besoin d'obtenir un seul fichier résultant pour faciliter le transfert. Dans ce cas, l'utilisateur peut définir cette propriété sur true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


Définit les feuilles à rendre. La valeur par défaut est toutes les feuilles visibles du classeur : [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

### setShowAllSheets(boolean value) {#setShowAllSheets-boolean-}
```
public void setShowAllSheets(boolean value)
```


Indique si toutes les feuilles sont affichées lors de l'enregistrement en un seul fichier HTML.

**Remarks**

Ne fonctionne que lorsque [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) est True.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


Indique s'il faut trier les noms définis avant d'enregistrer le fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSpaceMode(int value) {#setSpaceMode-int-}
```
public void setSpaceMode(int value)
```


Indique comment les espaces sont rendus dans la sortie HTML. Cette option s'applique actuellement uniquement aux formats numériques (par ex. format comptable). La valeur par défaut est [HtmlSpaceMode.CSS](../../com.aspose.cells/htmlspacemode\#CSS).

Voir [HtmlSpaceMode](../../com.aspose.cells/htmlspacemode).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


Définit le IStreamProvider pour l'exportation des objets.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setTableCssId(String value) {#setTableCssId-java.lang.String-}
```
public void setTableCssId(String value)
```


Définit le préfixe du nom CSS de type tel que tr, col, td, etc., ils sont contenus dans l'élément table qui possède l'attribut TableCssId spécifique. La valeur par défaut est "".

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


Indique si la mise à jour du paramètre smart art est activée. La valeur par défaut est false.

**Remarks**

N'affecte que après l'appel de la méthode Shape.GetResultOfSmartArt() et lorsque les formes mises en cache existent dans le fichier modèle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier.

**Remarks**

La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Définit le rappel d’avertissement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

### setWidthScalable(boolean value) {#setWidthScalable-boolean-}
```
public void setWidthScalable(boolean value)
```


Indique si la largeur des colonnes est exportée en unité d'échelle vers le html. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setWorksheetScalable(boolean value) {#setWorksheetScalable-boolean-}
```
public void setWorksheetScalable(boolean value)
```


Indique si le zoom avant ou arrière du HTML via le niveau de zoom de la feuille de calcul est appliqué lors de l'enregistrement du fichier en HTML, la valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

