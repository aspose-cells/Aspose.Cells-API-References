---
title: "Classe MainWeb"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridWeb.MainWeb. Classe parente du contrôle GridWeb. Usage interne uniquement"
type: docs
url: /fr/net/aspose.cells.gridweb/mainweb/
---
## MainWeb class

Classe parente du contrôle GridWeb. Usage interne uniquement.

```csharp
public class MainWeb : ExtWebControl, INamingContainer, IPostBackDataHandler, 
    IPostBackEventHandler, ISerializable
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [MainWeb](mainweb/)() | Le constructeur par défaut du contrôle MainWeb. |

## Propriétés

| Nom | Description |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb/mainweb/activecell/) { get; set; } | Obtient ou définit la cellule active de la feuille actuelle. Modifié pour être modifiable depuis la version 1.9.0.1. |
| [ActiveCellBgColor](../../aspose.cells.gridweb/mainweb/activecellbgcolor/) { get; set; } | Spécifie la couleur d'arrière-plan de la cellule active. |
| [ActiveCellColor](../../aspose.cells.gridweb/mainweb/activecellcolor/) { get; set; } | Spécifie la couleur de la cellule active. |
| [ActiveHeaderBgColor](../../aspose.cells.gridweb/mainweb/activeheaderbgcolor/) { get; set; } | Spécifie la couleur d'arrière-plan de l'en-tête de ligne/colonne actif. |
| [ActiveHeaderColor](../../aspose.cells.gridweb/mainweb/activeheadercolor/) { get; set; } | Spécifie la couleur de l'en-tête de ligne/colonne actif. |
| [ActiveSheet](../../aspose.cells.gridweb/mainweb/activesheet/) { get; } | Obtient la feuille active |
| [ActiveSheetIndex](../../aspose.cells.gridweb/mainweb/activesheetindex/) { get; set; } | Obtient ou définit l'index de la feuille active. Égal à WebWorksheets.ActiveSheetIndex. |
| [ActiveTabStyle](../../aspose.cells.gridweb/mainweb/activetabstyle/) { get; set; } | Spécifie le style de l'onglet actif. |
| [ACWClientPath](../../aspose.cells.gridweb/mainweb/acwclientpath/) { get; set; } | Obtient ou définit le chemin web des fichiers script/image du contrôle. Par exemple : "http://localhost/acw_client". Vous pouvez également définir cette valeur dans le fichier web.config. Ajoutez cette section à la section `<configuration>` :`<appSettings>``<add key="aspose.cells.gridweb.acw_client_path" value="/acw_client/" />``</appSettings>` |
| [ACWLanguageFileUrl](../../aspose.cells.gridweb/mainweb/acwlanguagefileurl/) { get; set; } | Obtient ou définit l'URL web du fichier de langue du contrôle. Par exemple : "/acw_client/lang_en.js". Par défaut, un fichier anglais intégré est utilisé. |
| [AutoRefreshChart](../../aspose.cells.gridweb/mainweb/autorefreshchart/) { get; set; } | Obtient ou définit si l'image du graphique est mise à jour lors de la mise à jour de la valeur de la cellule. La valeur par défaut est true |
| [BottomTableStyle](../../aspose.cells.gridweb/mainweb/bottomtablestyle/) { get; set; } | Obtient ou définit le style de la barre inférieure du contrôle. |
| [CurrentPageIndex](../../aspose.cells.gridweb/mainweb/currentpageindex/) { get; set; } | Obtient ou définit l'index de page actuel en mode pagination. |
| [CustomCalculationEngine](../../aspose.cells.gridweb/mainweb/customcalculationengine/) { get; set; } | Représente le moteur de calcul personnalisé de l'utilisateur pour étendre le moteur de calcul par défaut d'Aspose.Cells. |
| [CustomCommandButtons](../../aspose.cells.gridweb/mainweb/customcommandbuttons/) { get; } | Obtient la collection de boutons de commande personnalisés |
| [CustomStyleFileName](../../aspose.cells.gridweb/mainweb/customstylefilename/) { get; set; } | Obtient ou définit le nom du fichier de style personnalisé. |
| [DefaultFontName](../../aspose.cells.gridweb/mainweb/defaultfontname/) { get; set; } | Obtient ou définit le nom de police par défaut du contrôle. |
| [DefaultFontSize](../../aspose.cells.gridweb/mainweb/defaultfontsize/) { get; set; } | Obtient ou définit la taille de police par défaut du contrôle. |
| [DefaultGridLineColor](../../aspose.cells.gridweb/mainweb/defaultgridlinecolor/) { get; set; } | Obtient ou définit la couleur de la ligne de grille par défaut. |
| [DisplayCellTip](../../aspose.cells.gridweb/mainweb/displaycelltip/) { get; set; } | Obtient ou définit si les astuces doivent être affichées. la valeur par défaut est true. |
| [EditMode](../../aspose.cells.gridweb/mainweb/editmode/) { get; set; } | Obtient ou définit le mode d'édition du contrôle. |
| [EnableAJAX](../../aspose.cells.gridweb/mainweb/enableajax/) { get; set; } | Obtient ou définit si l'appel AJAX doit être utilisé. la valeur par défaut est true. |
| [EnableAsync](../../aspose.cells.gridweb/mainweb/enableasync/) { get; set; } | Obtient ou définit si les données des cellules sont chargées de manière asynchrone, il est suggéré de l'appliquer pour une feuille contenant plus de 10000 cellules. |
| [EnableClientColumnOperations](../../aspose.cells.gridweb/mainweb/enableclientcolumnoperations/) { get; set; } | Obtient ou définit si les opérations de colonne côté client sont activées. |
| [EnableClientFreeze](../../aspose.cells.gridweb/mainweb/enableclientfreeze/) { get; set; } | Obtient ou définit si les opérations de gel côté client sont activées. |
| [EnableClientMergeOperations](../../aspose.cells.gridweb/mainweb/enableclientmergeoperations/) { get; set; } | Obtient ou définit si les opérations de fusion côté client sont activées. |
| [EnableClientResizeColumnRow](../../aspose.cells.gridweb/mainweb/enableclientresizecolumnrow/) { get; set; } | Obtient ou définit si le redimensionnement des colonnes et des lignes côté client est activé. |
| [EnableClientRowOperations](../../aspose.cells.gridweb/mainweb/enableclientrowoperations/) { get; set; } | Obtient ou définit si les opérations de ligne côté client sont activées. |
| [EnableDoubleClickEvent](../../aspose.cells.gridweb/mainweb/enabledoubleclickevent/) { get; set; } | Obtient ou définit si l'événement double-clic côté client est activé. |
| [EnableMetalLightEffect](../../aspose.cells.gridweb/mainweb/enablemetallighteffect/) { get; set; } | Obtient ou définit si l'effet de lumière métallique doit être appliqué. |
| [EnablePaging](../../aspose.cells.gridweb/mainweb/enablepaging/) { get; set; } | Obtient ou définit si le mode de pagination du contrôle est activé. |
| [EnableStyleDialogbox](../../aspose.cells.gridweb/mainweb/enablestyledialogbox/) { get; set; } | Obtient ou définit si la boîte de dialogue de style côté client est activée. |
| [FilteredPaging](../../aspose.cells.gridweb/mainweb/filteredpaging/) { get; set; } | Obtient ou définit si la pagination après filtrage des données est activée, cela prendra effet lorsque EnablePaging est true. |
| [ForceValidation](../../aspose.cells.gridweb/mainweb/forcevalidation/) { get; set; } | Obtient ou définit si la validation côté client doit être forcée. |
| [FrameTableStyle](../../aspose.cells.gridweb/mainweb/frametablestyle/) { get; set; } | Obtient ou définit le style du cadre du contrôle. |
| [GoonDefaultSaveOperation](../../aspose.cells.gridweb/mainweb/goondefaultsaveoperation/) { get; set; } | Obtient ou définit si GridWeb effectuera l'opération d'enregistrement par défaut, la valeur par défaut est true. |
| [HeaderBarHeight](../../aspose.cells.gridweb/mainweb/headerbarheight/) { get; set; } | Obtient ou définit la hauteur (System.Web.UI.WebControl.Unit) de la barre d'en-tête supérieure du contrôle. |
| [HeaderBarStyle](../../aspose.cells.gridweb/mainweb/headerbarstyle/) { get; set; } | Obtient ou définit le style de la barre d'en-tête. |
| [HeaderBarTableStyle](../../aspose.cells.gridweb/mainweb/headerbartablestyle/) { get; set; } | Obtient ou définit le style de la barre d'en-tête du contrôle. |
| [HeaderBarWidth](../../aspose.cells.gridweb/mainweb/headerbarwidth/) { get; set; } | Obtient ou définit la largeur (System.Web.UI.WebControl.Unit) ou la barre d'en-tête gauche du contrôle. |
| override [Height](../../aspose.cells.gridweb/mainweb/height/) { get; set; } | Obtient ou définit la hauteur (System.Web.UI.WebControl.Unit) du contrôle. |
| [IgnoreStyleWithNoData](../../aspose.cells.gridweb/mainweb/ignorestylewithnodata/) { get; set; } | Obtient ou définit si GridWeb ignore l'affichage des lignes ou colonnes qui ne contiennent pas de valeurs de cellule mais qui sont tout de même stylisées. Si la valeur est true, les performances seront meilleures. La valeur par défaut est false, ce qui signifie que si la dernière ligne/colonne consécutive n'a pas de valeurs de cellule mais est stylisée, nous les afficherons quand même. Cette option n'est valable que lorsque EnableAsync est false. Cette option n'a aucun effet lorsque EnableAsync est true, ce qui signifie que GridWeb affichera toutes les lignes/colonnes avec style. |
| [IsCalculateFormula](../../aspose.cells.gridweb/mainweb/iscalculateformula/) { get; set; } | Obtient ou définit s'il faut calculer la formule après les changements de valeur de cellule ou après l'importation du fichier. La valeur par défaut est true. |
| [IsPostBack](../../aspose.cells.gridweb/mainweb/ispostback/) { get; } | Obtient une valeur indiquant si gridweb est chargé en réponse à un postback client, ou s'il est chargé et accédé pour la première fois. |
| [LoadOptions](../../aspose.cells.gridweb/mainweb/loadoptions/) { get; set; } | Représente les options de chargement pour GridWeb. |
| [MaxColumn](../../aspose.cells.gridweb/mainweb/maxcolumn/) { get; set; } | Obtient ou définit l'index maximal de colonne affichée (basé sur zéro) de la feuille Web. Le contrôle utilise la plus grande valeur entre MaxColumn et la colonne maximale des données de la feuille. |
| [MaxRow](../../aspose.cells.gridweb/mainweb/maxrow/) { get; set; } | Obtient ou définit l'index maximal de ligne affichée (basé sur zéro) de la feuille Web. Le contrôle utilise la plus grande valeur entre MaxRow et la ligne maximale des données de la feuille. |
| [Message](../../aspose.cells.gridweb/mainweb/message/) { get; set; } | Obtient ou définit le message pour la grille. |
| [MinColumn](../../aspose.cells.gridweb/mainweb/mincolumn/) { get; set; } | Obtient ou définit l'index minimal de colonne affichée (basé sur zéro) de la feuille Web. Le contrôle utilise la plus petite valeur entre MinColumn et la colonne minimale des données de la feuille. |
| [MinRow](../../aspose.cells.gridweb/mainweb/minrow/) { get; set; } | Obtient ou définit l'index minimal de ligne affichée (basé sur zéro) de la feuille Web. Le contrôle utilise la plus petite valeur entre MinRow et la ligne minimale des données de la feuille. |
| [ModifiedCells](../../aspose.cells.gridweb/mainweb/modifiedcells/) { get; } | Obtient la collection des cellules modifiées par le client. |
| [NeedRenderGroupRows](../../aspose.cells.gridweb/mainweb/needrendergrouprows/) { get; set; } | Obtient ou définit s'il faut afficher les grouprows . |
| [NoHScroll](../../aspose.cells.gridweb/mainweb/nohscroll/) { get; set; } | Obtient ou définit une valeur indiquant si la barre de défilement horizontale est masquée. |
| [NoScroll](../../aspose.cells.gridweb/mainweb/noscroll/) { get; set; } | Obtient ou définit s'il faut afficher la barre de défilement . |
| [NoVScroll](../../aspose.cells.gridweb/mainweb/novscroll/) { get; set; } | Obtient ou définit une valeur indiquant si la barre de défilement verticale est masquée. |
| [OnAjaxCallFinishedClientFunction](../../aspose.cells.gridweb/mainweb/onajaxcallfinishedclientfunction/) { get; set; } | Obtient ou définit le nom de la fonction côté client à appeler lorsque l'appel ajax est terminé. La fonction client doit être déclarée ainsi : function GridAjaxcallFinished() { alert(this.id+" ajaxcall finished "); } Note : Vous pouvez utiliser le pointeur "this" dans la fonction client pour référencer le contrôle de grille qui déclenche l'événement. |
| [OnCellErrorClientFunction](../../aspose.cells.gridweb/mainweb/oncellerrorclientfunction/) { get; set; } | Obtient ou définit le nom de la fonction côté client à appeler lorsqu'une validation de cellule échoue. La fonction client doit être déclarée ainsi : function MyOnCellError(cell) { alert(this.getCellValueByCell(cell)); } Note : Vous pouvez utiliser le pointeur "this" dans la fonction client pour référencer le contrôle de grille qui déclenche l'événement. |
| [OnCellSelectedAjaxCallBackClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedajaxcallbackclientfunction/) { get; set; } | Obtient ou définit la fonction côté client à appeler lorsqu'une cellule est sélectionnée. La fonction client doit être déclarée ainsi : function MyOnSelectCellAjaxCallBack(cell,customerdata) { } Note : Vous pouvez utiliser le pointeur "this" dans la fonction client pour référencer le contrôle de grille qui déclenche l'événement. |
| [OnCellSelectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedclientfunction/) { get; set; } | Obtient ou définit la fonction côté client à appeler lorsqu'une cellule est sélectionnée. La fonction client doit être déclarée ainsi : function MyOnSelectCell(cell) { GridWeb1.setCellValueByCell(cell, "test"); } Note : Vous pouvez utiliser le pointeur "this" dans la fonction client pour référencer le contrôle de grille qui déclenche l'événement. |
| [OnCellUnselectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellunselectedclientfunction/) { get; set; } | Obtient ou définit la fonction côté client à appeler lorsqu'une cellule est désélectionnée. La fonction client doit être déclarée ainsi : function MyOnUnselectCell(cell) { this.setCellValueByCell(cell, "test"); } Note : Vous pouvez utiliser le pointeur "this" dans la fonction client pour référencer le contrôle de grille qui déclenche l'événement. |
| [OnCellUpdatedClientFunction](../../aspose.cells.gridweb/mainweb/oncellupdatedclientfunction/) { get; set; } | Obtient ou définit le nom de la fonction côté client à appeler lorsqu'une valeur de cellule est mise à jour. La fonction client doit être déclarée ainsi : function MyOnCellUpdated(cell) { alert(this.getCellValueByCell(cell)); } Note : Vous pouvez utiliser le pointeur "this" dans la fonction client pour référencer le contrôle de grille qui déclenche l'événement. |
| [OnContextMenuShowClientFunction](../../aspose.cells.gridweb/mainweb/oncontextmenushowclientfunction/) { get; set; } | Obtient ou définit la fonction côté client à appeler lorsque le menu contextuel sera affiché. La fonction client doit être déclarée ainsi : function onContextMenuShow() { var menu = event.srcElement; menu.setItemVisibility(\"Delete\", \"block\"); menu.setItemVisibility(\"Update\", \"none\"); }Note : Vous pouvez utiliser le pointeur \"this\" dans la fonction client pour référencer le contrôle de grille qui déclenche l'événement. |
| [OnDoubleClickCellClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickcellclientfunction/) { get; set; } | Obtient ou définit la fonction côté client à appeler lorsqu'une cellule est double-cliquée. La fonction client doit être déclarée ainsi : function MyOnDoubleClickCell(cell) { this.setCellValueByCell(cell, \"test\"); }Note : Vous pouvez utiliser le pointeur \"this\" dans la fonction client pour référencer le contrôle de grille qui déclenche l'événement. |
| [OnDoubleClickRowClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickrowclientfunction/) { get; set; } | Obtient ou définit la fonction côté client à appeler lorsqu'une ligne est double-cliquée. La fonction client doit être déclarée ainsi : function MyOnRowDoubleClick(row) { alert(row); }Note : Vous pouvez utiliser le pointeur \"this\" dans la fonction client pour référencer le contrôle de grille qui déclenche l'événement. |
| [OnGridInitClientFunction](../../aspose.cells.gridweb/mainweb/ongridinitclientfunction/) { get; set; } | Obtient ou définit le nom de la fonction côté client à appeler lorsque la grille est initialisée. La fonction client doit être déclarée ainsi : function MyOnGridInit(grid) { alert(\"The grid is initialized: \" + grid.id); }Note : Vous pouvez utiliser le pointeur \"this\" dans la fonction client pour référencer le contrôle de grille qui déclenche l'événement. |
| [OnlyAuto](../../aspose.cells.gridweb/mainweb/onlyauto/) { get; set; } | Obtient ou définit si seules les lignes dont la hauteur n'est pas personnalisée sont ajustées, la valeur par défaut est false |
| [OnPageChangeClientFunction](../../aspose.cells.gridweb/mainweb/onpagechangeclientfunction/) { get; set; } | Obtient ou définit la fonction côté client à appeler après le changement d'index de page. Ne prend effet que lorsque EnablePaging est true. La fonction client doit être déclarée ainsi : function MyOnPageChange(index) { console.log(\"current page is:\"+index); }Note : Vous pouvez utiliser le pointeur \"this\" dans la fonction client pour référencer le contrôle de grille qui déclenche l'événement. |
| [OnPageSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onpagesubmitclientfunction/) { get; set; } | Obtient ou définit la fonction client à appeler avant que la page ne soit soumise côté client. |
| [OnShapeSelectedClientFunction](../../aspose.cells.gridweb/mainweb/onshapeselectedclientfunction/) { get; set; } | Obtient ou définit la fonction côté client à appeler lorsqu'une forme est sélectionnée. La fonction client doit être déclarée ainsi : function MyOnSelectShape(shape) { var name=shape.getAttribute(\"namevalue\") var text=shape.getAttribute(\"textvalue\") var value=shape.getAttribute(\"controlvalue\") var type=shape.getAttribute(\"msotype\") }Note : Vous pouvez utiliser le pointeur \"this\" dans la fonction client pour référencer le contrôle de grille qui déclenche l'événement. |
| [OnSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onsubmitclientfunction/) { get; set; } | Obtient ou définit la fonction client à appeler avant que le contrôle ne soit soumis côté client. La fonction client doit être déclarée ainsi : function MyOnSubmit(arg, cancelEdit) { return true;} L'argument arg est l'argument de soumission, contenant la commande à envoyer au serveur. Le booléen cancelEdit indique si le contrôle a abandonné l'entrée utilisateur avant la soumission. Le contrôle continuera à soumettre si la fonction renvoie true. Note : Vous pouvez utiliser le pointeur \"this\" dans la fonction client pour référencer le contrôle de grille qui déclenche l'événement. |
| [PageSize](../../aspose.cells.gridweb/mainweb/pagesize/) { get; set; } | Obtient ou définit la taille de page en mode pagination. |
| [PresetStyle](../../aspose.cells.gridweb/mainweb/presetstyle/) { get; set; } | Obtient ou définit le style prédéfini. |
| [RefreshValidation](../../aspose.cells.gridweb/mainweb/refreshvalidation/) { get; set; } | Obtient ou définit s'il faut rafraîchir la valeur de validation après les changements de valeur de cellule. |
| [RenderHiddenRow](../../aspose.cells.gridweb/mainweb/renderhiddenrow/) { get; set; } | Obtient ou définit si la ligne masquée est rendue dans GridControl, la valeur par défaut est false. Si vous devez réafficher la ligne masquée ultérieurement, vous devez la définir sur true. |
| [RowHeightForCSV](../../aspose.cells.gridweb/mainweb/rowheightforcsv/) { get; set; } | Obtient ou définit la valeur de hauteur de ligne en points pour le fichier csv, la valeur par défaut est 14.5. |
| [ScrollBarArrowColor](../../aspose.cells.gridweb/mainweb/scrollbararrowcolor/) { get; set; } | Spécifie la couleur du bouton flèche de la barre de défilement. |
| [ScrollBarBaseColor](../../aspose.cells.gridweb/mainweb/scrollbarbasecolor/) { get; set; } | Spécifie la couleur de la barre de défilement du contrôle. |
| [SelectCellBgColor](../../aspose.cells.gridweb/mainweb/selectcellbgcolor/) { get; set; } | Spécifie la couleur d'arrière-plan des cellules sélectionnées dans la plage à sélection multiple. |
| [SelectCellColor](../../aspose.cells.gridweb/mainweb/selectcellcolor/) { get; set; } | Spécifie la couleur des cellules sélectionnées dans la plage à sélection multiple. |
| [SessionMode](../../aspose.cells.gridweb/mainweb/sessionmode/) { get; set; } | Obtient ou définit le mode de session de la grille. |
| [SessionStorePath](../../aspose.cells.gridweb/mainweb/sessionstorepath/) { get; set; } | Obtient ou définit le chemin de stockage du cache de session lorsque le mode de session est File ou ViewState, etc. : gridweb.SessionStorePath=\"c:/mytempdir/session\"; alors les données de session seront stockées dans c:/mytempdir/session |
| [Settings](../../aspose.cells.gridweb/mainweb/settings/) { get; set; } | Représente les paramètres du classeur. |
| [ShowAddButton](../../aspose.cells.gridweb/mainweb/showaddbutton/) { get; set; } | Obtient ou définit s'il faut afficher le bouton d'ajout de feuille de calcul. |
| [ShowBottomBar](../../aspose.cells.gridweb/mainweb/showbottombar/) { get; set; } | Spécifie s'il faut afficher la barre de commande (inclut la barre de commande et la barre d'onglets) en bas du contrôle. |
| [ShowCellEditBox](../../aspose.cells.gridweb/mainweb/showcelleditbox/) { get; set; } | Indique si Gridweb affiche la barre d'outils de zone de texte comme dans MS-EXCEL. Si activé, une zone de texte pour la cellule actuelle sera affichée dans Gridweb. Si nous activons cette fonctionnalité, nous devons importer la bibliothèque jquery js dans vos fichiers aspx pour prendre en charge cette nouvelle fonctionnalité. Toutes les dernières versions de jquery sont compatibles, etc. |
| [ShowCommandBarAtTop](../../aspose.cells.gridweb/mainweb/showcommandbarattop/) { get; set; } | Spécifie si la barre de commande (inclut la barre de commande et la barre d'onglets) doit être affichée en haut du contrôle. |
| [ShowContextMenu](../../aspose.cells.gridweb/mainweb/showcontextmenu/) { get; set; } | Obtient ou définit si le menu contextuel doit être affiché. La valeur par défaut est true. |
| [ShowDefaultGridLine](../../aspose.cells.gridweb/mainweb/showdefaultgridline/) { get; set; } | Obtient ou définit si les lignes de grille par défaut des cellules doivent être affichées. |
| [ShowHeaderBar](../../aspose.cells.gridweb/mainweb/showheaderbar/) { get; set; } | Obtient ou définit si la barre d'en-tête doit être affichée |
| [ShowLoading](../../aspose.cells.gridweb/mainweb/showloading/) { get; set; } | Spécifie si une boîte de dialogue de chargement doit être affichée pendant le postback vers le serveur. |
| [ShowLoadingPosition](../../aspose.cells.gridweb/mainweb/showloadingposition/) { get; set; } | Spécifie la position gauche, haut (en px) pour afficher la boîte de dialogue de chargement pendant le postback vers le serveur, etc. 100,200 signifie que la position gauche, haut de la boîte de dialogue de chargement est à 100px,200px. |
| [ShowSaveButton](../../aspose.cells.gridweb/mainweb/showsavebutton/) { get; set; } | Obtient ou définit si le bouton d'enregistrement doit être affiché. |
| [ShowSubmitButton](../../aspose.cells.gridweb/mainweb/showsubmitbutton/) { get; set; } | Obtient ou définit si le bouton de soumission doit être affiché. |
| [ShowTabBar](../../aspose.cells.gridweb/mainweb/showtabbar/) { get; set; } | Obtient ou définit si la barre d'onglets doit être affichée. |
| [ShowTabNavigation](../../aspose.cells.gridweb/mainweb/showtabnavigation/) { get; set; } | Obtient ou définit si le bouton de navigation des onglets est affiché, la valeur par défaut est true. |
| [ShowUndoButton](../../aspose.cells.gridweb/mainweb/showundobutton/) { get; set; } | Obtient ou définit si le bouton d'annulation doit être affiché. |
| [SpanWrap](../../aspose.cells.gridweb/mainweb/spanwrap/) { get; set; } | Spécifie si le contenu doit être enveloppé dans la portée de cellule. La valeur par défaut est true. |
| [TabStyle](../../aspose.cells.gridweb/mainweb/tabstyle/) { get; set; } | Obtient ou définit le style de la barre d'onglets. |
| [UseClientPageHeight](../../aspose.cells.gridweb/mainweb/useclientpageheight/) { get; set; } | Obtient ou définit si GridWeb utilise la hauteur de la page client comme hauteur du contrôle, adapté lorsque Height=\"100%\" est défini, la valeur par défaut est false. |
| [ViewPanelScrollLeft](../../aspose.cells.gridweb/mainweb/viewpanelscrollleft/) { get; set; } | Obtient ou définit la position de la barre de défilement du panneau de visualisation de la grille. |
| [ViewPanelScrollTop](../../aspose.cells.gridweb/mainweb/viewpanelscrolltop/) { get; set; } | Obtient ou définit la position de la barre de défilement du panneau de visualisation de la grille. |
| [ViewTableStyle](../../aspose.cells.gridweb/mainweb/viewtablestyle/) { get; set; } | Obtient ou définit le style du panneau de visualisation des données. |
| [WebWorksheets](../../aspose.cells.gridweb/mainweb/webworksheets/) { get; } |  |
| override [Width](../../aspose.cells.gridweb/mainweb/width/) { get; set; } | Obtient ou définit la largeur (System.Web.UI.WebControl.Unit) du contrôle. |
| [WorkSheets](../../aspose.cells.gridweb/mainweb/worksheets/) { get; } | Obtient ou définit la collection des feuilles de calcul. |
| [XhtmlMode](../../aspose.cells.gridweb/mainweb/xhtmlmode/) { get; set; } | Obtient ou définit si le style XHTML doit être utilisé, la valeur par défaut est true. |
| static [DPI](../../aspose.cells.gridweb/mainweb/dpi/) { get; set; } | Obtient / Définit le DPI de la machine. |
| static [PictureCachePath](../../aspose.cells.gridweb/mainweb/picturecachepath/) { get; set; } | Obtient ou définit le chemin de stockage des images pour le classeur, toutes les formes et images seront stockées dans ce répertoire, le chemin par défaut est acwcache sous le répertoire de base de l'application actuelle ; les utilisateurs doivent mettre en place un service planifié pour nettoyer les fichiers dont la durée de session est expirée. |

## Méthodes

| Nom | Description |
| --- | --- |
| [CalculateFormula](../../aspose.cells.gridweb/mainweb/calculateformula/)() | Calcule le résultat des formules. |
| override [DataBind](../../aspose.cells.gridweb/mainweb/databind/)() | Liez le contrôle et tous ses contrôles enfants à sa source de données. |
| override [Dispose](../../aspose.cells.gridweb/mainweb/dispose/)() |  |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile)(Stream) | Importe depuis un flux de fichier Excel, y compris un flux de fichier disque ou un flux mémoire. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_2)(string) | Importe depuis un fichier Excel. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_1)(Stream, string) | Importe depuis un flux de fichier Excel, y compris un flux de fichier disque ou un flux mémoire. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_3)(string, string) | Importe depuis un fichier Excel. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile/#loadcsvfile)(Stream) | Charge les données depuis un flux de fichier CSV. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile/#loadcsvfile_1)(string) | Charge les données depuis un fichier CSV. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile/#loadhtmlfile)(Stream) | Charge les données depuis un flux de fichier HTML. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile/#loadhtmlfile_1)(string) | Charge les données depuis un fichier HTML. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile/#loadspreadsheetmlfile)(Stream) | Charge les données depuis un flux de fichier SpreadSheetML. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile/#loadspreadsheetmlfile_1)(string) | Charge les données depuis un fichier SpreadSheetML. |
| [RefreshChartShape](../../aspose.cells.gridweb/mainweb/refreshchartshape/)() | Actualisez toutes les images de graphiques pour la feuille de calcul active. |
| override [RenderBeginTag](../../aspose.cells.gridweb/mainweb/renderbegintag/)(HtmlTextWriter) |  |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile/#savecsvfile)(Stream) | Enregistre les données dans un flux de fichier CSV. |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile/#savecsvfile_1)(string) | Enregistre les données dans un fichier CSV. |
| [SaveCustomStyleFile](../../aspose.cells.gridweb/mainweb/savecustomstylefile/)(string) | Enregistre les données de style actuelles du contrôle dans un fichier XML. Peut être utilisé pour créer votre fichier de style personnalisé. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile/#savehtmlfile)(Stream) | Enregistre les données dans un flux de fichier HTML. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile/#savehtmlfile_1)(string) | Enregistre les données dans un fichier HTML. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile/#savespreadsheetmlfile)(Stream) | Enregistre les données dans un flux de fichier SpreadSheetML. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile/#savespreadsheetmlfile_1)(string) | Enregistre les données dans un fichier SpreadSheetML. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile)(Stream) | Enregistre les feuilles de calcul dans un fichier Excel. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_3)(string) | Enregistre les feuilles de calcul dans un fichier Excel au format Excel 2003. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_1)(Stream, GridSaveFormat) | Enregistre les feuilles de calcul dans un fichier Excel. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_2)(Stream, GridSaveOptions) | Enregistre les feuilles de calcul dans un fichier Excel. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_4)(string, GridSaveFormat) | Enregistre les feuilles de calcul dans un fichier Excel. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_5)(string, GridSaveOptions) | Enregistre les feuilles de calcul dans un fichier Excel. |
| [SetCustomStyle](../../aspose.cells.gridweb/mainweb/setcustomstyle/)(Stream) | Définit le fichier de style personnalisé à partir d'un flux, y compris le flux de fichier disque ou le flux mémoire. |

## Événements

| Nom | Description |
| --- | --- |
| event [AfterColumnFilter](../../aspose.cells.gridweb/mainweb/aftercolumnfilter/) | Se produit après le filtrage de la colonne. |
| event [AjaxCallFinished](../../aspose.cells.gridweb/mainweb/ajaxcallfinished/) | Se déclenche lorsque la mise à jour ajax du contrôle est terminée.(le EnableAJAX doit être défini sur true) |
| event [BeforeColumnFilter](../../aspose.cells.gridweb/mainweb/beforecolumnfilter/) | Se produit avant la colonne à filtrer. |
| event [CellClickOnAjax](../../aspose.cells.gridweb/mainweb/cellclickonajax/) | Se produit lorsque la cellule est cliquée, et nécessite un ajaxcallback pour cet événement. |
| event [CellClientUpdate](../../aspose.cells.gridweb/mainweb/cellclientupdate/) | Se produit lorsqu'une mise à jour de cellule client se produit. Lorsque cet événement est déclenché, son paramètre e.Argument contient le nom de la commande. |
| event [CellCommand](../../aspose.cells.gridweb/mainweb/cellcommand/) | Se produit lorsque le lien hypertexte de commande d'une cellule est cliqué. Lorsque cet événement est déclenché, son paramètre e.Argument contient le nom de la commande. |
| event [CellDoubleClick](../../aspose.cells.gridweb/mainweb/celldoubleclick/) | Se produit lorsque la cellule est double-cliquée. |
| event [CellError](../../aspose.cells.gridweb/mainweb/cellerror/) | Se produit lorsqu'il y a une erreur de valeur d'entrée dans la cellule. |
| event [CellModifiedOnAjax](../../aspose.cells.gridweb/mainweb/cellmodifiedonajax/) | Se produit lorsque la cellule est modifiée dans ajaxcall. |
| event [ColumnDeleted](../../aspose.cells.gridweb/mainweb/columndeleted/) | Se produit lorsque l'utilisateur supprime une colonne depuis le menu côté client. |
| event [ColumnDeleting](../../aspose.cells.gridweb/mainweb/columndeleting/) | Se produit lorsque l'utilisateur tente de supprimer une colonne depuis le menu côté client. Vous pouvez gérer cet événement et définir le paramètre cancel sur True pour annuler l'opération de suppression. |
| event [ColumnDoubleClick](../../aspose.cells.gridweb/mainweb/columndoubleclick/) | Se produit lorsque l'en-tête de colonne est double-cliqué. |
| event [ColumnInserted](../../aspose.cells.gridweb/mainweb/columninserted/) | Se produit lorsque l'utilisateur insère une colonne depuis le menu côté client. |
| event [CustomCommand](../../aspose.cells.gridweb/mainweb/customcommand/) | Se produit lorsque l'utilisateur clique sur un bouton de commande personnalisé. |
| event [LoadCustomData](../../aspose.cells.gridweb/mainweb/loadcustomdata/) | Se déclenche lorsque le SessionMode du contrôle est défini sur Custom et doit charger les données de la feuille. Vous pouvez gérer cet événement en mode Session personnalisé pour charger les données de la feuille depuis un fichier ou une base de données. |
| event [PageIndexChanged](../../aspose.cells.gridweb/mainweb/pageindexchanged/) | Se produit lorsque l'index de page de la feuille du contrôle a changé. |
| event [RowDeleted](../../aspose.cells.gridweb/mainweb/rowdeleted/) | Se produit lorsque l'utilisateur a supprimé une ligne depuis le menu côté client. |
| event [RowDeleting](../../aspose.cells.gridweb/mainweb/rowdeleting/) | Se produit lorsque l'utilisateur tente de supprimer une ligne depuis le menu côté client. Vous pouvez gérer cet événement et lancer une exception RejectDeleteException pour annuler l'opération de suppression. |
| event [RowDoubleClick](../../aspose.cells.gridweb/mainweb/rowdoubleclick/) | Se produit lorsque l'en-tête de ligne est double-cliqué. |
| event [RowInserted](../../aspose.cells.gridweb/mainweb/rowinserted/) | Se produit lorsque l'utilisateur insère une ligne depuis le menu côté client. |
| event [SaveCommand](../../aspose.cells.gridweb/mainweb/savecommand/) | Se produit lorsque le bouton \"save\" est cliqué. |
| event [SheetAdded](../../aspose.cells.gridweb/mainweb/sheetadded/) | Se produit lorsque l'utilisateur ajoute une feuille de calcul depuis le menu de la barre d'outils. |
| event [SheetDataUpdated](../../aspose.cells.gridweb/mainweb/sheetdataupdated/) | Se produit lorsque le contrôle a chargé les données postées et mis à jour les données de la feuille. |
| event [SheetTabClick](../../aspose.cells.gridweb/mainweb/sheettabclick/) | Se produit lorsque l'onglet de la feuille est cliqué. |
| event [SubmitCommand](../../aspose.cells.gridweb/mainweb/submitcommand/) | Se produit lorsque le bouton \"submit\" est cliqué. |
| event [UndoCommand](../../aspose.cells.gridweb/mainweb/undocommand/) | Se produit lorsque le bouton "undo" est cliqué. |

### Exemples

```csharp
[C#]
	GridWeb GridWeb1 = new GridWeb();
//faites votre travail
```

### Voir aussi

* class [ExtWebControl](../extwebcontrol/)
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


