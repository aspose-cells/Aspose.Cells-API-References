---
title: "GridWebBean"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente le bean java GridWeb"
type: docs
url: /fr/java/com.aspose.gridweb/gridwebbean/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.WebControl](../../com.aspose.gridweb/webcontrol), [com.aspose.gridweb.ExtWebControl](../../com.aspose.gridweb/extwebcontrol), [com.aspose.gridweb.MainWeb](../../com.aspose.gridweb/mainweb)
```
public class GridWebBean extends MainWeb
```

Représente le bean java GridWeb
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [GridWebBean()](#GridWebBean--) | le constructeur par défaut de GridWebBean |
## Champs

| Champ | Description |
| --- | --- |
| [AfterColumnFilter](#AfterColumnFilter) | Se produit après le filtrage de la colonne. |
| [AjaxCallFinished](#AjaxCallFinished) | Se déclenche lorsque la mise à jour ajax du contrôle est terminée. |
| [BeforeColumnFilter](#BeforeColumnFilter) | Se produit avant que la colonne ne soit filtrée. |
| [CellClickOnAjax](#CellClickOnAjax) | Se produit lorsque la cellule est cliquée, et nécessite un rappel ajax pour cet événement. |
| [CellClientUpdate](#CellClientUpdate) | Se produit lorsqu'une mise à jour de cellule côté client a lieu. |
| [CellCommand](#CellCommand) | Se produit lorsque le lien hypertexte de commande d'une cellule est cliqué. |
| [CellDoubleClick](#CellDoubleClick) | Se produit lorsque la cellule est double-cliquée. |
| [CellModifiedOnAjax](#CellModifiedOnAjax) | Se produit lorsque la cellule est modifiée lors d'un appel ajax. |
| [ColumnDeleted](#ColumnDeleted) | Se produit lorsque l'utilisateur supprime une colonne du menu côté client. |
| [ColumnDeleting](#ColumnDeleting) | Se produit lorsque l'utilisateur tente de supprimer une colonne du menu côté client. |
| [ColumnDoubleClick](#ColumnDoubleClick) | Se produit lorsque l'en-tête de colonne est double-cliqué. |
| [ColumnInserted](#ColumnInserted) | Se produit lorsque l'utilisateur insère une colonne depuis le menu côté client. |
| [CustomCommand](#CustomCommand) | Se produit lorsque l'utilisateur clique sur un bouton de commande personnalisé. |
| [LoadCustomData](#LoadCustomData) | Se déclenche lorsque le SessionMode du contrôle est défini sur Custom et doit charger les données de la feuille. |
| [PageIndexChanged](#PageIndexChanged) | Se produit lorsque l'index de page de la feuille du contrôle a changé. |
| [RowDeleted](#RowDeleted) | Se produit lorsque l'utilisateur a supprimé une ligne depuis le menu côté client. |
| [RowDeleting](#RowDeleting) | Se produit lorsque l'utilisateur essaie de supprimer une ligne depuis le menu côté client. |
| [RowDoubleClick](#RowDoubleClick) | Se produit lorsque l'en-tête de ligne est double-cliqué. |
| [RowInserted](#RowInserted) | Se produit lorsque l'utilisateur insère une ligne depuis le menu côté client. |
| [SaveCommand](#SaveCommand) | Se produit lorsque le bouton "save" est cliqué. |
| [SheetAdded](#SheetAdded) | Se produit lorsque l'utilisateur ajoute une feuille de calcul depuis le menu de la barre d'outils. |
| [SheetTabClick](#SheetTabClick) | Se produit lorsque l'onglet de la feuille est cliqué. |
| [SubmitCommand](#SubmitCommand) | Se produit lorsque le bouton "submit" est cliqué. |
| [UndoCommand](#UndoCommand) | Se produit lorsque le bouton "undo" est cliqué. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [calculateFormula()](#calculateFormula--) | Calcule le résultat des formules. |
| [createChildControls()](#createChildControls--) | Implémente CreateChildControls depuis WebControl, utilisé uniquement en interne. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getACWClientPath()](#getACWClientPath--) | Obtient le chemin web des fichiers script/image du contrôle. |
| [getACWLanguageFileUrl()](#getACWLanguageFileUrl--) | Obtient l'URL web du fichier de langue du contrôle. |
| [getActiveCell()](#getActiveCell--) | Obtient la cellule active de la feuille actuelle. |
| [getActiveCellBgColor()](#getActiveCellBgColor--) | Spécifie la couleur d'arrière-plan de la cellule active. |
| [getActiveCellColor()](#getActiveCellColor--) | Spécifie la couleur de la cellule active. |
| [getActiveHeaderBgColor()](#getActiveHeaderBgColor--) | Spécifie la couleur d'arrière-plan de l'en-tête de ligne/colonne active. |
| [getActiveHeaderColor()](#getActiveHeaderColor--) | Spécifie la couleur de l'en-tête de ligne/colonne active. |
| [getActiveSheet()](#getActiveSheet--) | Obtient la feuille active |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | Obtient l'index de la feuille active. |
| [getActiveTabStyle()](#getActiveTabStyle--) | Spécifie le style de l'onglet actif. |
| [getAutoRefreshChart()](#getAutoRefreshChart--) | Obtient le style de la barre inférieure du contrôle. |
| [getBackColor()](#getBackColor--) | Obtient le BackColor dans le WebControl |
| [getBeanID()](#getBeanID--) | obtenir l'id html du bean |
| [getBorderColor()](#getBorderColor--) | Obtient le BorderColor dans le WebControl |
| [getBorderStyle()](#getBorderStyle--) | Obtient le BorderStyle dans le WebControl |
| [getBorderWidth()](#getBorderWidth--) | Obtient le BorderWidth dans le WebControl |
| [getBottomTableStyle()](#getBottomTableStyle--) | Obtient l'index de la page actuelle en mode pagination. |
| [getClass()](#getClass--) |  |
| [getCssClass()](#getCssClass--) | Obtient le CssClass dans le WebControl |
| [getCurrentPageIndex()](#getCurrentPageIndex--) | Obtient l'index de page actuel en mode pagination. |
| [getCustomCalculationEngine()](#getCustomCalculationEngine--) | Représente le moteur de calcul personnalisé de l'utilisateur pour étendre le moteur de calcul par défaut d'Aspose.Cells. |
| [getCustomCommandButtons()](#getCustomCommandButtons--) | Obtient la collection de boutons de commande personnalisés |
| [getCustomStyleFileName()](#getCustomStyleFileName--) | Obtient le nom du fichier de style personnalisé. |
| [getDPI()](#getDPI--) | Obtient / Définit le DPI de la machine. |
| [getDefaultFontName()](#getDefaultFontName--) | Obtient le nom de police par défaut du contrôle. |
| [getDefaultFontSize()](#getDefaultFontSize--) | Obtient la taille de police par défaut du contrôle. |
| [getDefaultGridLineColor()](#getDefaultGridLineColor--) | Obtient la couleur de la ligne de grille par défaut. |
| [getDisplayCellTip()](#getDisplayCellTip--) | Obtient si les astuces doivent être affichées. la valeur par défaut est true. |
| [getEditMode()](#getEditMode--) | Obtient le mode d'édition du contrôle. |
| [getEnableAJAX()](#getEnableAJAX--) | Obtient si l'appel AJAX doit être utilisé. la valeur par défaut est true. |
| [getEnableAsync()](#getEnableAsync--) | Obtient si les données des cellules sont chargées de manière asynchrone, suggéré de l'appliquer pour une feuille contenant plus de 10000 cellules. |
| [getEnableClientColumnOperations()](#getEnableClientColumnOperations--) | Obtient si les opérations de colonne côté client sont activées. |
| [getEnableClientFreeze()](#getEnableClientFreeze--) | Obtient si les opérations de gel côté client sont activées. |
| [getEnableClientMergeOperations()](#getEnableClientMergeOperations--) | Obtient si les opérations de fusion côté client sont activées. |
| [getEnableClientResizeColumnRow()](#getEnableClientResizeColumnRow--) | Obtient si le redimensionnement des colonnes et des lignes côté client est activé. |
| [getEnableClientRowOperations()](#getEnableClientRowOperations--) | Obtient si les opérations de ligne côté client sont activées. |
| [getEnableDoubleClickEvent()](#getEnableDoubleClickEvent--) | Obtient si l'événement double-clic côté client est activé. |
| [getEnableMetalLightEffect()](#getEnableMetalLightEffect--) | Obtient si l'effet de lumière métallique est appliqué. |
| [getEnablePaging()](#getEnablePaging--) | Obtient si le mode de pagination du contrôle est activé. |
| [getEnableStyleDialogbox()](#getEnableStyleDialogbox--) | Obtient si la boîte de dialogue de style côté client est activée. |
| [getEnabled()](#getEnabled--) | Obtient le Enabled dans le WebControl |
| [getFilteredPaging()](#getFilteredPaging--) | Obtient si la pagination après filtrage des données est activée, prendra effet lorsque EnablePaging est true. |
| [getFont()](#getFont--) | Obtient le Font dans le WebControl |
| [getForceValidation()](#getForceValidation--) | Obtient si la validation côté client est forcée. |
| [getForeColor()](#getForeColor--) | Obtient le ForeColor dans le WebControl |
| [getFrameTableStyle()](#getFrameTableStyle--) | Obtient le style de cadre du contrôle. |
| [getGoonDefaultSaveOperation()](#getGoonDefaultSaveOperation--) | Obtient si GridWeb effectuera l'opération d'enregistrement par défaut, la valeur par défaut est true. |
| [getHTMLBody()](#getHTMLBody--) | le code html du bean pour le corps html, il doit être obtenu après l'appel des méthodes init et prepareRender |
| [getHTMLHead()](#getHTMLHead--) | le code html du bean pour l'en-tête html, il doit être obtenu après l'appel de la méthode init et prepareRender |
| [getHeaderBarHeight()](#getHeaderBarHeight--) | Obtient la hauteur (System.Web.UI.WebControl.Unit) de la barre d'en-tête supérieure du contrôle. |
| [getHeaderBarStyle()](#getHeaderBarStyle--) | Obtient le style de la barre d'en-tête. |
| [getHeaderBarTableStyle()](#getHeaderBarTableStyle--) | Obtient le style de la barre d'en-tête du contrôle. |
| [getHeaderBarWidth()](#getHeaderBarWidth--) | Obtient la largeur( System.Web.UI.WebControl.Unit ) ou la barre d'en-tête gauche du contrôle. |
| [getHeight()](#getHeight--) | Obtient la hauteur( System.Web.UI.WebControl.Unit ) du contrôle. |
| [getIgnoreStyleWithNoData()](#getIgnoreStyleWithNoData--) | Obtient si GridWeb ignore l'affichage des lignes ou des colonnes qui ne contiennent pas de valeurs de cellule mais qui sont toujours stylisées. |
| [getLoadOptions()](#getLoadOptions--) | Représente les options de chargement pour GridWeb. |
| [getMaxColumn()](#getMaxColumn--) | Obtient l'index de colonne d'affichage maximal (base zéro) de la feuille Web. |
| [getMaxRow()](#getMaxRow--) | Obtient l'index de ligne d'affichage maximal (base zéro) de la feuille Web. |
| [getMessage()](#getMessage--) | Obtient le message pour la grille. |
| [getMinColumn()](#getMinColumn--) | Obtient l'index de colonne d'affichage minimal (base zéro) de la feuille Web. |
| [getMinRow()](#getMinRow--) | Obtient l'index de ligne d'affichage minimal (base zéro) de la feuille Web. |
| [getModifiedCells()](#getModifiedCells--) | Obtient la collection des cellules modifiées par le client. |
| [getNeedRenderGroupRows()](#getNeedRenderGroupRows--) | Obtient si afficher les grouprows. |
| [getNoHScroll()](#getNoHScroll--) | Obtient une valeur indiquant si la barre de défilement horizontale est masquée. |
| [getNoScroll()](#getNoScroll--) | Obtient si la barre de défilement doit être affichée. |
| [getNoVScroll()](#getNoVScroll--) | Obtient une valeur indiquant si la barre de défilement verticale est masquée. |
| [getOnAjaxCallFinishedClientFunction()](#getOnAjaxCallFinishedClientFunction--) | Obtient le nom de la fonction côté client à appeler lorsque l'appel ajax est terminé. |
| [getOnCellErrorClientFunction()](#getOnCellErrorClientFunction--) | Obtient le nom de la fonction côté client à appeler lorsqu'une validation de cellule échoue. |
| [getOnCellSelectedAjaxCallBackClientFunction()](#getOnCellSelectedAjaxCallBackClientFunction--) | Obtient la fonction côté client à appeler lorsqu'une cellule est sélectionnée. |
| [getOnCellSelectedClientFunction()](#getOnCellSelectedClientFunction--) | Obtient la fonction côté client à appeler lorsqu'une cellule est sélectionnée. |
| [getOnCellUnselectedClientFunction()](#getOnCellUnselectedClientFunction--) | Obtient la fonction côté client à appeler lorsqu'une cellule est désélectionnée. |
| [getOnCellUpdatedClientFunction()](#getOnCellUpdatedClientFunction--) | Obtient le nom de la fonction côté client à appeler lorsqu'une valeur de cellule est mise à jour. |
| [getOnContextMenuShowClientFunction()](#getOnContextMenuShowClientFunction--) | Obtient la fonction côté client à appeler lorsque le menu contextuel sera affiché. |
| [getOnDoubleClickCellClientFunction()](#getOnDoubleClickCellClientFunction--) | Obtient la fonction côté client à appeler lorsqu'une cellule est double-cliquée. |
| [getOnDoubleClickRowClientFunction()](#getOnDoubleClickRowClientFunction--) | Obtient la fonction côté client à appeler lorsqu'une ligne est double-cliquée. |
| [getOnGridInitClientFunction()](#getOnGridInitClientFunction--) | Obtient le nom de la fonction côté client à appeler lorsque la grille est initialisée. |
| [getOnPageChangeClientFunction()](#getOnPageChangeClientFunction--) | Obtient la fonction côté client à appeler après le changement d'index de page. Ne prend effet que lorsque EnablePaging est vrai. |
| [getOnPageSubmitClientFunction()](#getOnPageSubmitClientFunction--) | Obtient la fonction client à appeler avant que la page ne soit soumise côté client. |
| [getOnShapeSelectedClientFunction()](#getOnShapeSelectedClientFunction--) | Obtient la fonction côté client à appeler lorsqu'une forme est sélectionnée. |
| [getOnSubmitClientFunction()](#getOnSubmitClientFunction--) | Obtient la fonction client à appeler avant que le contrôle ne soit soumis côté client. |
| [getOnlyAuto()](#getOnlyAuto--) | Obtient si seules les lignes dont la hauteur n'est pas personnalisée sont ajustées, la valeur par défaut est false. |
| [getPageSize()](#getPageSize--) | Obtient la taille de la page en mode pagination. |
| [getPictureCachePath()](#getPictureCachePath--) | Obtient le chemin de stockage des images pour le classeur, toutes les formes et images seront stockées dans ce répertoire, le chemin par défaut est acwcache sous le répertoire de base de l'application actuelle ; les utilisateurs doivent implémenter un service planifié pour nettoyer les fichiers dont le temps de session est expiré. |
| [getPresetStyle()](#getPresetStyle--) | Obtient le style prédéfini. |
| [getRefreshValidation()](#getRefreshValidation--) | Obtient si la valeur de validation doit être rafraîchie après la modification de la valeur de la cellule. |
| [getRenderHiddenRow()](#getRenderHiddenRow--) | Obtient si la ligne masquée est rendue dans GridControl, la valeur par défaut est false. |
| [getRowHeightForCSV()](#getRowHeightForCSV--) | Obtient la valeur de hauteur de ligne en points pour le fichier csv, la valeur par défaut est 14,5. |
| [getScrollBarArrowColor()](#getScrollBarArrowColor--) | Spécifie la couleur du bouton flèche de la barre de défilement. |
| [getScrollBarBaseColor()](#getScrollBarBaseColor--) | Spécifie la couleur de la barre de défilement du contrôle. |
| [getSelectCellBgColor()](#getSelectCellBgColor--) | Spécifie la couleur d'arrière-plan des cellules sélectionnées dans une plage de sélection multiple. |
| [getSelectCellColor()](#getSelectCellColor--) | Spécifie la couleur des cellules sélectionnées dans une plage de sélection multiple. |
| [getSessionStorePath()](#getSessionStorePath--) | Obtient le chemin de stockage du cache de session lorsque le mode de session est File ou ViewState, etc : gridweb.SessionStorePath="c:/mytempdir/session"; alors les données de session seront stockées dans c:/mytempdir/session |
| [getSettings()](#getSettings--) | Représente les paramètres du classeur. |
| [getShowAddButton()](#getShowAddButton--) | Obtient si le bouton d'ajout de feuille de calcul doit être affiché. |
| [getShowBottomBar()](#getShowBottomBar--) | Spécifie si la barre de commande (incluant la barre de commande et la barre d'onglets) doit être affichée en bas du contrôle. |
| [getShowCellEditBox()](#getShowCellEditBox--) | Indique si Gridweb affiche la barre d'outils de la zone de saisie comme dans MS-EXCEL. Si activé, une zone de saisie pour la cellule actuelle sera affichée dans Gridweb. |
| [getShowCommandBarAtTop()](#getShowCommandBarAtTop--) | Spécifie si la barre de commande (incluant la barre de commande et la barre d'onglets) doit être affichée en haut du contrôle. |
| [getShowContextMenu()](#getShowContextMenu--) | Obtient si le menu contextuel doit être affiché. La valeur par défaut est true. |
| [getShowDefaultGridLine()](#getShowDefaultGridLine--) | Obtient si les lignes de grille par défaut des cellules doivent être affichées. |
| [getShowHeaderBar()](#getShowHeaderBar--) | Obtient si la barre d'en-tête doit être affichée |
| [getShowLoading()](#getShowLoading--) | Spécifie si une boîte de dialogue de chargement doit être affichée pendant le postback vers le serveur. |
| [getShowLoadingPosition()](#getShowLoadingPosition--) | Spécifie la position gauche, haut (en px) pour afficher la boîte de dialogue de chargement pendant le postback vers le serveur, etc. 100,200 signifie que la position gauche, haut de la boîte de dialogue de chargement est à 100 px,200 px. |
| [getShowSaveButton()](#getShowSaveButton--) | Obtient si le bouton d'enregistrement doit être affiché. |
| [getShowSubmitButton()](#getShowSubmitButton--) | Obtient si le bouton de soumission doit être affiché. |
| [getShowTabBar()](#getShowTabBar--) | Obtient si la barre d'onglets doit être affichée. |
| [getShowTabNavigation()](#getShowTabNavigation--) | Obtient si le bouton de navigation des onglets est affiché, la valeur par défaut est true. |
| [getShowUndoButton()](#getShowUndoButton--) | Obtient si le bouton d'annulation doit être affiché. |
| [getSpanWrap()](#getSpanWrap--) | Spécifie si le contenu doit être enveloppé dans la portée de cellule, la valeur par défaut est true. |
| [getTabIndex()](#getTabIndex--) | Obtient le TabIndex dans le WebControl |
| [getTabStyle()](#getTabStyle--) | Obtient le style de la barre d'onglets. |
| [getToolTip()](#getToolTip--) | Obtient le ToolTip dans le WebControl |
| [getUseClientPageHeight()](#getUseClientPageHeight--) | Obtient si GridWeb utilise la hauteur de la page client comme hauteur du contrôle, adapté lorsque Height="100%" est défini, la valeur par défaut est false. |
| [getViewPanelScrollLeft()](#getViewPanelScrollLeft--) | Obtient la position de la barre de défilement du panneau de vue de la grille. |
| [getViewPanelScrollTop()](#getViewPanelScrollTop--) | Obtient la position de la barre de défilement du panneau de vue de la grille. |
| [getViewTableStyle()](#getViewTableStyle--) | Obtient le style du panneau de vue des données. |
| [getWidth()](#getWidth--) | Obtient la largeur (System.Web.UI.WebControl.Unit) du contrôle. |
| [getWorkSheets()](#getWorkSheets--) | Obtient la collection des feuilles de calcul. |
| [getXhtmlMode()](#getXhtmlMode--) | Obtient si le style XHTML doit être utilisé, la valeur par défaut est true. |
| [hashCode()](#hashCode--) |  |
| [importExcelFile(InputStream stream)](#importExcelFile-java.io.InputStream-) | Importe depuis un flux de fichier Excel, y compris le flux de fichier disque ou le flux mémoire. |
| [importExcelFile(InputStream stream, String passwordtoOpen)](#importExcelFile-java.io.InputStream-java.lang.String-) | Importe depuis un flux de fichier Excel, y compris le flux de fichier disque ou le flux mémoire. |
| [importExcelFile(String fileName)](#importExcelFile-java.lang.String-) | Importe depuis un fichier Excel. |
| [importExcelFile(String fileName, String passwordtoOpen)](#importExcelFile-java.lang.String-java.lang.String-) | Importe depuis un fichier Excel. |
| [init()](#init--) | le bean doit être initialisé par la requête et la réponse du servlet de la page actuelle |
| [isCalculateFormula()](#isCalculateFormula--) | Obtient si la formule doit être calculée après les changements de valeur de cellule ou après l'importation du fichier. |
| [loadCSVFile(InputStream stream)](#loadCSVFile-java.io.InputStream-) | Charge les données depuis un flux de fichier CSV. |
| [loadCSVFile(String fileName)](#loadCSVFile-java.lang.String-) | Charge les données depuis un fichier CSV. |
| [loadHTMLFile(InputStream stream)](#loadHTMLFile-java.io.InputStream-) | Charge les données depuis un flux de fichier HTML. |
| [loadHTMLFile(String fileName)](#loadHTMLFile-java.lang.String-) | Charge les données depuis un fichier HTML. |
| [loadSpreadSheetMLFile(InputStream stream)](#loadSpreadSheetMLFile-java.io.InputStream-) | Charge les données depuis un flux de fichier SpreadSheetML. |
| [loadSpreadSheetMLFile(String fileName)](#loadSpreadSheetMLFile-java.lang.String-) | Charge les données depuis un fichier SpreadSheetML. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [prepareRender()](#prepareRender--) | la méthode doit être appelée avant le rendu du bean GridWeb |
| [refreshChartShape()](#refreshChartShape--) | Actualise toutes les images de graphiques pour la feuille de calcul active. |
| [saveCSVFile(OutputStream stream)](#saveCSVFile-java.io.OutputStream-) | Enregistre les données dans un flux de fichier CSV. |
| [saveCSVFile(String targetFile)](#saveCSVFile-java.lang.String-) | Enregistre les données dans un fichier CSV. |
| [saveCustomStyleFile(String fileName)](#saveCustomStyleFile-java.lang.String-) | Enregistre les données de style actuelles du contrôle dans un fichier XML. |
| [saveHTMLFile(OutputStream stream)](#saveHTMLFile-java.io.OutputStream-) | Enregistre les données dans un flux de fichier HTML. |
| [saveHTMLFile(String targetFile)](#saveHTMLFile-java.lang.String-) | Enregistre les données dans un fichier HTML. |
| [saveSpreadSheetMLFile(OutputStream stream)](#saveSpreadSheetMLFile-java.io.OutputStream-) | Enregistre les données dans un flux de fichier SpreadSheetML. |
| [saveSpreadSheetMLFile(String targetFile)](#saveSpreadSheetMLFile-java.lang.String-) | Enregistre les données dans un fichier SpreadSheetML. |
| [saveToExcelFile(OutputStream stream)](#saveToExcelFile-java.io.OutputStream-) | Enregistre les feuilles de calcul dans un fichier Excel. |
| [saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions)](#saveToExcelFile-java.io.OutputStream-com.aspose.gridweb.GridSaveOptions-) | Enregistre les feuilles de calcul dans un fichier Excel. |
| [saveToExcelFile(OutputStream stream, int format)](#saveToExcelFile-java.io.OutputStream-int-) | Enregistre les feuilles de calcul dans un fichier Excel. |
| [saveToExcelFile(String targetFile)](#saveToExcelFile-java.lang.String-) | Enregistre les feuilles de calcul dans un fichier Excel au format Excel 2003. |
| [saveToExcelFile(String targetFile, GridSaveOptions saveOptions)](#saveToExcelFile-java.lang.String-com.aspose.gridweb.GridSaveOptions-) | Enregistre les feuilles de calcul dans un fichier Excel. |
| [saveToExcelFile(String targetFile, int format)](#saveToExcelFile-java.lang.String-int-) | Enregistre les feuilles de calcul dans un fichier Excel. |
| [setACWClientPath(String value)](#setACWClientPath-java.lang.String-) | Définit le chemin web des fichiers script/image du contrôle. |
| [setACWLanguageFileUrl(String value)](#setACWLanguageFileUrl-java.lang.String-) | Définit l'URL web du fichier de langue du contrôle. |
| [setActiveCell(GridCell value)](#setActiveCell-com.aspose.gridweb.GridCell-) | Définit la cellule active de la feuille actuelle. |
| [setActiveCellBgColor(Color value)](#setActiveCellBgColor-com.aspose.gridweb.Color-) | Spécifie la couleur d'arrière-plan de la cellule active. |
| [setActiveCellColor(Color value)](#setActiveCellColor-com.aspose.gridweb.Color-) | Spécifie la couleur de la cellule active. |
| [setActiveHeaderBgColor(Color value)](#setActiveHeaderBgColor-com.aspose.gridweb.Color-) | Spécifie la couleur d'arrière-plan de l'en-tête de ligne/colonne active. |
| [setActiveHeaderColor(Color value)](#setActiveHeaderColor-com.aspose.gridweb.Color-) | Spécifie la couleur de l'en-tête de ligne/colonne active. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | Définit l'index de la feuille active. |
| [setActiveTabStyle(GridTableItemStyle value)](#setActiveTabStyle-com.aspose.gridweb.GridTableItemStyle-) | Spécifie le style de l'onglet actif. |
| [setAutoRefreshChart(boolean value)](#setAutoRefreshChart-boolean-) | Définit si l'image du graphique est mise à jour lors de la mise à jour de la valeur de la cellule. La valeur par défaut est true. |
| [setBackColor(Color value)](#setBackColor-com.aspose.gridweb.Color-) | Définit le BackColor dans le WebControl |
| [setBeanID(String beanID)](#setBeanID-java.lang.String-) | définir l'id html du bean |
| [setBorderColor(Color value)](#setBorderColor-com.aspose.gridweb.Color-) | Définit le BorderColor dans le WebControl |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Définit le BorderStyle dans le WebControl |
| [setBorderWidth(Unit value)](#setBorderWidth-com.aspose.gridweb.Unit-) | Définit le BorderWidth dans le WebControl |
| [setBottomTableStyle(GridTableStyle value)](#setBottomTableStyle-com.aspose.gridweb.GridTableStyle-) | Définit le style de la barre inférieure du contrôle. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Définit s'il faut calculer la formule après les changements de valeur de cellule ou après l'importation du fichier. |
| [setCssClass(String value)](#setCssClass-java.lang.String-) | Définit le CssClass dans le WebControl |
| [setCurrentPageIndex(int value)](#setCurrentPageIndex-int-) | Définit l'index de la page actuelle en mode pagination. |
| [setCustomCalculationEngine(GridAbstractCalculationEngine value)](#setCustomCalculationEngine-com.aspose.gridweb.GridAbstractCalculationEngine-) | Représente le moteur de calcul personnalisé de l'utilisateur pour étendre le moteur de calcul par défaut d'Aspose.Cells. |
| [setCustomStyle(InputStream stream)](#setCustomStyle-java.io.InputStream-) | Définit le fichier de style personnalisé à partir d'un flux, y compris le flux de fichier disque ou le flux mémoire. |
| [setCustomStyleFileName(String value)](#setCustomStyleFileName-java.lang.String-) | Définit le nom du fichier de style personnalisé. |
| [setDPI(double value)](#setDPI-double-) | Obtient / Définit le DPI de la machine. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Définit le nom de police par défaut du contrôle. |
| [setDefaultFontSize(FontUnit value)](#setDefaultFontSize-com.aspose.gridweb.FontUnit-) | Définit la taille de police par défaut du contrôle. |
| [setDefaultGridLineColor(Color value)](#setDefaultGridLineColor-com.aspose.gridweb.Color-) | Définit la couleur par défaut des lignes de la grille. |
| [setDisplayCellTip(boolean value)](#setDisplayCellTip-boolean-) | Définit s'il faut afficher les astuces. La valeur par défaut est true. |
| [setEditMode(boolean value)](#setEditMode-boolean-) | Définit le mode d'édition du contrôle. |
| [setEnableAJAX(boolean value)](#setEnableAJAX-boolean-) | Définit s'il faut utiliser l'appel AJAX. La valeur par défaut est true. |
| [setEnableAsync(boolean value)](#setEnableAsync-boolean-) | Définit s'il faut charger les données des cellules de manière asynchrone, recommandé pour une feuille contenant plus de 10 000 cellules. |
| [setEnableClientColumnOperations(boolean value)](#setEnableClientColumnOperations-boolean-) | Définit s'il faut activer les opérations de colonne côté client. |
| [setEnableClientFreeze(boolean value)](#setEnableClientFreeze-boolean-) | Définit s'il faut activer les opérations de gel côté client. |
| [setEnableClientMergeOperations(boolean value)](#setEnableClientMergeOperations-boolean-) | Définit s'il faut activer les opérations de fusion côté client. |
| [setEnableClientResizeColumnRow(boolean value)](#setEnableClientResizeColumnRow-boolean-) | Définit si l'agrandissement des colonnes et des lignes côté client est activé. |
| [setEnableClientRowOperations(boolean value)](#setEnableClientRowOperations-boolean-) | Définit si les opérations de ligne côté client sont activées. |
| [setEnableDoubleClickEvent(boolean value)](#setEnableDoubleClickEvent-boolean-) | Définit si l'événement double-clic côté client est activé. |
| [setEnableMetalLightEffect(boolean value)](#setEnableMetalLightEffect-boolean-) | Définit si l'effet de lumière métallique doit être appliqué. |
| [setEnablePaging(boolean value)](#setEnablePaging-boolean-) | Définit si le mode de pagination du contrôle est activé. |
| [setEnableStyleDialogbox(boolean value)](#setEnableStyleDialogbox-boolean-) | Définit si la boîte de dialogue de style côté client est activée. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Définit le Enabled dans le WebControl |
| [setFilteredPaging(boolean value)](#setFilteredPaging-boolean-) | Définit si la pagination après filtrage des données est activée, prendra effet lorsque EnablePaging est vrai. |
| [setForceValidation(boolean value)](#setForceValidation-boolean-) | Définit si la validation côté client doit être forcée. |
| [setForeColor(Color value)](#setForeColor-com.aspose.gridweb.Color-) | Définit le ForeColor dans le WebControl |
| [setFrameTableStyle(GridTableStyle value)](#setFrameTableStyle-com.aspose.gridweb.GridTableStyle-) | Définit le style du cadre du contrôle. |
| [setGoonDefaultSaveOperation(boolean value)](#setGoonDefaultSaveOperation-boolean-) | Définit si GridWeb effectuera l'opération d'enregistrement par défaut, la valeur par défaut est vraie. |
| [setHeaderBarHeight(Unit value)](#setHeaderBarHeight-com.aspose.gridweb.Unit-) | Définit la hauteur (System.Web.UI.WebControl.Unit) de la barre d'en-tête supérieure du contrôle. |
| [setHeaderBarStyle(GridTableItemStyle value)](#setHeaderBarStyle-com.aspose.gridweb.GridTableItemStyle-) | Définit le style de la barre d'en-tête. |
| [setHeaderBarTableStyle(GridTableStyle value)](#setHeaderBarTableStyle-com.aspose.gridweb.GridTableStyle-) | Définit le style de la barre d'en-tête du contrôle. |
| [setHeaderBarWidth(Unit value)](#setHeaderBarWidth-com.aspose.gridweb.Unit-) | Définit la largeur (System.Web.UI.WebControl.Unit) de la barre d'en-tête gauche du contrôle. |
| [setHeight(Unit value)](#setHeight-com.aspose.gridweb.Unit-) | Définit la hauteur (System.Web.UI.WebControl.Unit) du contrôle. |
| [setIgnoreStyleWithNoData(boolean value)](#setIgnoreStyleWithNoData-boolean-) | Définit si GridWeb ignore l'affichage des lignes ou colonnes qui ne contiennent pas de valeurs de cellule mais qui sont toujours stylisées. |
| [setLoadOptions(GridLoadOptions value)](#setLoadOptions-com.aspose.gridweb.GridLoadOptions-) | Représente les options de chargement pour GridWeb. |
| [setMaxColumn(int value)](#setMaxColumn-int-) | Définit l'index maximal de colonne affichée (base zéro) de la feuille Web. |
| [setMaxRow(int value)](#setMaxRow-int-) | Définit l'index maximal de ligne affichée (base zéro) de la feuille Web. |
| [setMessage(String value)](#setMessage-java.lang.String-) | Définit le message pour la grille. |
| [setMinColumn(int value)](#setMinColumn-int-) | Définit l'index minimal de colonne affichée (base zéro) de la feuille Web. |
| [setMinRow(int value)](#setMinRow-int-) | Définit l'index minimal de ligne affichée (base zéro) de la feuille Web. |
| [setNeedRenderGroupRows(boolean value)](#setNeedRenderGroupRows-boolean-) | Définit si les lignes de groupe doivent être affichées. |
| [setNoHScroll(boolean value)](#setNoHScroll-boolean-) | Définit une valeur indiquant si la barre de défilement horizontale est masquée. |
| [setNoScroll(boolean value)](#setNoScroll-boolean-) | Définit si la barre de défilement doit être affichée. |
| [setNoVScroll(boolean value)](#setNoVScroll-boolean-) | Définit une valeur indiquant si la barre de défilement verticale est masquée. |
| [setOnAjaxCallFinishedClientFunction(String value)](#setOnAjaxCallFinishedClientFunction-java.lang.String-) | Définit le nom de la fonction côté client à appeler lorsque l'appel ajax est terminé. |
| [setOnCellErrorClientFunction(String value)](#setOnCellErrorClientFunction-java.lang.String-) | Définit le nom de la fonction côté client à appeler lorsqu'une validation de cellule échoue. |
| [setOnCellSelectedAjaxCallBackClientFunction(String value)](#setOnCellSelectedAjaxCallBackClientFunction-java.lang.String-) | Définit la fonction côté client à appeler lorsqu'une cellule est sélectionnée. |
| [setOnCellSelectedClientFunction(String value)](#setOnCellSelectedClientFunction-java.lang.String-) | Définit la fonction côté client à appeler lorsqu'une cellule est sélectionnée. |
| [setOnCellUnselectedClientFunction(String value)](#setOnCellUnselectedClientFunction-java.lang.String-) | Définit la fonction côté client à appeler lorsqu'une cellule est désélectionnée. |
| [setOnCellUpdatedClientFunction(String value)](#setOnCellUpdatedClientFunction-java.lang.String-) | Définit le nom de la fonction côté client à appeler lorsque la valeur d'une cellule est mise à jour. |
| [setOnContextMenuShowClientFunction(String value)](#setOnContextMenuShowClientFunction-java.lang.String-) | Définit la fonction côté client à appeler lorsque le menu contextuel sera affiché. |
| [setOnDoubleClickCellClientFunction(String value)](#setOnDoubleClickCellClientFunction-java.lang.String-) | Définit la fonction côté client à appeler lorsqu'une cellule est double-cliquée. |
| [setOnDoubleClickRowClientFunction(String value)](#setOnDoubleClickRowClientFunction-java.lang.String-) | Définit la fonction côté client à appeler lorsqu'une ligne est double-cliquée. |
| [setOnGridInitClientFunction(String value)](#setOnGridInitClientFunction-java.lang.String-) | Définit le nom de la fonction côté client à appeler lorsque la grille est initialisée. |
| [setOnPageChangeClientFunction(String value)](#setOnPageChangeClientFunction-java.lang.String-) | Définit la fonction côté client à appeler après le changement d'index de page. Ne prend effet que lorsque EnablePaging est vrai. |
| [setOnPageSubmitClientFunction(String value)](#setOnPageSubmitClientFunction-java.lang.String-) | Définit la fonction client à appeler avant que la page ne soit soumise côté client. |
| [setOnShapeSelectedClientFunction(String value)](#setOnShapeSelectedClientFunction-java.lang.String-) | Définit la fonction côté client à appeler lorsqu'une forme est sélectionnée. |
| [setOnSubmitClientFunction(String value)](#setOnSubmitClientFunction-java.lang.String-) | Définit la fonction client à appeler avant que le contrôle ne soit soumis côté client. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Définit si seules les lignes dont la hauteur n'est pas personnalisée doivent être ajustées, la valeur par défaut est false. |
| [setPageSize(int value)](#setPageSize-int-) | Définit la taille de page en mode pagination. |
| [setPictureCachePath(String value)](#setPictureCachePath-java.lang.String-) | Définit le chemin de stockage des images pour le classeur, toutes les formes et images seront stockées dans ce répertoire, le chemin par défaut est acwcache sous le répertoire de base de l'application actuelle. Les utilisateurs doivent implémenter un service planifié pour nettoyer les fichiers dont le délai de session est expiré. |
| [setPresetStyle(int value)](#setPresetStyle-int-) | Définit le style prédéfini. |
| [setRefreshValidation(boolean value)](#setRefreshValidation-boolean-) | Définit s'il faut rafraîchir la valeur de validation après que la valeur de la cellule a changé. |
| [setRenderHiddenRow(boolean value)](#setRenderHiddenRow-boolean-) | Définit si la ligne masquée est rendue dans GridControl, la valeur par défaut est false. |
| [setRowHeightForCSV(double value)](#setRowHeightForCSV-double-) | Définit la valeur de hauteur de ligne en points pour le fichier csv, la valeur par défaut est 14,5. |
| [setScrollBarArrowColor(Color value)](#setScrollBarArrowColor-com.aspose.gridweb.Color-) | Spécifie la couleur du bouton flèche de la barre de défilement. |
| [setScrollBarBaseColor(Color value)](#setScrollBarBaseColor-com.aspose.gridweb.Color-) | Spécifie la couleur de la barre de défilement du contrôle. |
| [setSelectCellBgColor(Color value)](#setSelectCellBgColor-com.aspose.gridweb.Color-) | Spécifie la couleur d'arrière-plan des cellules sélectionnées dans une plage de sélection multiple. |
| [setSelectCellColor(Color value)](#setSelectCellColor-com.aspose.gridweb.Color-) | Spécifie la couleur des cellules sélectionnées dans une plage de sélection multiple. |
| [setSessionStorePath(String value)](#setSessionStorePath-java.lang.String-) | Définit le chemin de stockage du cache de session lorsque le mode de session est File ou ViewState, etc. : gridweb.SessionStorePath="c:/mytempdir/session"; il stockera alors les données de session dans c:/mytempdir/session. |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridweb.GridWorkbookSettings-) | Représente les paramètres du classeur. |
| [setShowAddButton(boolean value)](#setShowAddButton-boolean-) | Définit s'il faut afficher le bouton d'ajout de feuille de calcul. |
| [setShowBottomBar(boolean value)](#setShowBottomBar-boolean-) | Spécifie si la barre de commande (incluant la barre de commande et la barre d'onglets) doit être affichée en bas du contrôle. |
| [setShowCellEditBox(boolean value)](#setShowCellEditBox-boolean-) | Indique si Gridweb affiche la barre d'outils de la zone de saisie comme dans MS-EXCEL. Si activé, une zone de saisie pour la cellule actuelle sera affichée dans Gridweb. |
| [setShowCommandBarAtTop(boolean value)](#setShowCommandBarAtTop-boolean-) | Spécifie si la barre de commande (incluant la barre de commande et la barre d'onglets) doit être affichée en haut du contrôle. |
| [setShowContextMenu(boolean value)](#setShowContextMenu-boolean-) | Définit s'il faut afficher le menu contextuel. La valeur par défaut est true. |
| [setShowDefaultGridLine(boolean value)](#setShowDefaultGridLine-boolean-) | Définit s'il faut afficher les lignes de grille par défaut des cellules. |
| [setShowHeaderBar(boolean value)](#setShowHeaderBar-boolean-) | Définit s'il faut afficher la barre d'en-tête |
| [setShowLoading(boolean value)](#setShowLoading-boolean-) | Spécifie si une boîte de dialogue de chargement doit être affichée pendant le postback vers le serveur. |
| [setShowLoadingPosition(String value)](#setShowLoadingPosition-java.lang.String-) | Spécifie la position gauche, haut (en px) pour afficher la boîte de dialogue de chargement pendant le postback vers le serveur, etc. 100,200 signifie que la position gauche, haut de la boîte de dialogue de chargement est à 100 px,200 px. |
| [setShowSaveButton(boolean value)](#setShowSaveButton-boolean-) | Définit si le bouton d'enregistrement doit être affiché. |
| [setShowSubmitButton(boolean value)](#setShowSubmitButton-boolean-) | Définit si le bouton de soumission doit être affiché. |
| [setShowTabBar(boolean value)](#setShowTabBar-boolean-) | Définit si la barre d'onglets doit être affichée. |
| [setShowTabNavigation(boolean value)](#setShowTabNavigation-boolean-) | Définit si le bouton de navigation des onglets est affiché, la valeur par défaut est true. |
| [setShowUndoButton(boolean value)](#setShowUndoButton-boolean-) | Définit si le bouton d'annulation doit être affiché. |
| [setSpanWrap(boolean value)](#setSpanWrap-boolean-) | Spécifie si le contenu doit être enveloppé dans la portée de cellule, la valeur par défaut est true. |
| [setTabIndex(short value)](#setTabIndex-short-) | Définit le TabIndex dans le WebControl |
| [setTabStyle(GridTableItemStyle value)](#setTabStyle-com.aspose.gridweb.GridTableItemStyle-) | Définit le style de la barre d'onglets. |
| [setToolTip(String value)](#setToolTip-java.lang.String-) | Définit le ToolTip dans le WebControl |
| [setUseClientPageHeight(boolean value)](#setUseClientPageHeight-boolean-) | Définit si GridWeb utilise la hauteur de la page client comme hauteur du contrôle, adapté lorsque la propriété Height=\"100%\" est définie, la valeur par défaut est false. |
| [setViewPanelScrollLeft(String value)](#setViewPanelScrollLeft-java.lang.String-) | Définit la position de la barre de défilement du panneau de visualisation de la grille. |
| [setViewPanelScrollTop(String value)](#setViewPanelScrollTop-java.lang.String-) | Définit la position de la barre de défilement du panneau de visualisation de la grille. |
| [setViewTableStyle(GridTableStyle value)](#setViewTableStyle-com.aspose.gridweb.GridTableStyle-) | Définit le style du panneau de visualisation des données. |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Définit la largeur (System.Web.UI.WebControl.Unit) du contrôle. |
| [setXhtmlMode(boolean value)](#setXhtmlMode-boolean-) | Définit si le style XHTML doit être utilisé, la valeur par défaut est true. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWebBean() {#GridWebBean--}
```
public GridWebBean()
```


le constructeur par défaut de GridWebBean

### AfterColumnFilter {#AfterColumnFilter}
```
public RowColumnEventHandler AfterColumnFilter
```


Se produit après le filtrage de la colonne.

### AjaxCallFinished {#AjaxCallFinished}
```
public WorkbookEventHandler AjaxCallFinished
```


Se déclenche lorsque la mise à jour ajax du contrôle est terminée (EnableAJAX doit être défini sur true).

### BeforeColumnFilter {#BeforeColumnFilter}
```
public RowColumnEventHandler BeforeColumnFilter
```


Se produit avant que la colonne ne soit filtrée.

### CellClickOnAjax {#CellClickOnAjax}
```
public CellEventStringHandler CellClickOnAjax
```


Se produit lorsque la cellule est cliquée, et nécessite un rappel ajax pour cet événement.

### CellClientUpdate {#CellClientUpdate}
```
public CellEventHandler CellClientUpdate
```


Se produit lorsqu'une mise à jour d'une cellule client se produit. Lorsque cet événement est déclenché, son paramètre e.Argument contient le nom de la commande.

### CellCommand {#CellCommand}
```
public CellEventHandler CellCommand
```


Se produit lorsqu'un hyperlien de commande d'une cellule est cliqué. Lorsque cet événement est déclenché, son paramètre e.Argument contient le nom de la commande.

### CellDoubleClick {#CellDoubleClick}
```
public CellEventHandler CellDoubleClick
```


Se produit lorsque la cellule est double-cliquée.

### CellModifiedOnAjax {#CellModifiedOnAjax}
```
public CellEventHandler CellModifiedOnAjax
```


Se produit lorsque la cellule est modifiée lors d'un appel ajax.

### ColumnDeleted {#ColumnDeleted}
```
public RowColumnEventHandler ColumnDeleted
```


Se produit lorsque l'utilisateur supprime une colonne du menu côté client.

### ColumnDeleting {#ColumnDeleting}
```
public RowColumnEventHandler ColumnDeleting
```


Se produit lorsqu'un utilisateur tente de supprimer une colonne depuis le menu côté client. Vous pouvez gérer cet événement et définir le paramètre cancel sur True pour annuler l'opération de suppression.

### ColumnDoubleClick {#ColumnDoubleClick}
```
public RowColumnEventHandler ColumnDoubleClick
```


Se produit lorsque l'en-tête de colonne est double-cliqué.

### ColumnInserted {#ColumnInserted}
```
public RowColumnEventHandler ColumnInserted
```


Se produit lorsque l'utilisateur insère une colonne depuis le menu côté client.

### CustomCommand {#CustomCommand}
```
public CustomCommandEventHandler CustomCommand
```


Se produit lorsque l'utilisateur clique sur un bouton de commande personnalisé.

### LoadCustomData {#LoadCustomData}
```
public WorkbookEventHandler LoadCustomData
```


Se déclenche lorsque le SessionMode du contrôle est défini sur Custom et doit charger les données de la feuille. Vous pouvez gérer cet événement en mode Session personnalisée pour charger les données de la feuille depuis un fichier ou une base de données.

### PageIndexChanged {#PageIndexChanged}
```
public WorkbookEventHandler PageIndexChanged
```


Se produit lorsque l'index de page de la feuille du contrôle a changé.

### RowDeleted {#RowDeleted}
```
public RowColumnEventHandler RowDeleted
```


Se produit lorsque l'utilisateur a supprimé une ligne depuis le menu côté client.

### RowDeleting {#RowDeleting}
```
public RowColumnEventHandler RowDeleting
```


Se produit lorsqu'un utilisateur tente de supprimer une ligne depuis le menu côté client. Vous pouvez gérer cet événement et lancer une exception RejectDeleteException pour annuler l'opération de suppression.

### RowDoubleClick {#RowDoubleClick}
```
public RowColumnEventHandler RowDoubleClick
```


Se produit lorsque l'en-tête de ligne est double-cliqué.

### RowInserted {#RowInserted}
```
public RowColumnEventHandler RowInserted
```


Se produit lorsque l'utilisateur insère une ligne depuis le menu côté client.

### SaveCommand {#SaveCommand}
```
public WorkbookEventHandler SaveCommand
```


Se produit lorsque le bouton "save" est cliqué.

### SheetAdded {#SheetAdded}
```
public SheetEventHandler SheetAdded
```


Se produit lorsque l'utilisateur ajoute une feuille de calcul depuis le menu de la barre d'outils.

### SheetTabClick {#SheetTabClick}
```
public WorkbookEventHandler SheetTabClick
```


Se produit lorsque l'onglet de la feuille est cliqué.

### SubmitCommand {#SubmitCommand}
```
public WorkbookEventHandler SubmitCommand
```


Se produit lorsque le bouton "submit" est cliqué.

### UndoCommand {#UndoCommand}
```
public WorkbookEventHandler UndoCommand
```


Se produit lorsque le bouton "undo" est cliqué.

### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


Calcule le résultat des formules.

### createChildControls() {#createChildControls--}
```
public void createChildControls()
```


Implémente CreateChildControls depuis WebControl, utilisé uniquement en interne.

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
### getACWClientPath() {#getACWClientPath--}
```
public String getACWClientPath()
```


Obtient le chemin web des fichiers script/image du contrôle. Par exemple : \"http://localhost/acw\\_client\". Vous pouvez également définir cette valeur dans le fichier web.config. Ajoutez cette section à la section `<configuration>` :
`<appSettings>`
`<add key=\"aspose.cells.gridweb.acw_client_path\" value=\"/acw_client/\" />`
`</appSettings>`


**Returns:**
java.lang.String
### getACWLanguageFileUrl() {#getACWLanguageFileUrl--}
```
public String getACWLanguageFileUrl()
```


Obtient l'URL web du fichier de langue du contrôle. Par exemple : \"/acw\\_client/lang\\_en.js\".
Par défaut, un fichier anglais intégré est utilisé.


**Returns:**
java.lang.String
### getActiveCell() {#getActiveCell--}
```
public GridCell getActiveCell()
```


Obtient la cellule active de la feuille actuelle. Modifiée pour être modifiable depuis la version 1.9.0.1.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getActiveCellBgColor() {#getActiveCellBgColor--}
```
public Color getActiveCellBgColor()
```


Spécifie la couleur d'arrière-plan de la cellule active.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveCellColor() {#getActiveCellColor--}
```
public Color getActiveCellColor()
```


Spécifie la couleur de la cellule active.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveHeaderBgColor() {#getActiveHeaderBgColor--}
```
public Color getActiveHeaderBgColor()
```


Spécifie la couleur d'arrière-plan de l'en-tête de ligne/colonne active.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveHeaderColor() {#getActiveHeaderColor--}
```
public Color getActiveHeaderColor()
```


Spécifie la couleur de l'en-tête de ligne/colonne active.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveSheet() {#getActiveSheet--}
```
public GridWorksheet getActiveSheet()
```


Obtient la feuille active

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet)
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


Obtient l'index de la feuille active. Égal à WebWorksheets.ActiveSheetIndex.

**Returns:**
int
### getActiveTabStyle() {#getActiveTabStyle--}
```
public GridTableItemStyle getActiveTabStyle()
```


Spécifie le style de l'onglet actif.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getAutoRefreshChart() {#getAutoRefreshChart--}
```
public boolean getAutoRefreshChart()
```


Obtient le style de la barre inférieure du contrôle.

**Returns:**
boolean
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


Obtient le BackColor dans le WebControl

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBeanID() {#getBeanID--}
```
public String getBeanID()
```


obtenir l'id html du bean

**Returns:**
java.lang.String
### getBorderColor() {#getBorderColor--}
```
public Color getBorderColor()
```


Obtient le BorderColor dans le WebControl

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Obtient le BorderStyle dans le WebControl

Voir [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Returns:**
int
### getBorderWidth() {#getBorderWidth--}
```
public Unit getBorderWidth()
```


Obtient le BorderWidth dans le WebControl

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getBottomTableStyle() {#getBottomTableStyle--}
```
public GridTableStyle getBottomTableStyle()
```


Obtient l'index de la page actuelle en mode pagination.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCssClass() {#getCssClass--}
```
public String getCssClass()
```


Obtient le CssClass dans le WebControl

**Returns:**
java.lang.String
### getCurrentPageIndex() {#getCurrentPageIndex--}
```
public int getCurrentPageIndex()
```


Obtient l'index de page actuel en mode pagination.

**Remarks**

En mode pagination, le contrôle affichera une fois PageSize lignes de données, et affichera le contrôle de sélection de page dans la barre d'onglets.

**Returns:**
int
### getCustomCalculationEngine() {#getCustomCalculationEngine--}
```
public GridAbstractCalculationEngine getCustomCalculationEngine()
```


Représente le moteur de calcul personnalisé de l'utilisateur pour étendre le moteur de calcul par défaut d'Aspose.Cells.

**Returns:**
[GridAbstractCalculationEngine](../../com.aspose.gridweb/gridabstractcalculationengine)
### getCustomCommandButtons() {#getCustomCommandButtons--}
```
public CustomCommandButtonCollection getCustomCommandButtons()
```


Obtient la collection de boutons de commande personnalisés

**Returns:**
[CustomCommandButtonCollection](../../com.aspose.gridweb/customcommandbuttoncollection)
### getCustomStyleFileName() {#getCustomStyleFileName--}
```
public String getCustomStyleFileName()
```


Obtient le nom du fichier de style personnalisé.

**Remarks**

Le fichier de style personnalisé est un fichier XML. Lorsque le nom du fichier est défini, le fichier sera chargé immédiatement. Voici le contenu du "style prédéfini standard" ------------------------------------------------------- <Aspose.Cells.GridWeb.ViewerStyleTemplate runat="server" HeaderBarWidth="30pt" ScrollBarBaseColor="" FrameTableStyle-BorderStyle="Solid" FrameTableStyle-LeftBorderStyle-BorderWidth="" FrameTableStyle-LeftBorderStyle-BorderColor="" FrameTableStyle-RightBorderStyle-BorderWidth="" FrameTableStyle-RightBorderStyle-BorderColor="" FrameTableStyle-BorderWidth="1px" FrameTableStyle-CellSpacing="0" FrameTableStyle-BorderColor="Gray" FrameTableStyle-CellPadding="0" FrameTableStyle-TopBorderStyle-BorderWidth="" FrameTableStyle-TopBorderStyle-BorderColor="" FrameTableStyle-BottomBorderStyle-BorderWidth="" FrameTableStyle-BottomBorderStyle-BorderColor="" HeaderBarStyle-LeftBorderStyle-BorderStyle="Solid" HeaderBarStyle-LeftBorderStyle-BorderWidth="1px" HeaderBarStyle-LeftBorderStyle-BorderColor="White" HeaderBarStyle-VerticalAlign="Middle" HeaderBarStyle-RightBorderStyle-BorderStyle="Solid" HeaderBarStyle-RightBorderStyle-BorderWidth="1px" HeaderBarStyle-RightBorderStyle-BorderColor="Gray" HeaderBarStyle-BorderWidth="1px" HeaderBarStyle-Font-Size="10pt" HeaderBarStyle-BorderColor="Gray" HeaderBarStyle-BorderStyle="Solid" HeaderBarStyle-HorizontalAlign="Center" HeaderBarStyle-ForeColor="Black" HeaderBarStyle-TopBorderStyle-BorderStyle="Solid" HeaderBarStyle-TopBorderStyle-BorderWidth="1px" HeaderBarStyle-TopBorderStyle-BorderColor="White" HeaderBarStyle-BackColor="\#E0E0E0" HeaderBarStyle-BottomBorderStyle-BorderStyle="Solid" HeaderBarStyle-BottomBorderStyle-BorderWidth="1px" HeaderBarStyle-BottomBorderStyle-BorderColor="Gray" ViewTableStyle-LeftBorderStyle-BorderWidth="" ViewTableStyle-LeftBorderStyle-BorderColor="" ViewTableStyle-LayoutFixed="Fixed" ViewTableStyle-RightBorderStyle-BorderWidth="" ViewTableStyle-RightBorderStyle-BorderColor="" ViewTableStyle-BorderWidth="0px" ViewTableStyle-CellSpacing="0" ViewTableStyle-CellPadding="0" ViewTableStyle-TopBorderStyle-BorderWidth="" ViewTableStyle-TopBorderStyle-BorderColor="" ViewTableStyle-BottomBorderStyle-BorderWidth="" ViewTableStyle-BottomBorderStyle-BorderColor="" BottomTableStyle-LeftBorderStyle-BorderWidth="" BottomTableStyle-LeftBorderStyle-BorderColor="" BottomTableStyle-LayoutFixed="Fixed" BottomTableStyle-RightBorderStyle-BorderWidth="" BottomTableStyle-RightBorderStyle-BorderColor="" BottomTableStyle-BorderWidth="0px" BottomTableStyle-CellSpacing="0" BottomTableStyle-CellPadding="1" BottomTableStyle-TopBorderStyle-BorderStyle="Solid" BottomTableStyle-TopBorderStyle-BorderWidth="1px" BottomTableStyle-TopBorderStyle-BorderColor="Gray" BottomTableStyle-BottomBorderStyle-BorderWidth="" BottomTableStyle-BottomBorderStyle-BorderColor="" HeaderBarHeight="15pt" ActiveTabStyle-LeftBorderStyle-BorderWidth="" ActiveTabStyle-LeftBorderStyle-BorderColor="" ActiveTabStyle-RightBorderStyle-BorderWidth="" ActiveTabStyle-RightBorderStyle-BorderColor="" ActiveTabStyle-Height="15pt" ActiveTabStyle-BorderWidth="1px" ActiveTabStyle-Font-Size="10pt" ActiveTabStyle-BorderColor="Gray" ActiveTabStyle-ForeColor="Black" ActiveTabStyle-TopBorderStyle-BorderWidth="" ActiveTabStyle-TopBorderStyle-BorderColor="" ActiveTabStyle-BackColor="White" ActiveTabStyle-BottomBorderStyle-BorderWidth="" ActiveTabStyle-BottomBorderStyle-BorderColor="" HeaderBarTableStyle-LeftBorderStyle-BorderWidth="" HeaderBarTableStyle-LeftBorderStyle-BorderColor="" HeaderBarTableStyle-LayoutFixed="Fixed" HeaderBarTableStyle-RightBorderStyle-BorderWidth="" HeaderBarTableStyle-RightBorderStyle-BorderColor="" HeaderBarTableStyle-BorderWidth="0px" HeaderBarTableStyle-CellSpacing="0" HeaderBarTableStyle-BorderCollapse="Separate" HeaderBarTableStyle-CellPadding="0" HeaderBarTableStyle-TopBorderStyle-BorderWidth="" HeaderBarTableStyle-TopBorderStyle-BorderColor="" HeaderBarTableStyle-BottomBorderStyle-BorderWidth="" HeaderBarTableStyle-BottomBorderStyle-BorderColor="" TabStyle-LeftBorderStyle-BorderWidth="" TabStyle-LeftBorderStyle-BorderColor="" TabStyle-RightBorderStyle-BorderWidth="" TabStyle-RightBorderStyle-BorderColor="" TabStyle-Height="15pt" TabStyle-BorderWidth="1px" TabStyle-Font-Size="10pt" TabStyle-BorderColor="Gray" TabStyle-ForeColor="Black" TabStyle-TopBorderStyle-BorderWidth="" TabStyle-TopBorderStyle-BorderColor="" TabStyle-BackColor="\#E0E0E0" TabStyle-BottomBorderStyle-BorderWidth="" TabStyle-BottomBorderStyle-BorderColor="" ScrollBarArrowColor=""></Aspose.Cells.GridWeb.ViewerStyleTemplate>

**Example**

```
         		GridWeb1.setCustomStyleFileName("c:\\style\\mystyle.xml");
```

**Returns:**
java.lang.String
### getDPI() {#getDPI--}
```
public static double getDPI()
```


Obtient / Définit le DPI de la machine.

**Remarks**

**Returns:**
double
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Obtient le nom de police par défaut du contrôle.

**Example**

```
         		GridWeb1.setDefaultFontName("Arial");
```

**Returns:**
java.lang.String
### getDefaultFontSize() {#getDefaultFontSize--}
```
public FontUnit getDefaultFontSize()
```


Obtient la taille de police par défaut du contrôle.

**Example**

```
         		GridWeb1.setDefaultFontSize(new FontUnit("10pt"));
```

**Returns:**
[FontUnit](../../com.aspose.gridweb/fontunit)
### getDefaultGridLineColor() {#getDefaultGridLineColor--}
```
public Color getDefaultGridLineColor()
```


Obtient la couleur de la ligne de grille par défaut.

**Example**

```
         		GridWeb1.setDefaultGridLineColor(Color.getRed());
```

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getDisplayCellTip() {#getDisplayCellTip--}
```
public boolean getDisplayCellTip()
```


Obtient si les astuces doivent être affichées. la valeur par défaut est true.

**Returns:**
boolean
### getEditMode() {#getEditMode--}
```
public boolean getEditMode()
```


Obtient le mode d'édition du contrôle.

**Remarks**

Lorsque la valeur est vraie, les cellules du contrôle sont modifiables, et les icônes "save" et "undo" sont affichées. Lorsque la valeur est fausse, les cellules du contrôle sont en lecture seule, et les icônes "save" et "undo" ne sont pas affichées.

**Returns:**
boolean
### getEnableAJAX() {#getEnableAJAX--}
```
public boolean getEnableAJAX()
```


Obtient si l'appel AJAX doit être utilisé. la valeur par défaut est true.

**Returns:**
boolean
### getEnableAsync() {#getEnableAsync--}
```
public boolean getEnableAsync()
```


Obtient si les données des cellules sont chargées de manière asynchrone, suggéré de l'appliquer pour une feuille contenant plus de 10000 cellules.

**Returns:**
boolean
### getEnableClientColumnOperations() {#getEnableClientColumnOperations--}
```
public boolean getEnableClientColumnOperations()
```


Obtient si les opérations de colonne côté client sont activées.

**Remarks**

Lorsque la valeur est vraie, l'utilisateur peut utiliser le menu contextuel pour ajouter/supprimer des colonnes.

**Returns:**
boolean
### getEnableClientFreeze() {#getEnableClientFreeze--}
```
public boolean getEnableClientFreeze()
```


Obtient si les opérations de gel côté client sont activées.

**Remarks**

Lorsque la valeur est vraie, l'utilisateur peut utiliser le menu contextuel pour figer/dégeler les volets.

**Returns:**
boolean
### getEnableClientMergeOperations() {#getEnableClientMergeOperations--}
```
public boolean getEnableClientMergeOperations()
```


Obtient si les opérations de fusion côté client sont activées.

**Remarks**

Lorsque la valeur est vraie, l'utilisateur peut utiliser le menu contextuel pour fusionner/dissocier les cellules.

**Returns:**
boolean
### getEnableClientResizeColumnRow() {#getEnableClientResizeColumnRow--}
```
public boolean getEnableClientResizeColumnRow()
```


Obtient si le redimensionnement des colonnes et des lignes côté client est activé.

**Remarks**

Lorsque la valeur est vraie, l'utilisateur peut redimensionner la colonne et la ligne côté client.

**Returns:**
boolean
### getEnableClientRowOperations() {#getEnableClientRowOperations--}
```
public boolean getEnableClientRowOperations()
```


Obtient si les opérations de ligne côté client sont activées.

**Remarks**

Lorsque la valeur est vraie, l'utilisateur peut utiliser le menu contextuel pour ajouter/supprimer des lignes.

**Returns:**
boolean
### getEnableDoubleClickEvent() {#getEnableDoubleClickEvent--}
```
public boolean getEnableDoubleClickEvent()
```


Obtient si l'événement double-clic côté client est activé.

**Remarks**

Lorsque la valeur est vraie, le contrôle recevra les événements de double-clic côté client et vous pourrez gérer ces événements côté serveur. Sinon, le contrôle ignorera tout événement de double-clic.

**Returns:**
boolean
### getEnableMetalLightEffect() {#getEnableMetalLightEffect--}
```
public boolean getEnableMetalLightEffect()
```


Obtient si l'effet de lumière métallique est appliqué.

**Returns:**
boolean
### getEnablePaging() {#getEnablePaging--}
```
public boolean getEnablePaging()
```


Obtient si le mode de pagination du contrôle est activé.

**Remarks**

Lorsque la valeur est vraie, le contrôle affichera PageSize lignes de données d'un coup, et affichera le sélecteur de page dans la barre d'onglets.

**Returns:**
boolean
### getEnableStyleDialogbox() {#getEnableStyleDialogbox--}
```
public boolean getEnableStyleDialogbox()
```


Obtient si la boîte de dialogue de style côté client est activée.

**Remarks**

Lorsque la valeur est vraie, l'utilisateur peut utiliser la boîte de dialogue de style pour définir le style d'une cellule en sélectionnant "Format Cell..." dans le menu contextuel.

**Returns:**
boolean
### getEnabled() {#getEnabled--}
```
public boolean getEnabled()
```


Obtient le Enabled dans le WebControl

**Returns:**
boolean
### getFilteredPaging() {#getFilteredPaging--}
```
public boolean getFilteredPaging()
```


Obtient si la pagination après filtrage des données est activée, prendra effet lorsque EnablePaging est true.

**Remarks**

Lorsque la valeur est vraie, le contrôle paginera en fonction des données filtrées, la valeur par défaut est false.

**Returns:**
boolean
### getFont() {#getFont--}
```
public FontInfo getFont()
```


Obtient le Font dans le WebControl

**Returns:**
[FontInfo](../../com.aspose.gridweb/fontinfo)
### getForceValidation() {#getForceValidation--}
```
public boolean getForceValidation()
```


Obtient si la validation côté client est forcée.

**Remarks**

Lorsque la valeur est vraie, les données ne seront pas envoyées au serveur tant que tous les champs de saisie ne sont pas valides.

**Returns:**
boolean
### getForeColor() {#getForeColor--}
```
public Color getForeColor()
```


Obtient le ForeColor dans le WebControl

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getFrameTableStyle() {#getFrameTableStyle--}
```
public GridTableStyle getFrameTableStyle()
```


Obtient le style de cadre du contrôle.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getGoonDefaultSaveOperation() {#getGoonDefaultSaveOperation--}
```
public boolean getGoonDefaultSaveOperation()
```


Obtient si GridWeb effectuera l'opération d'enregistrement par défaut, la valeur par défaut est true.

**Returns:**
boolean
### getHTMLBody() {#getHTMLBody--}
```
public String getHTMLBody()
```


le code html du bean pour le corps html, il doit être obtenu après l'appel des méthodes init et prepareRender

**Returns:**
java.lang.String
### getHTMLHead() {#getHTMLHead--}
```
public String getHTMLHead()
```


le code html du bean pour l'en-tête html, il doit être obtenu après l'appel de la méthode init et prepareRender

**Returns:**
java.lang.String
### getHeaderBarHeight() {#getHeaderBarHeight--}
```
public Unit getHeaderBarHeight()
```


Obtient la hauteur (System.Web.UI.WebControl.Unit) de la barre d'en-tête supérieure du contrôle.

**Example**

```
         		GridWeb1.setHeaderBarWidth(new Unit(32, com.aspose.gridweb.UnitType.Point));
         		GridWeb1.setHeaderBarHeight(new Unit(24, com.aspose.gridweb.UnitType.Point));
```

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getHeaderBarStyle() {#getHeaderBarStyle--}
```
public GridTableItemStyle getHeaderBarStyle()
```


Obtient le style de la barre d'en-tête.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getHeaderBarTableStyle() {#getHeaderBarTableStyle--}
```
public GridTableStyle getHeaderBarTableStyle()
```


Obtient le style de la barre d'en-tête du contrôle.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getHeaderBarWidth() {#getHeaderBarWidth--}
```
public Unit getHeaderBarWidth()
```


Obtient la largeur( System.Web.UI.WebControl.Unit ) ou la barre d'en-tête gauche du contrôle.

**Example**

```
         		GridWeb1.setHeaderBarWidth(new Unit(32, com.aspose.gridweb.UnitType.Point));
         		GridWeb1.setHeaderBarHeight(new Unit(24, com.aspose.gridweb.UnitType.Point));
```

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getHeight() {#getHeight--}
```
public Unit getHeight()
```


Obtient la hauteur( System.Web.UI.WebControl.Unit ) du contrôle.

**Example**

```
         		GridWeb1.setWidth(new Unit(320, com.aspose.gridweb.UnitType.Point));
         		GridWeb1.setHeight(new Unit(240, com.aspose.gridweb.UnitType.Point));
```

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getIgnoreStyleWithNoData() {#getIgnoreStyleWithNoData--}
```
public boolean getIgnoreStyleWithNoData()
```


Obtient si GridWeb ignore l'affichage des lignes ou colonnes qui ne contiennent pas de valeurs de cellule mais qui sont tout de même stylisées. Si la valeur est vraie, les performances seront meilleures. La valeur par défaut est false, ce qui signifie que si la dernière ligne/colonne consécutive n'a pas de valeurs de cellule mais est stylisée, nous les afficherons quand même. Cette option n'est valable que lorsque EnableAsync est false. Cette option n'a aucun effet lorsque EnableAsync est true, ce qui signifie que GridWeb affichera toutes les lignes/colonnes avec style.

**Returns:**
boolean
### getLoadOptions() {#getLoadOptions--}
```
public GridLoadOptions getLoadOptions()
```


Représente les options de chargement pour GridWeb.

**Returns:**
[GridLoadOptions](../../com.aspose.gridweb/gridloadoptions)
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Obtient l'indice maximal de colonne affichée (index zéro) de la feuille web. Le contrôle utilise la plus grande valeur entre MaxColumn et la colonne maximale des données de la feuille.

**Example**

```
         		// Creates a 4x4 "display window".
         		GridWeb1.setMinRow(2);
         		GridWeb1.setMaxRow(5);
         		GridWeb1.setMinColumn(3);
         		GridWeb1.setMaxColumn(6);
```

**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Obtient l'indice maximal de ligne affichée (index zéro) de la feuille web. Le contrôle utilise la plus grande valeur entre MaxRow et la ligne maximale des données de la feuille.

**Example**

```
         		// Creates a 4x4 "display window".
         		GridWeb1.setMinRow(2);
         		GridWeb1.setMaxRow(5);
         		GridWeb1.setMinColumn(3);
         		GridWeb1.setMaxColumn(6);
```

**Returns:**
int
### getMessage() {#getMessage--}
```
public String getMessage()
```


Obtient le message pour la grille.

**Returns:**
java.lang.String
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


Obtient l'indice minimal de colonne affichée (index zéro) de la feuille web. Le contrôle utilise la plus petite valeur entre MinColumn et la colonne minimale des données de la feuille.

**Example**

```
         		// Creates a 4x4 "display window".
         		GridWeb1.setMinRow(2);
         		GridWeb1.setMaxRow(5);
         		GridWeb1.setMinColumn(3);
         		GridWeb1.setMaxColumn(6);
```

**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```


Obtient l'indice minimal de ligne affichée (index zéro) de la feuille web. Le contrôle utilise la plus petite valeur entre MinRow et la ligne minimale des données de la feuille.

**Example**

```
         		// Creates a 4x4 "display window".
         		GridWeb1.setMinRow(2);
         		GridWeb1.setMaxRow(5);
         		GridWeb1.setMinColumn(3);
         		GridWeb1.setMaxColumn(6);
```

**Returns:**
int
### getModifiedCells() {#getModifiedCells--}
```
public ArrayList getModifiedCells()
```


Obtient la collection des cellules modifiées par le client.

**Returns:**
java.util.ArrayList
### getNeedRenderGroupRows() {#getNeedRenderGroupRows--}
```
public boolean getNeedRenderGroupRows()
```


Obtient si afficher les grouprows.

**Returns:**
boolean
### getNoHScroll() {#getNoHScroll--}
```
public boolean getNoHScroll()
```


Obtient une valeur indiquant si la barre de défilement horizontale est masquée.

**Returns:**
boolean
### getNoScroll() {#getNoScroll--}
```
public boolean getNoScroll()
```


Obtient si la barre de défilement doit être affichée.

**Returns:**
boolean
### getNoVScroll() {#getNoVScroll--}
```
public boolean getNoVScroll()
```


Obtient une valeur indiquant si la barre de défilement verticale est masquée.

**Returns:**
boolean
### getOnAjaxCallFinishedClientFunction() {#getOnAjaxCallFinishedClientFunction--}
```
public String getOnAjaxCallFinishedClientFunction()
```


Obtient le nom de la fonction côté client à appeler lorsque l'appel ajax est terminé. La fonction client doit être déclarée ainsi :
function GridAjaxcallFinished()
\{
alert(this.id+" ajaxcall finished ");
\}

Remarque : vous pouvez utiliser le pointeur "this" dans la fonction client pour faire référence au contrôle de grille qui déclenche l'événement.

**Returns:**
java.lang.String
### getOnCellErrorClientFunction() {#getOnCellErrorClientFunction--}
```
public String getOnCellErrorClientFunction()
```


Obtient le nom de la fonction côté client à appeler lorsqu'une validation de cellule échoue. La fonction client doit être déclarée ainsi :
function MyOnCellError(cell)
\{
alert(this.getCellValueByCell(cell));
\}

Remarque : vous pouvez utiliser le pointeur "this" dans la fonction client pour faire référence au contrôle de grille qui déclenche l'événement.

**Returns:**
java.lang.String
### getOnCellSelectedAjaxCallBackClientFunction() {#getOnCellSelectedAjaxCallBackClientFunction--}
```
public String getOnCellSelectedAjaxCallBackClientFunction()
```


Obtient la fonction côté client à appeler lorsqu'une cellule est sélectionnée. La fonction client doit être déclarée comme suit :
function MyOnSelectCellAjaxCallBack(cell,customerdata)
\{

\}

Remarque : vous pouvez utiliser le pointeur "this" dans la fonction client pour faire référence au contrôle de grille qui déclenche l'événement.

**Returns:**
java.lang.String
### getOnCellSelectedClientFunction() {#getOnCellSelectedClientFunction--}
```
public String getOnCellSelectedClientFunction()
```


Obtient la fonction côté client à appeler lorsqu'une cellule est sélectionnée. La fonction client doit être déclarée comme suit :
function MyOnSelectCell(cell)
\{
GridWeb1.setCellValueByCell(cell, "test");
\}

Remarque : vous pouvez utiliser le pointeur "this" dans la fonction client pour faire référence au contrôle de grille qui déclenche l'événement.

**Returns:**
java.lang.String
### getOnCellUnselectedClientFunction() {#getOnCellUnselectedClientFunction--}
```
public String getOnCellUnselectedClientFunction()
```


Obtient la fonction côté client à appeler lorsqu'une cellule est désélectionnée. La fonction client doit être déclarée comme suit :
function MyOnUnselectCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

Remarque : vous pouvez utiliser le pointeur "this" dans la fonction client pour faire référence au contrôle de grille qui déclenche l'événement.

**Returns:**
java.lang.String
### getOnCellUpdatedClientFunction() {#getOnCellUpdatedClientFunction--}
```
public String getOnCellUpdatedClientFunction()
```


Obtient le nom de la fonction côté client à appeler lorsque la valeur d'une cellule est mise à jour. La fonction client doit être déclarée comme suit :
function MyOnCellUpdated(cell)
\{
alert(this.getCellValueByCell(cell));
\}

Remarque : vous pouvez utiliser le pointeur "this" dans la fonction client pour faire référence au contrôle de grille qui déclenche l'événement.

**Returns:**
java.lang.String
### getOnContextMenuShowClientFunction() {#getOnContextMenuShowClientFunction--}
```
public String getOnContextMenuShowClientFunction()
```


Obtient la fonction côté client à appeler lorsque le menu contextuel sera affiché. La fonction client doit être déclarée comme suit :
function onContextMenuShow()
\{
var menu = event.srcElement;
menu.setItemVisibility("Delete", "block");
menu.setItemVisibility("Update", "none");
\}

Remarque : vous pouvez utiliser le pointeur "this" dans la fonction client pour faire référence au contrôle de grille qui déclenche l'événement.

**Returns:**
java.lang.String
### getOnDoubleClickCellClientFunction() {#getOnDoubleClickCellClientFunction--}
```
public String getOnDoubleClickCellClientFunction()
```


Obtient la fonction côté client à appeler lorsqu'une cellule est double-cliquée. La fonction client doit être déclarée comme suit :
function MyOnDoubleClickCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

Remarque : vous pouvez utiliser le pointeur "this" dans la fonction client pour faire référence au contrôle de grille qui déclenche l'événement.

**Returns:**
java.lang.String
### getOnDoubleClickRowClientFunction() {#getOnDoubleClickRowClientFunction--}
```
public String getOnDoubleClickRowClientFunction()
```


Obtient la fonction côté client à appeler lorsqu'une ligne est double-cliquée. La fonction client doit être déclarée comme suit :
function MyOnRowDoubleClick(row)
\{
alert(row);
\}

Remarque : vous pouvez utiliser le pointeur "this" dans la fonction client pour faire référence au contrôle de grille qui déclenche l'événement.

**Returns:**
java.lang.String
### getOnGridInitClientFunction() {#getOnGridInitClientFunction--}
```
public String getOnGridInitClientFunction()
```


Obtient le nom de la fonction côté client à appeler lorsque la grille est initialisée. La fonction client doit être déclarée comme suit :
function MyOnGridInit(grid)
\{
alert("The grid is initialized: " + grid.id);
\}

Remarque : vous pouvez utiliser le pointeur "this" dans la fonction client pour faire référence au contrôle de grille qui déclenche l'événement.

**Returns:**
java.lang.String
### getOnPageChangeClientFunction() {#getOnPageChangeClientFunction--}
```
public String getOnPageChangeClientFunction()
```


Obtient la fonction côté client à appeler après le changement d'index de page. Ne prend effet que lorsque EnablePaging est vrai. La fonction client doit être déclarée comme suit :
function MyOnPageChange(index)
\{
console.log("current page is:"+index);
\}

Remarque : vous pouvez utiliser le pointeur "this" dans la fonction client pour faire référence au contrôle de grille qui déclenche l'événement.

**Returns:**
java.lang.String
### getOnPageSubmitClientFunction() {#getOnPageSubmitClientFunction--}
```
public String getOnPageSubmitClientFunction()
```


Obtient la fonction client à appeler avant que la page ne soit soumise côté client.

**Returns:**
java.lang.String
### getOnShapeSelectedClientFunction() {#getOnShapeSelectedClientFunction--}
```
public String getOnShapeSelectedClientFunction()
```


Obtient la fonction côté client à appeler lorsqu'une forme est sélectionnée. La fonction client doit être déclarée ainsi :
function MyOnSelectShape(shape)
\{
var name=shape.getAttribute("namevalue")
var text=shape.getAttribute("textvalue")
var value=shape.getAttribute("controlvalue")
var type=shape.getAttribute("msotype")
\}

Remarque : vous pouvez utiliser le pointeur "this" dans la fonction client pour faire référence au contrôle de grille qui déclenche l'événement.

**Returns:**
java.lang.String
### getOnSubmitClientFunction() {#getOnSubmitClientFunction--}
```
public String getOnSubmitClientFunction()
```


Obtient la fonction côté client à appeler avant que le contrôle ne soit soumis côté client. La fonction client doit être déclarée ainsi :
function MyOnSubmit(arg, cancelEdit)
\{
return true;
\}
L'arg est l'argument de soumission, il contient la commande à poster au serveur. Le cancelEdit est une valeur booléenne indiquant si le contrôle a rejeté l'entrée de l'utilisateur avant la soumission. Le contrôle continuera à soumettre si la fonction renvoie true.
Remarque : vous pouvez utiliser le pointeur "this" dans la fonction client pour faire référence au contrôle de grille qui déclenche l'événement.

**Returns:**
java.lang.String
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


Obtient si seules les lignes dont la hauteur n'est pas personnalisée sont ajustées, la valeur par défaut est false.

**Returns:**
boolean
### getPageSize() {#getPageSize--}
```
public int getPageSize()
```


Obtient la taille de la page en mode pagination.

**Remarks**

En mode pagination, le contrôle affichera une fois PageSize lignes de données, et affichera le contrôle de sélection de page dans la barre d'onglets.

**Returns:**
int
### getPictureCachePath() {#getPictureCachePath--}
```
public static String getPictureCachePath()
```


Obtient le chemin de stockage des images pour le classeur, toutes les formes et images seront stockées dans ce répertoire, le chemin par défaut est acwcache sous le répertoire de base de l'application actuelle ; les utilisateurs doivent implémenter un service planifié pour nettoyer les fichiers dont le temps de session est expiré.

**Returns:**
java.lang.String
### getPresetStyle() {#getPresetStyle--}
```
public int getPresetStyle()
```


Obtient le style prédéfini.

Voir [PresetStyle](../../com.aspose.gridweb/presetstyle).

**Example**

```
         		GridWeb1.setPresetStyle(PresetStyle.TRADITIONAL_1);
```

**Returns:**
int
### getRefreshValidation() {#getRefreshValidation--}
```
public boolean getRefreshValidation()
```


Obtient si la valeur de validation doit être rafraîchie après la modification de la valeur de la cellule.

**Returns:**
boolean
### getRenderHiddenRow() {#getRenderHiddenRow--}
```
public boolean getRenderHiddenRow()
```


Obtient si la ligne masquée est rendue dans GridControl, la valeur par défaut est false. Si vous devez réafficher la ligne masquée plus tard, vous devez la définir sur true.

**Returns:**
boolean
### getRowHeightForCSV() {#getRowHeightForCSV--}
```
public double getRowHeightForCSV()
```


Obtient la valeur de hauteur de ligne en points pour le fichier csv, la valeur par défaut est 14,5.

**Returns:**
double
### getScrollBarArrowColor() {#getScrollBarArrowColor--}
```
public Color getScrollBarArrowColor()
```


Spécifie la couleur du bouton flèche de la barre de défilement.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getScrollBarBaseColor() {#getScrollBarBaseColor--}
```
public Color getScrollBarBaseColor()
```


Spécifie la couleur de la barre de défilement du contrôle.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCellBgColor() {#getSelectCellBgColor--}
```
public Color getSelectCellBgColor()
```


Spécifie la couleur d'arrière-plan des cellules sélectionnées dans une plage de sélection multiple.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCellColor() {#getSelectCellColor--}
```
public Color getSelectCellColor()
```


Spécifie la couleur des cellules sélectionnées dans une plage de sélection multiple.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSessionStorePath() {#getSessionStorePath--}
```
public String getSessionStorePath()
```


Obtient le chemin de stockage du cache de session lorsque le mode de session est File ou ViewState, etc : gridweb.SessionStorePath="c:/mytempdir/session"; alors les données de session seront stockées dans c:/mytempdir/session

**Returns:**
java.lang.String
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


Représente les paramètres du classeur.

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridweb/gridworkbooksettings)
### getShowAddButton() {#getShowAddButton--}
```
public boolean getShowAddButton()
```


Obtient si le bouton d'ajout de feuille de calcul doit être affiché.

**Returns:**
boolean
### getShowBottomBar() {#getShowBottomBar--}
```
public boolean getShowBottomBar()
```


Spécifie si la barre de commande (incluant la barre de commande et la barre d'onglets) doit être affichée en bas du contrôle.

**Returns:**
boolean
### getShowCellEditBox() {#getShowCellEditBox--}
```
public boolean getShowCellEditBox()
```


Indique si Gridweb affiche la barre d'outils de la zone d'édition comme dans MS-EXCEL. Si elle est activée, une zone d'édition pour la cellule actuelle sera affichée dans Gridweb. Si nous activons cette fonctionnalité, nous devons importer la bibliothèque jquery js dans vos fichiers aspx pour prendre en charge cette nouvelle fonctionnalité. Toute version récente de jquery convient, etc.

**Returns:**
boolean
### getShowCommandBarAtTop() {#getShowCommandBarAtTop--}
```
public boolean getShowCommandBarAtTop()
```


Spécifie si la barre de commande (incluant la barre de commande et la barre d'onglets) doit être affichée en haut du contrôle.

**Returns:**
boolean
### getShowContextMenu() {#getShowContextMenu--}
```
public boolean getShowContextMenu()
```


Obtient si le menu contextuel doit être affiché. La valeur par défaut est true.

**Returns:**
boolean
### getShowDefaultGridLine() {#getShowDefaultGridLine--}
```
public boolean getShowDefaultGridLine()
```


Obtient si les lignes de grille par défaut des cellules doivent être affichées.

**Returns:**
boolean
### getShowHeaderBar() {#getShowHeaderBar--}
```
public boolean getShowHeaderBar()
```


Obtient si la barre d'en-tête doit être affichée

**Returns:**
boolean
### getShowLoading() {#getShowLoading--}
```
public boolean getShowLoading()
```


Spécifie si une boîte de dialogue de chargement doit être affichée pendant le postback vers le serveur.

**Returns:**
boolean
### getShowLoadingPosition() {#getShowLoadingPosition--}
```
public String getShowLoadingPosition()
```


Spécifie la position gauche, haut (en px) pour afficher la boîte de dialogue de chargement pendant le postback vers le serveur, etc. 100,200 signifie que la position gauche, haut de la boîte de dialogue de chargement est à 100 px,200 px.

**Returns:**
java.lang.String
### getShowSaveButton() {#getShowSaveButton--}
```
public boolean getShowSaveButton()
```


Obtient si le bouton d'enregistrement doit être affiché.

**Returns:**
boolean
### getShowSubmitButton() {#getShowSubmitButton--}
```
public boolean getShowSubmitButton()
```


Obtient si le bouton de soumission doit être affiché.

**Returns:**
boolean
### getShowTabBar() {#getShowTabBar--}
```
public boolean getShowTabBar()
```


Obtient si la barre d'onglets doit être affichée.

**Returns:**
boolean
### getShowTabNavigation() {#getShowTabNavigation--}
```
public boolean getShowTabNavigation()
```


Obtient si le bouton de navigation des onglets est affiché, la valeur par défaut est true.

**Returns:**
boolean
### getShowUndoButton() {#getShowUndoButton--}
```
public boolean getShowUndoButton()
```


Obtient si le bouton d'annulation doit être affiché.

**Returns:**
boolean
### getSpanWrap() {#getSpanWrap--}
```
public boolean getSpanWrap()
```


Spécifie si le contenu doit être enveloppé dans la portée de cellule, la valeur par défaut est true.

**Returns:**
boolean
### getTabIndex() {#getTabIndex--}
```
public short getTabIndex()
```


Obtient le TabIndex dans le WebControl

**Returns:**
short
### getTabStyle() {#getTabStyle--}
```
public GridTableItemStyle getTabStyle()
```


Obtient le style de la barre d'onglets.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getToolTip() {#getToolTip--}
```
public String getToolTip()
```


Obtient le ToolTip dans le WebControl

**Returns:**
java.lang.String
### getUseClientPageHeight() {#getUseClientPageHeight--}
```
public boolean getUseClientPageHeight()
```


Obtient si GridWeb utilise la hauteur de la page client comme hauteur du contrôle, adapté lorsque Height="100%" est défini, la valeur par défaut est false.

**Returns:**
boolean
### getViewPanelScrollLeft() {#getViewPanelScrollLeft--}
```
public String getViewPanelScrollLeft()
```


Obtient la position de la barre de défilement du panneau de vue de la grille.

**Returns:**
java.lang.String
### getViewPanelScrollTop() {#getViewPanelScrollTop--}
```
public String getViewPanelScrollTop()
```


Obtient la position de la barre de défilement du panneau de vue de la grille.

**Returns:**
java.lang.String
### getViewTableStyle() {#getViewTableStyle--}
```
public GridTableStyle getViewTableStyle()
```


Obtient le style du panneau de vue des données.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


Obtient la largeur (System.Web.UI.WebControl.Unit) du contrôle.

**Example**

```
         		GridWeb1.setWidth(new Unit(320, com.aspose.gridweb.UnitType.Point));
         		GridWeb1.setHeight(new Unit(240, com.aspose.gridweb.UnitType.Point));
```

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getWorkSheets() {#getWorkSheets--}
```
public GridWorksheetCollection getWorkSheets()
```


Obtient la collection des feuilles de calcul.

**Returns:**
[GridWorksheetCollection](../../com.aspose.gridweb/gridworksheetcollection)
### getXhtmlMode() {#getXhtmlMode--}
```
public boolean getXhtmlMode()
```


Obtient si le style XHTML doit être utilisé, la valeur par défaut est true.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### importExcelFile(InputStream stream) {#importExcelFile-java.io.InputStream-}
```
public void importExcelFile(InputStream stream)
```


Importe depuis un flux de fichier Excel, y compris le flux de fichier disque ou le flux mémoire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | Le flux du fichier Excel, incluant le flux de fichier disque ou le flux mémoire. |

### importExcelFile(InputStream stream, String passwordtoOpen) {#importExcelFile-java.io.InputStream-java.lang.String-}
```
public void importExcelFile(InputStream stream, String passwordtoOpen)
```


Importe depuis un flux de fichier Excel, y compris le flux de fichier disque ou le flux mémoire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | Le flux du fichier Excel, incluant le flux de fichier disque ou le flux mémoire. |
| passwordtoOpen | java.lang.String | le mot de passe d'ouverture du fichier qui est chiffré. |

### importExcelFile(String fileName) {#importExcelFile-java.lang.String-}
```
public void importExcelFile(String fileName)
```


Importe depuis un fichier Excel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Le nom du fichier Excel. |

### importExcelFile(String fileName, String passwordtoOpen) {#importExcelFile-java.lang.String-java.lang.String-}
```
public void importExcelFile(String fileName, String passwordtoOpen)
```


Importe depuis un fichier Excel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Le nom du fichier Excel. |
| passwordtoOpen | java.lang.String | le mot de passe d'ouverture du fichier qui est chiffré. |

### init() {#init--}
```
public void init()
```


le bean doit être initialisé par la requête et la réponse du servlet de la page actuelle

### isCalculateFormula() {#isCalculateFormula--}
```
public boolean isCalculateFormula()
```


Obtient si la formule doit être calculée après les changements de valeur de cellule ou après l'importation du fichier. La valeur par défaut est true.

**Returns:**
boolean
### loadCSVFile(InputStream stream) {#loadCSVFile-java.io.InputStream-}
```
public void loadCSVFile(InputStream stream)
```


Charge les données depuis un flux de fichier CSV.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | Le flux de fichier. |

### loadCSVFile(String fileName) {#loadCSVFile-java.lang.String-}
```
public void loadCSVFile(String fileName)
```


Charge les données depuis un fichier CSV.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Le nom du fichier. |

### loadHTMLFile(InputStream stream) {#loadHTMLFile-java.io.InputStream-}
```
public void loadHTMLFile(InputStream stream)
```


Charge les données depuis un flux de fichier HTML.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | Le flux de fichier. |

### loadHTMLFile(String fileName) {#loadHTMLFile-java.lang.String-}
```
public void loadHTMLFile(String fileName)
```


Charge les données depuis un fichier HTML.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Le nom du fichier. |

### loadSpreadSheetMLFile(InputStream stream) {#loadSpreadSheetMLFile-java.io.InputStream-}
```
public void loadSpreadSheetMLFile(InputStream stream)
```


Charge les données depuis un flux de fichier SpreadSheetML.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | Le flux du fichier. |

### loadSpreadSheetMLFile(String fileName) {#loadSpreadSheetMLFile-java.lang.String-}
```
public void loadSpreadSheetMLFile(String fileName)
```


Charge les données depuis un fichier SpreadSheetML.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Le nom du fichier. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### prepareRender() {#prepareRender--}
```
public void prepareRender()
```


la méthode doit être appelée avant le rendu du bean GridWeb

### refreshChartShape() {#refreshChartShape--}
```
public void refreshChartShape()
```


Actualise toutes les images de graphiques pour la feuille de calcul active.

### saveCSVFile(OutputStream stream) {#saveCSVFile-java.io.OutputStream-}
```
public void saveCSVFile(OutputStream stream)
```


Enregistre les données dans un flux de fichier CSV.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Le flux de fichier. |

### saveCSVFile(String targetFile) {#saveCSVFile-java.lang.String-}
```
public void saveCSVFile(String targetFile)
```


Enregistre les données dans un fichier CSV.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| targetFile | java.lang.String | Le nom du fichier. |

### saveCustomStyleFile(String fileName) {#saveCustomStyleFile-java.lang.String-}
```
public void saveCustomStyleFile(String fileName)
```


Enregistre les données de style actuelles du contrôle dans un fichier XML. Peut être utilisé pour créer votre fichier de style personnalisé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Le nom du fichier de style. |

### saveHTMLFile(OutputStream stream) {#saveHTMLFile-java.io.OutputStream-}
```
public void saveHTMLFile(OutputStream stream)
```


Enregistre les données dans un flux de fichier HTML.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Le flux de fichier. |

### saveHTMLFile(String targetFile) {#saveHTMLFile-java.lang.String-}
```
public void saveHTMLFile(String targetFile)
```


Enregistre les données dans un fichier HTML.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| targetFile | java.lang.String | Le nom du fichier. |

### saveSpreadSheetMLFile(OutputStream stream) {#saveSpreadSheetMLFile-java.io.OutputStream-}
```
public void saveSpreadSheetMLFile(OutputStream stream)
```


Enregistre les données dans un flux de fichier SpreadSheetML.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Le flux de fichier. |

### saveSpreadSheetMLFile(String targetFile) {#saveSpreadSheetMLFile-java.lang.String-}
```
public void saveSpreadSheetMLFile(String targetFile)
```


Enregistre les données dans un fichier SpreadSheetML.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| targetFile | java.lang.String | Le nom du fichier. |

### saveToExcelFile(OutputStream stream) {#saveToExcelFile-java.io.OutputStream-}
```
public void saveToExcelFile(OutputStream stream)
```


Enregistre les feuilles de calcul dans un fichier Excel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Le flux dans lequel écrire. |

### saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions) {#saveToExcelFile-java.io.OutputStream-com.aspose.gridweb.GridSaveOptions-}
```
public void saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions)
```


Enregistre les feuilles de calcul dans un fichier Excel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Le flux dans lequel écrire. |
| saveOptions | [GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions) | Les options d'enregistrement. |

### saveToExcelFile(OutputStream stream, int format) {#saveToExcelFile-java.io.OutputStream-int-}
```
public void saveToExcelFile(OutputStream stream, int format)
```


Enregistre les feuilles de calcul dans un fichier Excel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Le flux dans lequel écrire. |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat). Le format de fichier (Excel2003, Excel2007, CSV, SpreadsheetML) |

### saveToExcelFile(String targetFile) {#saveToExcelFile-java.lang.String-}
```
public void saveToExcelFile(String targetFile)
```


Enregistre les feuilles de calcul dans un fichier Excel au format Excel 2003.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| targetFile | java.lang.String | Le nom du fichier cible dans lequel écrire. |

### saveToExcelFile(String targetFile, GridSaveOptions saveOptions) {#saveToExcelFile-java.lang.String-com.aspose.gridweb.GridSaveOptions-}
```
public void saveToExcelFile(String targetFile, GridSaveOptions saveOptions)
```


Enregistre les feuilles de calcul dans un fichier Excel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| targetFile | java.lang.String | Le nom du fichier cible dans lequel écrire. |
| saveOptions | [GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions) | Les options d'enregistrement. |

### saveToExcelFile(String targetFile, int format) {#saveToExcelFile-java.lang.String-int-}
```
public void saveToExcelFile(String targetFile, int format)
```


Enregistre les feuilles de calcul dans un fichier Excel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| targetFile | java.lang.String | Le nom du fichier cible dans lequel écrire. |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat). Le format de fichier (Excel2003, Excel2007, CSV, SpreadsheetML) |

### setACWClientPath(String value) {#setACWClientPath-java.lang.String-}
```
public void setACWClientPath(String value)
```


Définit le chemin web des fichiers script/image du contrôle. Par exemple : "http://localhost/acw\_client". Vous pouvez également définir cette valeur dans le fichier web.config. Ajoutez cette section à la section `<configuration>` :
`<appSettings>`
`<add key=\"aspose.cells.gridweb.acw_client_path\" value=\"/acw_client/\" />`
`</appSettings>`


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setACWLanguageFileUrl(String value) {#setACWLanguageFileUrl-java.lang.String-}
```
public void setACWLanguageFileUrl(String value)
```


Définit l'URL web du fichier de langue du contrôle. Par exemple : "/acw\_client/lang\_en.js".
Par défaut, un fichier anglais intégré est utilisé.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setActiveCell(GridCell value) {#setActiveCell-com.aspose.gridweb.GridCell-}
```
public void setActiveCell(GridCell value)
```


Définit la cellule active de la feuille actuelle. Modifié pour être modifiable depuis la version 1.9.0.1.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [GridCell](../../com.aspose.gridweb/gridcell) |  |

### setActiveCellBgColor(Color value) {#setActiveCellBgColor-com.aspose.gridweb.Color-}
```
public void setActiveCellBgColor(Color value)
```


Spécifie la couleur d'arrière-plan de la cellule active.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveCellColor(Color value) {#setActiveCellColor-com.aspose.gridweb.Color-}
```
public void setActiveCellColor(Color value)
```


Spécifie la couleur de la cellule active.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveHeaderBgColor(Color value) {#setActiveHeaderBgColor-com.aspose.gridweb.Color-}
```
public void setActiveHeaderBgColor(Color value)
```


Spécifie la couleur d'arrière-plan de l'en-tête de ligne/colonne active.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveHeaderColor(Color value) {#setActiveHeaderColor-com.aspose.gridweb.Color-}
```
public void setActiveHeaderColor(Color value)
```


Spécifie la couleur de l'en-tête de ligne/colonne active.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


Définit l'index de la feuille active. Égal à WebWorksheets.ActiveSheetIndex.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setActiveTabStyle(GridTableItemStyle value) {#setActiveTabStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setActiveTabStyle(GridTableItemStyle value)
```


Spécifie le style de l'onglet actif.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setAutoRefreshChart(boolean value) {#setAutoRefreshChart-boolean-}
```
public void setAutoRefreshChart(boolean value)
```


Définit si l'image du graphique est mise à jour lors de la mise à jour de la valeur de la cellule. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setBackColor(Color value) {#setBackColor-com.aspose.gridweb.Color-}
```
public void setBackColor(Color value)
```


Définit le BackColor dans le WebControl

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBeanID(String beanID) {#setBeanID-java.lang.String-}
```
public void setBeanID(String beanID)
```


définir l'id html du bean

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| beanID | java.lang.String |  |

### setBorderColor(Color value) {#setBorderColor-com.aspose.gridweb.Color-}
```
public void setBorderColor(Color value)
```


Définit le BorderColor dans le WebControl

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


Définit le BorderStyle dans le WebControl

Voir [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setBorderWidth(Unit value) {#setBorderWidth-com.aspose.gridweb.Unit-}
```
public void setBorderWidth(Unit value)
```


Définit le BorderWidth dans le WebControl

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setBottomTableStyle(GridTableStyle value) {#setBottomTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setBottomTableStyle(GridTableStyle value)
```


Définit le style de la barre inférieure du contrôle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


Définit s'il faut calculer la formule après les changements de valeur de cellule ou après l'importation du fichier. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCssClass(String value) {#setCssClass-java.lang.String-}
```
public void setCssClass(String value)
```


Définit le CssClass dans le WebControl

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCurrentPageIndex(int value) {#setCurrentPageIndex-int-}
```
public void setCurrentPageIndex(int value)
```


Définit l'index de la page actuelle en mode pagination.

**Remarks**

En mode pagination, le contrôle affichera une fois PageSize lignes de données, et affichera le contrôle de sélection de page dans la barre d'onglets.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setCustomCalculationEngine(GridAbstractCalculationEngine value) {#setCustomCalculationEngine-com.aspose.gridweb.GridAbstractCalculationEngine-}
```
public void setCustomCalculationEngine(GridAbstractCalculationEngine value)
```


Représente le moteur de calcul personnalisé de l'utilisateur pour étendre le moteur de calcul par défaut d'Aspose.Cells.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [GridAbstractCalculationEngine](../../com.aspose.gridweb/gridabstractcalculationengine) |  |

### setCustomStyle(InputStream stream) {#setCustomStyle-java.io.InputStream-}
```
public void setCustomStyle(InputStream stream)
```


Définit le fichier de style personnalisé à partir d'un flux, y compris le flux de fichier disque ou le flux mémoire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | Le flux du fichier, incluant le flux de fichier disque ou le flux mémoire. |

### setCustomStyleFileName(String value) {#setCustomStyleFileName-java.lang.String-}
```
public void setCustomStyleFileName(String value)
```


Définit le nom du fichier de style personnalisé.

**Remarks**

Le fichier de style personnalisé est un fichier XML. Lorsque le nom du fichier est défini, le fichier sera chargé immédiatement. Voici le contenu du "style prédéfini standard" ------------------------------------------------------- <Aspose.Cells.GridWeb.ViewerStyleTemplate runat="server" HeaderBarWidth="30pt" ScrollBarBaseColor="" FrameTableStyle-BorderStyle="Solid" FrameTableStyle-LeftBorderStyle-BorderWidth="" FrameTableStyle-LeftBorderStyle-BorderColor="" FrameTableStyle-RightBorderStyle-BorderWidth="" FrameTableStyle-RightBorderStyle-BorderColor="" FrameTableStyle-BorderWidth="1px" FrameTableStyle-CellSpacing="0" FrameTableStyle-BorderColor="Gray" FrameTableStyle-CellPadding="0" FrameTableStyle-TopBorderStyle-BorderWidth="" FrameTableStyle-TopBorderStyle-BorderColor="" FrameTableStyle-BottomBorderStyle-BorderWidth="" FrameTableStyle-BottomBorderStyle-BorderColor="" HeaderBarStyle-LeftBorderStyle-BorderStyle="Solid" HeaderBarStyle-LeftBorderStyle-BorderWidth="1px" HeaderBarStyle-LeftBorderStyle-BorderColor="White" HeaderBarStyle-VerticalAlign="Middle" HeaderBarStyle-RightBorderStyle-BorderStyle="Solid" HeaderBarStyle-RightBorderStyle-BorderWidth="1px" HeaderBarStyle-RightBorderStyle-BorderColor="Gray" HeaderBarStyle-BorderWidth="1px" HeaderBarStyle-Font-Size="10pt" HeaderBarStyle-BorderColor="Gray" HeaderBarStyle-BorderStyle="Solid" HeaderBarStyle-HorizontalAlign="Center" HeaderBarStyle-ForeColor="Black" HeaderBarStyle-TopBorderStyle-BorderStyle="Solid" HeaderBarStyle-TopBorderStyle-BorderWidth="1px" HeaderBarStyle-TopBorderStyle-BorderColor="White" HeaderBarStyle-BackColor="\#E0E0E0" HeaderBarStyle-BottomBorderStyle-BorderStyle="Solid" HeaderBarStyle-BottomBorderStyle-BorderWidth="1px" HeaderBarStyle-BottomBorderStyle-BorderColor="Gray" ViewTableStyle-LeftBorderStyle-BorderWidth="" ViewTableStyle-LeftBorderStyle-BorderColor="" ViewTableStyle-LayoutFixed="Fixed" ViewTableStyle-RightBorderStyle-BorderWidth="" ViewTableStyle-RightBorderStyle-BorderColor="" ViewTableStyle-BorderWidth="0px" ViewTableStyle-CellSpacing="0" ViewTableStyle-CellPadding="0" ViewTableStyle-TopBorderStyle-BorderWidth="" ViewTableStyle-TopBorderStyle-BorderColor="" ViewTableStyle-BottomBorderStyle-BorderWidth="" ViewTableStyle-BottomBorderStyle-BorderColor="" BottomTableStyle-LeftBorderStyle-BorderWidth="" BottomTableStyle-LeftBorderStyle-BorderColor="" BottomTableStyle-LayoutFixed="Fixed" BottomTableStyle-RightBorderStyle-BorderWidth="" BottomTableStyle-RightBorderStyle-BorderColor="" BottomTableStyle-BorderWidth="0px" BottomTableStyle-CellSpacing="0" BottomTableStyle-CellPadding="1" BottomTableStyle-TopBorderStyle-BorderStyle="Solid" BottomTableStyle-TopBorderStyle-BorderWidth="1px" BottomTableStyle-TopBorderStyle-BorderColor="Gray" BottomTableStyle-BottomBorderStyle-BorderWidth="" BottomTableStyle-BottomBorderStyle-BorderColor="" HeaderBarHeight="15pt" ActiveTabStyle-LeftBorderStyle-BorderWidth="" ActiveTabStyle-LeftBorderStyle-BorderColor="" ActiveTabStyle-RightBorderStyle-BorderWidth="" ActiveTabStyle-RightBorderStyle-BorderColor="" ActiveTabStyle-Height="15pt" ActiveTabStyle-BorderWidth="1px" ActiveTabStyle-Font-Size="10pt" ActiveTabStyle-BorderColor="Gray" ActiveTabStyle-ForeColor="Black" ActiveTabStyle-TopBorderStyle-BorderWidth="" ActiveTabStyle-TopBorderStyle-BorderColor="" ActiveTabStyle-BackColor="White" ActiveTabStyle-BottomBorderStyle-BorderWidth="" ActiveTabStyle-BottomBorderStyle-BorderColor="" HeaderBarTableStyle-LeftBorderStyle-BorderWidth="" HeaderBarTableStyle-LeftBorderStyle-BorderColor="" HeaderBarTableStyle-LayoutFixed="Fixed" HeaderBarTableStyle-RightBorderStyle-BorderWidth="" HeaderBarTableStyle-RightBorderStyle-BorderColor="" HeaderBarTableStyle-BorderWidth="0px" HeaderBarTableStyle-CellSpacing="0" HeaderBarTableStyle-BorderCollapse="Separate" HeaderBarTableStyle-CellPadding="0" HeaderBarTableStyle-TopBorderStyle-BorderWidth="" HeaderBarTableStyle-TopBorderStyle-BorderColor="" HeaderBarTableStyle-BottomBorderStyle-BorderWidth="" HeaderBarTableStyle-BottomBorderStyle-BorderColor="" TabStyle-LeftBorderStyle-BorderWidth="" TabStyle-LeftBorderStyle-BorderColor="" TabStyle-RightBorderStyle-BorderWidth="" TabStyle-RightBorderStyle-BorderColor="" TabStyle-Height="15pt" TabStyle-BorderWidth="1px" TabStyle-Font-Size="10pt" TabStyle-BorderColor="Gray" TabStyle-ForeColor="Black" TabStyle-TopBorderStyle-BorderWidth="" TabStyle-TopBorderStyle-BorderColor="" TabStyle-BackColor="\#E0E0E0" TabStyle-BottomBorderStyle-BorderWidth="" TabStyle-BottomBorderStyle-BorderColor="" ScrollBarArrowColor=""></Aspose.Cells.GridWeb.ViewerStyleTemplate>

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setDPI(double value) {#setDPI-double-}
```
public static void setDPI(double value)
```


Obtient / Définit le DPI de la machine.

**Remarks**

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Définit le nom de police par défaut du contrôle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setDefaultFontSize(FontUnit value) {#setDefaultFontSize-com.aspose.gridweb.FontUnit-}
```
public void setDefaultFontSize(FontUnit value)
```


Définit la taille de police par défaut du contrôle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [FontUnit](../../com.aspose.gridweb/fontunit) |  |

### setDefaultGridLineColor(Color value) {#setDefaultGridLineColor-com.aspose.gridweb.Color-}
```
public void setDefaultGridLineColor(Color value)
```


Définit la couleur par défaut des lignes de la grille.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setDisplayCellTip(boolean value) {#setDisplayCellTip-boolean-}
```
public void setDisplayCellTip(boolean value)
```


Définit s'il faut afficher les astuces. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEditMode(boolean value) {#setEditMode-boolean-}
```
public void setEditMode(boolean value)
```


Définit le mode d'édition du contrôle.

**Remarks**

Lorsque la valeur est vraie, les cellules du contrôle sont modifiables, et les icônes "save" et "undo" sont affichées. Lorsque la valeur est fausse, les cellules du contrôle sont en lecture seule, et les icônes "save" et "undo" ne sont pas affichées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEnableAJAX(boolean value) {#setEnableAJAX-boolean-}
```
public void setEnableAJAX(boolean value)
```


Définit s'il faut utiliser l'appel AJAX. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEnableAsync(boolean value) {#setEnableAsync-boolean-}
```
public void setEnableAsync(boolean value)
```


Définit s'il faut charger les données des cellules de manière asynchrone, recommandé pour une feuille contenant plus de 10 000 cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEnableClientColumnOperations(boolean value) {#setEnableClientColumnOperations-boolean-}
```
public void setEnableClientColumnOperations(boolean value)
```


Définit s'il faut activer les opérations de colonne côté client.

**Remarks**

Lorsque la valeur est vraie, l'utilisateur peut utiliser le menu contextuel pour ajouter/supprimer des colonnes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEnableClientFreeze(boolean value) {#setEnableClientFreeze-boolean-}
```
public void setEnableClientFreeze(boolean value)
```


Définit s'il faut activer les opérations de gel côté client.

**Remarks**

Lorsque la valeur est vraie, l'utilisateur peut utiliser le menu contextuel pour figer/dégeler les volets.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEnableClientMergeOperations(boolean value) {#setEnableClientMergeOperations-boolean-}
```
public void setEnableClientMergeOperations(boolean value)
```


Définit s'il faut activer les opérations de fusion côté client.

**Remarks**

Lorsque la valeur est vraie, l'utilisateur peut utiliser le menu contextuel pour fusionner/dissocier les cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEnableClientResizeColumnRow(boolean value) {#setEnableClientResizeColumnRow-boolean-}
```
public void setEnableClientResizeColumnRow(boolean value)
```


Définit si l'agrandissement des colonnes et des lignes côté client est activé.

**Remarks**

Lorsque la valeur est vraie, l'utilisateur peut redimensionner la colonne et la ligne côté client.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEnableClientRowOperations(boolean value) {#setEnableClientRowOperations-boolean-}
```
public void setEnableClientRowOperations(boolean value)
```


Définit si les opérations de ligne côté client sont activées.

**Remarks**

Lorsque la valeur est vraie, l'utilisateur peut utiliser le menu contextuel pour ajouter/supprimer des lignes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEnableDoubleClickEvent(boolean value) {#setEnableDoubleClickEvent-boolean-}
```
public void setEnableDoubleClickEvent(boolean value)
```


Définit si l'événement double-clic côté client est activé.

**Remarks**

Lorsque la valeur est vraie, le contrôle recevra les événements de double-clic côté client et vous pourrez gérer ces événements côté serveur. Sinon, le contrôle ignorera tout événement de double-clic.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEnableMetalLightEffect(boolean value) {#setEnableMetalLightEffect-boolean-}
```
public void setEnableMetalLightEffect(boolean value)
```


Définit si l'effet de lumière métallique doit être appliqué.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEnablePaging(boolean value) {#setEnablePaging-boolean-}
```
public void setEnablePaging(boolean value)
```


Définit si le mode de pagination du contrôle est activé.

**Remarks**

Lorsque la valeur est vraie, le contrôle affichera PageSize lignes de données d'un coup, et affichera le sélecteur de page dans la barre d'onglets.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEnableStyleDialogbox(boolean value) {#setEnableStyleDialogbox-boolean-}
```
public void setEnableStyleDialogbox(boolean value)
```


Définit si la boîte de dialogue de style côté client est activée.

**Remarks**

Lorsque la valeur est vraie, l'utilisateur peut utiliser la boîte de dialogue de style pour définir le style d'une cellule en sélectionnant "Format Cell..." dans le menu contextuel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


Définit le Enabled dans le WebControl

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFilteredPaging(boolean value) {#setFilteredPaging-boolean-}
```
public void setFilteredPaging(boolean value)
```


Définit si la pagination après filtrage des données est activée, prendra effet lorsque EnablePaging est vrai.

**Remarks**

Lorsque la valeur est vraie, le contrôle paginera en fonction des données filtrées, la valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setForceValidation(boolean value) {#setForceValidation-boolean-}
```
public void setForceValidation(boolean value)
```


Définit si la validation côté client doit être forcée.

**Remarks**

Lorsque la valeur est vraie, les données ne seront pas envoyées au serveur tant que tous les champs de saisie ne sont pas valides.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setForeColor(Color value) {#setForeColor-com.aspose.gridweb.Color-}
```
public void setForeColor(Color value)
```


Définit le ForeColor dans le WebControl

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setFrameTableStyle(GridTableStyle value) {#setFrameTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setFrameTableStyle(GridTableStyle value)
```


Définit le style du cadre du contrôle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setGoonDefaultSaveOperation(boolean value) {#setGoonDefaultSaveOperation-boolean-}
```
public void setGoonDefaultSaveOperation(boolean value)
```


Définit si GridWeb effectuera l'opération d'enregistrement par défaut, la valeur par défaut est vraie.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHeaderBarHeight(Unit value) {#setHeaderBarHeight-com.aspose.gridweb.Unit-}
```
public void setHeaderBarHeight(Unit value)
```


Définit la hauteur (System.Web.UI.WebControl.Unit) de la barre d'en-tête supérieure du contrôle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHeaderBarStyle(GridTableItemStyle value) {#setHeaderBarStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setHeaderBarStyle(GridTableItemStyle value)
```


Définit le style de la barre d'en-tête.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setHeaderBarTableStyle(GridTableStyle value) {#setHeaderBarTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setHeaderBarTableStyle(GridTableStyle value)
```


Définit le style de la barre d'en-tête du contrôle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setHeaderBarWidth(Unit value) {#setHeaderBarWidth-com.aspose.gridweb.Unit-}
```
public void setHeaderBarWidth(Unit value)
```


Définit la largeur (System.Web.UI.WebControl.Unit) de la barre d'en-tête gauche du contrôle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHeight(Unit value) {#setHeight-com.aspose.gridweb.Unit-}
```
public void setHeight(Unit value)
```


Définit la hauteur (System.Web.UI.WebControl.Unit) du contrôle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setIgnoreStyleWithNoData(boolean value) {#setIgnoreStyleWithNoData-boolean-}
```
public void setIgnoreStyleWithNoData(boolean value)
```


Définit si GridWeb ignore l'affichage des lignes ou colonnes qui ne contiennent pas de valeurs de cellule mais qui sont tout de même stylisées. Si défini sur true, les performances seront meilleures. La valeur par défaut est false, ce qui signifie que si la dernière ligne/colonne consécutive n'a pas de valeurs de cellule mais est stylisée, nous les afficherons quand même. Cette option n'est valable que lorsque EnableAsync est false. Cette option n'a aucun effet lorsque EnableAsync est true, ce qui signifie que GridWeb affichera toutes les lignes/colonnes avec style.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setLoadOptions(GridLoadOptions value) {#setLoadOptions-com.aspose.gridweb.GridLoadOptions-}
```
public void setLoadOptions(GridLoadOptions value)
```


Représente les options de chargement pour GridWeb.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [GridLoadOptions](../../com.aspose.gridweb/gridloadoptions) |  |

### setMaxColumn(int value) {#setMaxColumn-int-}
```
public void setMaxColumn(int value)
```


Définit l'index maximal de colonne affichée (basé sur zéro) de la feuille web. Le contrôle utilise la valeur la plus grande entre MaxColumn et la colonne maximale des données de la feuille.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setMaxRow(int value) {#setMaxRow-int-}
```
public void setMaxRow(int value)
```


Définit l'index maximal de ligne affichée (basé sur zéro) de la feuille web. Le contrôle utilise la valeur la plus grande entre MaxRow et la ligne maximale des données de la feuille.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setMessage(String value) {#setMessage-java.lang.String-}
```
public void setMessage(String value)
```


Définit le message pour la grille.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setMinColumn(int value) {#setMinColumn-int-}
```
public void setMinColumn(int value)
```


Définit l'index minimal de colonne affichée (basé sur zéro) de la feuille web. Le contrôle utilise la plus petite valeur entre MinColumn et la colonne minimale des données de la feuille.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setMinRow(int value) {#setMinRow-int-}
```
public void setMinRow(int value)
```


Définit l'index minimal de ligne affichée (basé sur zéro) de la feuille web. Le contrôle utilise la plus petite valeur entre MinRow et la ligne minimale des données de la feuille.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setNeedRenderGroupRows(boolean value) {#setNeedRenderGroupRows-boolean-}
```
public void setNeedRenderGroupRows(boolean value)
```


Définit si les lignes de groupe doivent être affichées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setNoHScroll(boolean value) {#setNoHScroll-boolean-}
```
public void setNoHScroll(boolean value)
```


Définit une valeur indiquant si la barre de défilement horizontale est masquée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setNoScroll(boolean value) {#setNoScroll-boolean-}
```
public void setNoScroll(boolean value)
```


Définit si la barre de défilement doit être affichée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setNoVScroll(boolean value) {#setNoVScroll-boolean-}
```
public void setNoVScroll(boolean value)
```


Définit une valeur indiquant si la barre de défilement verticale est masquée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setOnAjaxCallFinishedClientFunction(String value) {#setOnAjaxCallFinishedClientFunction-java.lang.String-}
```
public void setOnAjaxCallFinishedClientFunction(String value)
```


Définit le nom de la fonction côté client à appeler lorsque l'appel ajax est terminé. La fonction client doit être déclarée ainsi :
function GridAjaxcallFinished()
\{
alert(this.id+" ajaxcall finished ");
\}

Remarque : vous pouvez utiliser le pointeur "this" dans la fonction client pour faire référence au contrôle de grille qui déclenche l'événement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setOnCellErrorClientFunction(String value) {#setOnCellErrorClientFunction-java.lang.String-}
```
public void setOnCellErrorClientFunction(String value)
```


Définit le nom de la fonction côté client à appeler lorsqu'une validation de cellule échoue. La fonction client doit être déclarée ainsi :
function MyOnCellError(cell)
\{
alert(this.getCellValueByCell(cell));
\}

Remarque : vous pouvez utiliser le pointeur "this" dans la fonction client pour faire référence au contrôle de grille qui déclenche l'événement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setOnCellSelectedAjaxCallBackClientFunction(String value) {#setOnCellSelectedAjaxCallBackClientFunction-java.lang.String-}
```
public void setOnCellSelectedAjaxCallBackClientFunction(String value)
```


Définit la fonction côté client à appeler lorsqu'une cellule est sélectionnée. La fonction client doit être déclarée ainsi :
function MyOnSelectCellAjaxCallBack(cell,customerdata)
\{

\}

Remarque : vous pouvez utiliser le pointeur "this" dans la fonction client pour faire référence au contrôle de grille qui déclenche l'événement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setOnCellSelectedClientFunction(String value) {#setOnCellSelectedClientFunction-java.lang.String-}
```
public void setOnCellSelectedClientFunction(String value)
```


Définit la fonction côté client à appeler lorsqu'une cellule est sélectionnée. La fonction client doit être déclarée ainsi :
function MyOnSelectCell(cell)
\{
GridWeb1.setCellValueByCell(cell, "test");
\}

Remarque : vous pouvez utiliser le pointeur "this" dans la fonction client pour faire référence au contrôle de grille qui déclenche l'événement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setOnCellUnselectedClientFunction(String value) {#setOnCellUnselectedClientFunction-java.lang.String-}
```
public void setOnCellUnselectedClientFunction(String value)
```


Définit la fonction côté client à appeler lorsqu'une cellule est désélectionnée. La fonction client doit être déclarée ainsi :
function MyOnUnselectCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

Remarque : vous pouvez utiliser le pointeur "this" dans la fonction client pour faire référence au contrôle de grille qui déclenche l'événement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setOnCellUpdatedClientFunction(String value) {#setOnCellUpdatedClientFunction-java.lang.String-}
```
public void setOnCellUpdatedClientFunction(String value)
```


Définit le nom de la fonction côté client à appeler lorsque la valeur d'une cellule est mise à jour. La fonction client doit être déclarée ainsi :
function MyOnCellUpdated(cell)
\{
alert(this.getCellValueByCell(cell));
\}

Remarque : vous pouvez utiliser le pointeur "this" dans la fonction client pour faire référence au contrôle de grille qui déclenche l'événement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setOnContextMenuShowClientFunction(String value) {#setOnContextMenuShowClientFunction-java.lang.String-}
```
public void setOnContextMenuShowClientFunction(String value)
```


Définit la fonction côté client à appeler lorsque le menu contextuel sera affiché. La fonction client doit être déclarée ainsi :
function onContextMenuShow()
\{
var menu = event.srcElement;
menu.setItemVisibility("Delete", "block");
menu.setItemVisibility("Update", "none");
\}

Remarque : vous pouvez utiliser le pointeur "this" dans la fonction client pour faire référence au contrôle de grille qui déclenche l'événement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setOnDoubleClickCellClientFunction(String value) {#setOnDoubleClickCellClientFunction-java.lang.String-}
```
public void setOnDoubleClickCellClientFunction(String value)
```


Définit la fonction côté client à appeler lorsqu'une cellule est double-cliquée. La fonction client doit être déclarée ainsi :
function MyOnDoubleClickCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

Remarque : vous pouvez utiliser le pointeur "this" dans la fonction client pour faire référence au contrôle de grille qui déclenche l'événement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setOnDoubleClickRowClientFunction(String value) {#setOnDoubleClickRowClientFunction-java.lang.String-}
```
public void setOnDoubleClickRowClientFunction(String value)
```


Définit la fonction côté client à appeler lorsqu'une ligne est double-cliquée. La fonction client doit être déclarée ainsi :
function MyOnRowDoubleClick(row)
\{
alert(row);
\}

Remarque : vous pouvez utiliser le pointeur "this" dans la fonction client pour faire référence au contrôle de grille qui déclenche l'événement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setOnGridInitClientFunction(String value) {#setOnGridInitClientFunction-java.lang.String-}
```
public void setOnGridInitClientFunction(String value)
```


Définit le nom de la fonction côté client à appeler lorsque la grille est initialisée. La fonction client doit être déclarée ainsi :
function MyOnGridInit(grid)
\{
alert("The grid is initialized: " + grid.id);
\}

Remarque : vous pouvez utiliser le pointeur "this" dans la fonction client pour faire référence au contrôle de grille qui déclenche l'événement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setOnPageChangeClientFunction(String value) {#setOnPageChangeClientFunction-java.lang.String-}
```
public void setOnPageChangeClientFunction(String value)
```


Définit la fonction côté client à appeler après le changement d'index de page. Ne prend effet que lorsque EnablePaging est true. La fonction client doit être déclarée ainsi :
function MyOnPageChange(index)
\{
console.log("current page is:"+index);
\}

Remarque : vous pouvez utiliser le pointeur "this" dans la fonction client pour faire référence au contrôle de grille qui déclenche l'événement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setOnPageSubmitClientFunction(String value) {#setOnPageSubmitClientFunction-java.lang.String-}
```
public void setOnPageSubmitClientFunction(String value)
```


Définit la fonction client à appeler avant que la page ne soit soumise côté client.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setOnShapeSelectedClientFunction(String value) {#setOnShapeSelectedClientFunction-java.lang.String-}
```
public void setOnShapeSelectedClientFunction(String value)
```


Définit la fonction côté client à appeler lorsqu'une forme est sélectionnée. La fonction client doit être déclarée ainsi :
function MyOnSelectShape(shape)
\{
var name=shape.getAttribute("namevalue")
var text=shape.getAttribute("textvalue")
var value=shape.getAttribute("controlvalue")
var type=shape.getAttribute("msotype")
\}

Remarque : vous pouvez utiliser le pointeur "this" dans la fonction client pour faire référence au contrôle de grille qui déclenche l'événement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setOnSubmitClientFunction(String value) {#setOnSubmitClientFunction-java.lang.String-}
```
public void setOnSubmitClientFunction(String value)
```


Définit la fonction client à appeler avant que le contrôle ne soit soumis côté client. La fonction client doit être déclarée ainsi :
function MyOnSubmit(arg, cancelEdit)
\{
return true;
\}
L'arg est l'argument de soumission, il contient la commande à poster au serveur. Le cancelEdit est une valeur booléenne indiquant si le contrôle a rejeté l'entrée de l'utilisateur avant la soumission. Le contrôle continuera à soumettre si la fonction renvoie true.
Remarque : vous pouvez utiliser le pointeur "this" dans la fonction client pour faire référence au contrôle de grille qui déclenche l'événement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


Définit si seules les lignes dont la hauteur n'est pas personnalisée doivent être ajustées, la valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPageSize(int value) {#setPageSize-int-}
```
public void setPageSize(int value)
```


Définit la taille de page en mode pagination.

**Remarks**

En mode pagination, le contrôle affichera une fois PageSize lignes de données, et affichera le contrôle de sélection de page dans la barre d'onglets.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPictureCachePath(String value) {#setPictureCachePath-java.lang.String-}
```
public static void setPictureCachePath(String value)
```


Définit le chemin de stockage des images pour le classeur, toutes les formes et images seront stockées dans ce répertoire, le chemin par défaut est acwcache sous le répertoire de base de l'application actuelle. Les utilisateurs doivent implémenter un service planifié pour nettoyer les fichiers dont le délai de session est expiré.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setPresetStyle(int value) {#setPresetStyle-int-}
```
public void setPresetStyle(int value)
```


Définit le style prédéfini.

Voir [PresetStyle](../../com.aspose.gridweb/presetstyle).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setRefreshValidation(boolean value) {#setRefreshValidation-boolean-}
```
public void setRefreshValidation(boolean value)
```


Définit s'il faut rafraîchir la valeur de validation après que la valeur de la cellule a changé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRenderHiddenRow(boolean value) {#setRenderHiddenRow-boolean-}
```
public void setRenderHiddenRow(boolean value)
```


Définit si la ligne masquée est rendue dans GridControl, la valeur par défaut est false. Si vous devez réafficher la ligne masquée plus tard, vous devez la définir sur true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRowHeightForCSV(double value) {#setRowHeightForCSV-double-}
```
public void setRowHeightForCSV(double value)
```


Définit la valeur de hauteur de ligne en points pour le fichier csv, la valeur par défaut est 14,5.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setScrollBarArrowColor(Color value) {#setScrollBarArrowColor-com.aspose.gridweb.Color-}
```
public void setScrollBarArrowColor(Color value)
```


Spécifie la couleur du bouton flèche de la barre de défilement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setScrollBarBaseColor(Color value) {#setScrollBarBaseColor-com.aspose.gridweb.Color-}
```
public void setScrollBarBaseColor(Color value)
```


Spécifie la couleur de la barre de défilement du contrôle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSelectCellBgColor(Color value) {#setSelectCellBgColor-com.aspose.gridweb.Color-}
```
public void setSelectCellBgColor(Color value)
```


Spécifie la couleur d'arrière-plan des cellules sélectionnées dans une plage de sélection multiple.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSelectCellColor(Color value) {#setSelectCellColor-com.aspose.gridweb.Color-}
```
public void setSelectCellColor(Color value)
```


Spécifie la couleur des cellules sélectionnées dans une plage de sélection multiple.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSessionStorePath(String value) {#setSessionStorePath-java.lang.String-}
```
public void setSessionStorePath(String value)
```


Définit le chemin de stockage du cache de session lorsque le mode de session est File ou ViewState, etc. : gridweb.SessionStorePath="c:/mytempdir/session"; il stockera alors les données de session dans c:/mytempdir/session.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridweb.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


Représente les paramètres du classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridweb/gridworkbooksettings) |  |

### setShowAddButton(boolean value) {#setShowAddButton-boolean-}
```
public void setShowAddButton(boolean value)
```


Définit s'il faut afficher le bouton d'ajout de feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowBottomBar(boolean value) {#setShowBottomBar-boolean-}
```
public void setShowBottomBar(boolean value)
```


Spécifie si la barre de commande (incluant la barre de commande et la barre d'onglets) doit être affichée en bas du contrôle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowCellEditBox(boolean value) {#setShowCellEditBox-boolean-}
```
public void setShowCellEditBox(boolean value)
```


Indique si Gridweb affiche la barre d'outils de la zone d'édition comme dans MS-EXCEL. Si elle est activée, une zone d'édition pour la cellule actuelle sera affichée dans Gridweb. Si nous activons cette fonctionnalité, nous devons importer la bibliothèque jquery js dans vos fichiers aspx pour prendre en charge cette nouvelle fonctionnalité. Toute version récente de jquery convient, etc.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowCommandBarAtTop(boolean value) {#setShowCommandBarAtTop-boolean-}
```
public void setShowCommandBarAtTop(boolean value)
```


Spécifie si la barre de commande (incluant la barre de commande et la barre d'onglets) doit être affichée en haut du contrôle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowContextMenu(boolean value) {#setShowContextMenu-boolean-}
```
public void setShowContextMenu(boolean value)
```


Définit s'il faut afficher le menu contextuel. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowDefaultGridLine(boolean value) {#setShowDefaultGridLine-boolean-}
```
public void setShowDefaultGridLine(boolean value)
```


Définit s'il faut afficher les lignes de grille par défaut des cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowHeaderBar(boolean value) {#setShowHeaderBar-boolean-}
```
public void setShowHeaderBar(boolean value)
```


Définit s'il faut afficher la barre d'en-tête

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowLoading(boolean value) {#setShowLoading-boolean-}
```
public void setShowLoading(boolean value)
```


Spécifie si une boîte de dialogue de chargement doit être affichée pendant le postback vers le serveur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowLoadingPosition(String value) {#setShowLoadingPosition-java.lang.String-}
```
public void setShowLoadingPosition(String value)
```


Spécifie la position gauche, haut (en px) pour afficher la boîte de dialogue de chargement pendant le postback vers le serveur, etc. 100,200 signifie que la position gauche, haut de la boîte de dialogue de chargement est à 100 px,200 px.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setShowSaveButton(boolean value) {#setShowSaveButton-boolean-}
```
public void setShowSaveButton(boolean value)
```


Définit si le bouton d'enregistrement doit être affiché.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowSubmitButton(boolean value) {#setShowSubmitButton-boolean-}
```
public void setShowSubmitButton(boolean value)
```


Définit si le bouton de soumission doit être affiché.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowTabBar(boolean value) {#setShowTabBar-boolean-}
```
public void setShowTabBar(boolean value)
```


Définit si la barre d'onglets doit être affichée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowTabNavigation(boolean value) {#setShowTabNavigation-boolean-}
```
public void setShowTabNavigation(boolean value)
```


Définit si le bouton de navigation des onglets est affiché, la valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowUndoButton(boolean value) {#setShowUndoButton-boolean-}
```
public void setShowUndoButton(boolean value)
```


Définit si le bouton d'annulation doit être affiché.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSpanWrap(boolean value) {#setSpanWrap-boolean-}
```
public void setSpanWrap(boolean value)
```


Spécifie si le contenu doit être enveloppé dans la portée de cellule, la valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setTabIndex(short value) {#setTabIndex-short-}
```
public void setTabIndex(short value)
```


Définit le TabIndex dans le WebControl

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | short |  |

### setTabStyle(GridTableItemStyle value) {#setTabStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setTabStyle(GridTableItemStyle value)
```


Définit le style de la barre d'onglets.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setToolTip(String value) {#setToolTip-java.lang.String-}
```
public void setToolTip(String value)
```


Définit le ToolTip dans le WebControl

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setUseClientPageHeight(boolean value) {#setUseClientPageHeight-boolean-}
```
public void setUseClientPageHeight(boolean value)
```


Définit si GridWeb utilise la hauteur de la page client comme hauteur du contrôle, adapté lorsque la propriété Height=\"100%\" est définie, la valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setViewPanelScrollLeft(String value) {#setViewPanelScrollLeft-java.lang.String-}
```
public void setViewPanelScrollLeft(String value)
```


Définit la position de la barre de défilement du panneau de visualisation de la grille.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setViewPanelScrollTop(String value) {#setViewPanelScrollTop-java.lang.String-}
```
public void setViewPanelScrollTop(String value)
```


Définit la position de la barre de défilement du panneau de visualisation de la grille.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setViewTableStyle(GridTableStyle value) {#setViewTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setViewTableStyle(GridTableStyle value)
```


Définit le style du panneau de visualisation des données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


Définit la largeur (System.Web.UI.WebControl.Unit) du contrôle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setXhtmlMode(boolean value) {#setXhtmlMode-boolean-}
```
public void setXhtmlMode(boolean value)
```


Définit si le style XHTML doit être utilisé, la valeur par défaut est true.

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

