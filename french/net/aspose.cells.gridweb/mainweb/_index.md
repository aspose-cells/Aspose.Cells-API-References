---
title: MainWeb
second_title: Référence de l'API Aspose.Cells pour .NET
description: Classe parent du contrôle GridWeb.Usage interne uniquement.
type: docs
weight: 850
url: /fr/net/aspose.cells.gridweb/mainweb/
---
## MainWeb class

Classe parent du contrôle GridWeb.Usage interne uniquement.

```csharp
public class MainWeb : ExtWebControl, INamingContainer, IPostBackDataHandler, 
    IPostBackEventHandler, ISerializable
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [MainWeb](mainweb)() | Default_Constructor |

## Propriétés

| Nom | La description |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb/mainweb/activecell) { get; set; } | Obtient ou définit la cellule active de la feuille actuelle. Modifié pour être accessible en écriture depuis la version 1.9.0.1. |
| [ActiveCellBgColor](../../aspose.cells.gridweb/mainweb/activecellbgcolor) { get; set; } | Spécifie la couleur d'arrière-plan de la cellule active. |
| [ActiveCellColor](../../aspose.cells.gridweb/mainweb/activecellcolor) { get; set; } | Spécifie la couleur de la cellule active. |
| [ActiveHeaderBgColor](../../aspose.cells.gridweb/mainweb/activeheaderbgcolor) { get; set; } | Spécifie la couleur d'arrière-plan de l'en-tête de ligne/colonne actif. |
| [ActiveHeaderColor](../../aspose.cells.gridweb/mainweb/activeheadercolor) { get; set; } | Spécifie la couleur de l'en-tête de ligne/colonne actif. |
| [ActiveSheet](../../aspose.cells.gridweb/mainweb/activesheet) { get; } | Obtient la feuille active |
| [ActiveSheetIndex](../../aspose.cells.gridweb/mainweb/activesheetindex) { get; set; } | Obtient ou définit l'index de la feuille active. Égal à WebWorksheets.ActiveSheetIndex. |
| [ActiveTabStyle](../../aspose.cells.gridweb/mainweb/activetabstyle) { get; set; } | Spécifie le style de l'onglet actif. |
| [ACWClientPath](../../aspose.cells.gridweb/mainweb/acwclientpath) { get; set; } | Obtient ou définit le chemin Web des fichiers de script/image du contrôle. Par exemple : "http://localhost/acw_client". Vous pouvez également définir cette valeur dans le fichier web.config. Ajoutez cette section à la section &lt;configuration&gt; : &lt;appSettings&gt;&lt;add key="aspose.cells.gridweb.acw_client_path" value="/acw_client/" /&gt;&lt;/appSettings&gt; |
| [ACWLanguageFileUrl](../../aspose.cells.gridweb/mainweb/acwlanguagefileurl) { get; set; } | Obtient ou définit l'URL Web du fichier de langue du contrôle. Par exemple : "/acw_client/lang_en.js". Par défaut, un fichier anglais intégré est utilisé. |
| [AutoRefreshChart](../../aspose.cells.gridweb/mainweb/autorefreshchart) { get; set; } | Obtient ou définit si l'image du graphique est mise à jour lors de la mise à jour de la valeur de la cellule. La valeur par défaut est true |
| [BottomTableStyle](../../aspose.cells.gridweb/mainweb/bottomtablestyle) { get; set; } | Obtient ou définit le style de la barre inférieure du contrôle. |
| [CurrentPageIndex](../../aspose.cells.gridweb/mainweb/currentpageindex) { get; set; } |  |
| [CustomCalculationEngine](../../aspose.cells.gridweb/mainweb/customcalculationengine) { get; set; } | Représente le moteur de calcul personnalisé de l'utilisateur pour étendre le moteur de calcul par défaut d'Aspose.Cells. |
| [CustomCommandButtons](../../aspose.cells.gridweb/mainweb/customcommandbuttons) { get; } |  |
| [CustomStyleFileName](../../aspose.cells.gridweb/mainweb/customstylefilename) { get; set; } | Obtient ou définit le nom du fichier de style personnalisé. |
| [DefaultFontName](../../aspose.cells.gridweb/mainweb/defaultfontname) { get; set; } | Obtient ou définit le nom de la police par défaut du contrôle. |
| [DefaultFontSize](../../aspose.cells.gridweb/mainweb/defaultfontsize) { get; set; } | Obtient ou définit la taille de police par défaut du contrôle. |
| [DefaultGridLineColor](../../aspose.cells.gridweb/mainweb/defaultgridlinecolor) { get; set; } | Obtient ou définit la couleur de la ligne de grille par défaut. |
| [DisplayCellTip](../../aspose.cells.gridweb/mainweb/displaycelltip) { get; set; } |  |
| [EditMode](../../aspose.cells.gridweb/mainweb/editmode) { get; set; } | Obtient ou définit le mode d'édition du contrôle. |
| [EnableAJAX](../../aspose.cells.gridweb/mainweb/enableajax) { get; set; } |  |
| [EnableAsync](../../aspose.cells.gridweb/mainweb/enableasync) { get; set; } | Obtient ou définit si les données des cellules de charge de manière asynchrone, suggèrent d'appliquer pour une feuille avec plus de 10000 cellules. |
| [EnableClientColumnOperations](../../aspose.cells.gridweb/mainweb/enableclientcolumnoperations) { get; set; } | Obtient ou définit s'il faut activer les opérations de colonne côté client. |
| [EnableClientFreeze](../../aspose.cells.gridweb/mainweb/enableclientfreeze) { get; set; } | Obtient ou définit s'il faut activer les opérations de gel côté client. |
| [EnableClientMergeOperations](../../aspose.cells.gridweb/mainweb/enableclientmergeoperations) { get; set; } | Obtient ou définit s'il faut activer les opérations de fusion côté client. |
| [EnableClientResizeColumnRow](../../aspose.cells.gridweb/mainweb/enableclientresizecolumnrow) { get; set; } | Obtient ou définit s'il faut activer la colonne et la ligne de redimensionnement côté client. |
| [EnableClientRowOperations](../../aspose.cells.gridweb/mainweb/enableclientrowoperations) { get; set; } | Obtient ou définit s'il faut activer les opérations de ligne côté client. |
| [EnableDoubleClickEvent](../../aspose.cells.gridweb/mainweb/enabledoubleclickevent) { get; set; } | Obtient ou définit s'il faut activer l'événement de double-clic côté client. |
| [EnableMetalLightEffect](../../aspose.cells.gridweb/mainweb/enablemetallighteffect) { get; set; } | Obtient ou définit s'il faut appliquer un effet de lumière métallique. |
| [EnablePaging](../../aspose.cells.gridweb/mainweb/enablepaging) { get; set; } | Obtient ou définit s'il faut activer le mode de pagination du contrôle. |
| [EnableStyleDialogbox](../../aspose.cells.gridweb/mainweb/enablestyledialogbox) { get; set; } | Obtient ou définit s'il faut activer la boîte de dialogue de style côté client. |
| [FilteredPaging](../../aspose.cells.gridweb/mainweb/filteredpaging) { get; set; } | Obtient ou définit s'il faut activer la pagination après le filtrage des données, prendra effet lorsque EnablePaging est vrai. |
| [ForceValidation](../../aspose.cells.gridweb/mainweb/forcevalidation) { get; set; } | Obtient ou définit s'il faut forcer la validation côté client. |
| [FrameTableStyle](../../aspose.cells.gridweb/mainweb/frametablestyle) { get; set; } | Obtient ou définit le style de cadre du contrôle. |
| [GoonDefaultSaveOperation](../../aspose.cells.gridweb/mainweb/goondefaultsaveoperation) { get; set; } | Obtient ou définit si GridWeb effectuera l'opération d'enregistrement par défaut, la valeur par défaut est true. |
| [HeaderBarHeight](../../aspose.cells.gridweb/mainweb/headerbarheight) { get; set; } | Obtient ou définit la hauteur ( System.Web.UI.WebControl.Unit ) de la barre d'en-tête supérieure du contrôle. |
| [HeaderBarStyle](../../aspose.cells.gridweb/mainweb/headerbarstyle) { get; set; } | Obtient ou définit le style de la barre d'en-tête. |
| [HeaderBarTableStyle](../../aspose.cells.gridweb/mainweb/headerbartablestyle) { get; set; } | Obtient ou définit le style de la barre d'en-tête du contrôle. |
| [HeaderBarWidth](../../aspose.cells.gridweb/mainweb/headerbarwidth) { get; set; } | Obtient ou définit la largeur ( System.Web.UI.WebControl.Unit ) ou la barre d'en-tête gauche du contrôle. |
| override [Height](../../aspose.cells.gridweb/mainweb/height) { get; set; } | Obtient ou définit la hauteur ( System.Web.UI.WebControl.Unit ) du contrôle. |
| [IsCalculateFormula](../../aspose.cells.gridweb/mainweb/iscalculateformula) { get; set; } | Obtient ou définit s'il faut calculer la formule après la modification de la valeur de la cellule ou après l'importation du fichier. La valeur par défaut est true. |
| [IsPostBack](../../aspose.cells.gridweb/mainweb/ispostback) { get; } | Obtient une valeur indiquant si gridweb est chargé en réponse à une publication client, ou s'il est chargé et accédé pour la première fois. |
| [LinksTable](../../aspose.cells.gridweb/mainweb/linkstable) { get; } |  |
| [MaxColumn](../../aspose.cells.gridweb/mainweb/maxcolumn) { get; set; } | Obtient ou définit l'index de colonne d'affichage maximal (basé sur zéro) de la feuille Web. Le contrôle utilise la valeur la plus élevée de MaxColumn et la colonne maximale des données de feuille. |
| [MaxRow](../../aspose.cells.gridweb/mainweb/maxrow) { get; set; } | Obtient ou définit l'index de ligne d'affichage maximal (basé sur zéro) de la feuille Web. Le contrôle utilise la valeur la plus élevée de MaxRow et la ligne maximale des données de feuille. |
| [Message](../../aspose.cells.gridweb/mainweb/message) { get; set; } |  |
| [MinColumn](../../aspose.cells.gridweb/mainweb/mincolumn) { get; set; } |  |
| [MinRow](../../aspose.cells.gridweb/mainweb/minrow) { get; set; } | Obtient ou définit l'index de ligne d'affichage minimum (basé sur zéro) de la feuille Web. Le contrôle utilise la plus petite valeur de MinRow et la ligne min des données de la feuille. |
| [ModifiedCells](../../aspose.cells.gridweb/mainweb/modifiedcells) { get; } | Obtient la collection des cellules modifiées par le client. |
| [NeedRenderGroupRows](../../aspose.cells.gridweb/mainweb/needrendergrouprows) { get; set; } | Obtient ou définit s'il faut afficher les lignes de groupe . |
| [NoHScroll](../../aspose.cells.gridweb/mainweb/nohscroll) { get; set; } | Obtient ou définit une valeur indiquant si la barre de défilement horizontale est masquée. |
| [NoScroll](../../aspose.cells.gridweb/mainweb/noscroll) { get; set; } |  |
| [NoVScroll](../../aspose.cells.gridweb/mainweb/novscroll) { get; set; } | Obtient ou définit une valeur indiquant si la barre de défilement verticale est masquée. |
| [OnAjaxCallFinishedClientFunction](../../aspose.cells.gridweb/mainweb/onajaxcallfinishedclientfunction) { get; set; } | Obtient ou définit le nom de la fonction côté client à appeler lorsque l'appel ajax est terminé. La fonction client doit être déclarée comme ceci : fonction GridAjaxcallFinished() { alert(this.id+" appel ajax terminé "); } Remarque : Vous pouvez utiliser le pointeur "this" dans la fonction client pour pointer le contrôle de grille qui déclenche l'événement. |
| [OnCellErrorClientFunction](../../aspose.cells.gridweb/mainweb/oncellerrorclientfunction) { get; set; } | Obtient ou définit le nom de la fonction côté client à appeler lorsque la validation d'une cellule échoue. La fonction client doit être déclarée comme ceci : fonction MyOnCellError(cellule) { alert(GridWeb1.getCellValueByCell(cellule)); } Remarque : Vous pouvez utiliser le pointeur "this" dans la fonction client pour pointer le contrôle de grille qui déclenche l'événement. |
| [OnCellSelectedAjaxCallBackClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedajaxcallbackclientfunction) { get; set; } | Obtient ou définit la fonction côté client à appeler lorsqu'une cellule est sélectionnée. La fonction client doit être déclarée comme ceci : fonction MyOnSelectCellAjaxCallBack(cell,customerdata) { } Remarque : Vous pouvez utiliser le pointeur "this" dans la fonction client pour pointer le contrôle de grille qui déclenche l'événement. |
| [OnCellSelectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedclientfunction) { get; set; } | Obtient ou définit la fonction côté client à appeler lorsqu'une cellule est sélectionnée. La fonction client doit être déclarée comme ceci : fonction MyOnSelectCell(cellule) { GridWeb1.setCellValueByCell(cellule, "test"); } Remarque : Vous pouvez utiliser le pointeur "this" dans la fonction client pour pointer le contrôle de grille qui déclenche l'événement. |
| [OnCellUnselectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellunselectedclientfunction) { get; set; } | Obtient ou définit la fonction côté client à appeler lorsqu'une cellule est désélectionnée. La fonction client doit être déclarée comme ceci : fonction MyOnUnselectCell(cellule) { GridWeb1.setCellValueByCell(cellule, "test"); } Remarque : Vous pouvez utiliser le pointeur "this" dans la fonction client pour pointer le contrôle de grille qui déclenche l'événement. |
| [OnCellUpdatedClientFunction](../../aspose.cells.gridweb/mainweb/oncellupdatedclientfunction) { get; set; } | Obtient ou définit le nom de la fonction côté client à appeler lorsque la valeur d'une cellule est mise à jour. La fonction client doit être déclarée comme ceci : fonction MyOnCellUpdated(cellule) { alert(this.getCellValueByCell(cellule)); } Remarque : Vous pouvez utiliser le pointeur "this" dans la fonction client pour pointer le contrôle de grille qui déclenche l'événement. |
| [OnContextMenuShowClientFunction](../../aspose.cells.gridweb/mainweb/oncontextmenushowclientfunction) { get; set; } | Obtient ou définit la fonction côté client à appeler lorsque le menu contextuel sera affiché. La fonction client doit être déclarée comme ceci : fonction onContextMenuShow() { var menu = event.srcElement ; menu.setItemVisibility("Supprimer", "bloquer"); menu.setItemVisibility("Mettre à jour", "aucun"); } Remarque : Vous pouvez utiliser le pointeur "this" dans la fonction client pour pointer le contrôle de grille qui déclenche l'événement. |
| [OnDoubleClickCellClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickcellclientfunction) { get; set; } | Obtient ou définit la fonction côté client à appeler lorsqu'une cellule est double-cliquée. La fonction client doit être déclarée comme ceci : fonction MyOnDoubleClickCell(cellule) { GridWeb1.setCellValueByCell(cellule, "test"); } Remarque : Vous pouvez utiliser le pointeur "this" dans la fonction client pour pointer le contrôle de grille qui déclenche l'événement. |
| [OnDoubleClickRowClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickrowclientfunction) { get; set; } | Obtient ou définit la fonction côté client à appeler lorsqu'une ligne est double-cliquée. La fonction client doit être déclarée comme ceci : fonction MyOnRowDoubleClick(ligne) { alerte(ligne); } Remarque : Vous pouvez utiliser le pointeur "this" dans la fonction client pour pointer le contrôle de grille qui déclenche l'événement. |
| [OnGridInitClientFunction](../../aspose.cells.gridweb/mainweb/ongridinitclientfunction) { get; set; } | Obtient ou définit le nom de la fonction côté client à appeler lorsque la grille est initialisée. La fonction client doit être déclarée comme ceci : fonction MyOnGridInit(grille) { alert("La grille est initialisée : " + grid.id); } Remarque : Vous pouvez utiliser le pointeur "this" dans la fonction client pour pointer le contrôle de grille qui déclenche l'événement. |
| [OnlyAuto](../../aspose.cells.gridweb/mainweb/onlyauto) { get; set; } | Obtient ou définit s'il convient uniquement aux lignes dont la hauteur n'est pas personnalisée, la valeur par défaut est false |
| [OnPageChangeClientFunction](../../aspose.cells.gridweb/mainweb/onpagechangeclientfunction) { get; set; } | Obtient ou définit la fonction côté client à appeler après le changement d'index de page. Ne prend effet que lorsque EnablePaging est vrai. La fonction client doit être déclarée comme ceci : fonction MyOnPageChange(index) { console.log("la page actuelle est :"+index); } Remarque : Vous pouvez utiliser le pointeur "this" dans la fonction client pour pointer le contrôle de grille qui déclenche l'événement. |
| [OnPageSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onpagesubmitclientfunction) { get; set; } | Obtient ou définit la fonction client à appeler avant que la page ne soit soumise côté client. |
| [OnShapeSelectedClientFunction](../../aspose.cells.gridweb/mainweb/onshapeselectedclientfunction) { get; set; } | Obtient ou définit la fonction côté client à appeler lorsqu'une forme est sélectionnée. La fonction client doit être déclarée comme ceci : fonction MyOnSelectShape(forme) { var nom=forme.getAttribute("nomvaleur") var text=shape.getAttribute("textvalue") var value=shape.getAttribute("controlvalue") var type=shape.getAttribute("msotype") } Remarque : Vous pouvez utiliser le pointeur "this" dans la fonction client pour pointer le contrôle de grille qui déclenche l'événement. |
| [OnSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onsubmitclientfunction) { get; set; } | Obtient ou définit la fonction client à appeler avant que le contrôle ne soit soumis côté client. La fonction client doit être déclarée comme ceci : fonction MyOnSubmit(arg, cancelEdit) { retourner vrai ;} L'argument est l'argument de soumission, contient la commande à publier sur le serveur. La valeur cancelEdit est booléenne indique si le contrôle a rejeté l'entrée de l'utilisateur avant de soumettre. Le contrôle continuera à soumettre si la fonction renvoie true.  Remarque : Vous pouvez utiliser le pointeur "this" dans la fonction client pour pointer le contrôle de grille qui déclenche l'événement. |
| [PageSize](../../aspose.cells.gridweb/mainweb/pagesize) { get; set; } | Obtient ou définit la taille de la page en mode de pagination. |
| [PicturesTable](../../aspose.cells.gridweb/mainweb/picturestable) { get; } |  |
| [PresetStyle](../../aspose.cells.gridweb/mainweb/presetstyle) { get; set; } | Obtient ou définit le style prédéfini. |
| [RefreshValidation](../../aspose.cells.gridweb/mainweb/refreshvalidation) { get; set; } | Obtient ou définit s'il faut actualiser la valeur de validation après la modification de la valeur de la cellule. |
| [RenderHiddenRow](../../aspose.cells.gridweb/mainweb/renderhiddenrow) { get; set; } | Obtient ou définit si la ligne masquée est rendue dans GridControl, la valeur par défaut est false. si vous devez afficher la dernière ligne masquée, vous devez la définir sur true |
| [ScrollBarArrowColor](../../aspose.cells.gridweb/mainweb/scrollbararrowcolor) { get; set; } | Spécifie la couleur du bouton fléché de la barre de défilement. |
| [ScrollBarBaseColor](../../aspose.cells.gridweb/mainweb/scrollbarbasecolor) { get; set; } | Spécifie la couleur de la barre de défilement du champ. |
| [SelectCellBgColor](../../aspose.cells.gridweb/mainweb/selectcellbgcolor) { get; set; } | Spécifie la couleur d'arrière-plan des cellules sélectionnées dans la plage de sélection multiple. |
| [SelectCellColor](../../aspose.cells.gridweb/mainweb/selectcellcolor) { get; set; } | Spécifie la couleur des cellules sélectionnées dans la plage de sélection multiple. |
| [SessionLoaded](../../aspose.cells.gridweb/mainweb/sessionloaded) { get; set; } |  |
| [SessionMode](../../aspose.cells.gridweb/mainweb/sessionmode) { get; set; } | Obtient ou définit le mode de session de la grille. Il existe 4 types de mode de session : 1. Session (par défaut) : utiliser la session système pour stocker les données de la feuille. Généralement, asp.net utilise l'état de session InProc. La grille prend également en charge "StateServer" out process session state et SQLServer session state. 2. ViewState : utilisez l'état d'affichage de la page pour stocker les données de la feuille. 3. Personnalisé : utilisez les événements LoadCustomData et SheetDataUpdated pour stocker/récupérer les données de la feuille. 4. Fichier : stocker/récupérer les données de la feuille dans SessionStorePath. |
| [SessionSaved](../../aspose.cells.gridweb/mainweb/sessionsaved) { get; set; } |  |
| [SessionStorePath](../../aspose.cells.gridweb/mainweb/sessionstorepath) { get; set; } | Obtient ou définit le chemin du magasin de cache de session lorsque le mode de session est File ou ViewState, etc : gridweb.SessionStorePath="c:/mytempdir/session" ; alors il stockera les données de session dans c:/mytempdir/session |
| [Settings](../../aspose.cells.gridweb/mainweb/settings) { get; set; } | Représente les paramètres du classeur. |
| [ShapesTable](../../aspose.cells.gridweb/mainweb/shapestable) { get; } |  |
| [ShowAddButton](../../aspose.cells.gridweb/mainweb/showaddbutton) { get; set; } | Obtient ou définit s'il faut afficher le bouton d'ajout de feuille de calcul. |
| [ShowBottomBar](../../aspose.cells.gridweb/mainweb/showbottombar) { get; set; } |  |
| [ShowCellEditBox](../../aspose.cells.gridweb/mainweb/showcelleditbox) { get; set; } | si Gridweb affiche la barre d'outils de la zone d'édition comme dans MS-EXCEL. Si activé, une zone d'édition pour la cellule actuelle s'affichera dans Gridweb. si nous activons cette fonctionnalité, nous devons importer la bibliothèque jquery js dans vos fichiers aspx pour prendre en charge cette nouvelle fonctionnalité. toute la dernière version de jquery est ok. etc. |
| [ShowCommandBarAtTop](../../aspose.cells.gridweb/mainweb/showcommandbarattop) { get; set; } | Spécifie s'il faut afficher la barre de commandes (comprend la barre de commandes et la barre d'onglets) en haut du contrôle. |
| [ShowContextMenu](../../aspose.cells.gridweb/mainweb/showcontextmenu) { get; set; } |  |
| [ShowDefaultGridLine](../../aspose.cells.gridweb/mainweb/showdefaultgridline) { get; set; } | Obtient ou définit s'il faut afficher les lignes de grille par défaut des cellules. |
| [ShowHeaderBar](../../aspose.cells.gridweb/mainweb/showheaderbar) { get; set; } |  |
| [ShowLoading](../../aspose.cells.gridweb/mainweb/showloading) { get; set; } | Spécifie s'il faut afficher une boîte de dialogue de chargement lors de la publication sur le serveur. |
| [ShowLoadingPosition](../../aspose.cells.gridweb/mainweb/showloadingposition) { get; set; } | Spécifie la position supérieure gauche (en px) pour afficher la boîte de dialogue de chargement lors de la publication sur le serveur, etc. 100 200 signifie que la position supérieure gauche de la boîte de dialogue de chargement est à 100px,200px . |
| [ShowSaveButton](../../aspose.cells.gridweb/mainweb/showsavebutton) { get; set; } | Obtient ou définit s'il faut afficher le bouton de sauvegarde. |
| [ShowSubmitButton](../../aspose.cells.gridweb/mainweb/showsubmitbutton) { get; set; } | Obtient ou définit s'il faut afficher le bouton d'envoi. |
| [ShowTabBar](../../aspose.cells.gridweb/mainweb/showtabbar) { get; set; } |  |
| [ShowTabNavigation](../../aspose.cells.gridweb/mainweb/showtabnavigation) { get; set; } | Obtient ou définit si le bouton de navigation par onglet est affiché, la valeur par défaut est true. |
| [ShowUndoButton](../../aspose.cells.gridweb/mainweb/showundobutton) { get; set; } | Obtient ou définit s'il faut afficher le bouton d'annulation. |
| [SpanWrap](../../aspose.cells.gridweb/mainweb/spanwrap) { get; set; } | Spécifie s'il faut envelopper le contenu dans l'étendue de la cellule. La valeur par défaut est true. |
| [TabStyle](../../aspose.cells.gridweb/mainweb/tabstyle) { get; set; } | Obtient ou définit le style de la barre d'onglets. |
| [UseClientPageHeight](../../aspose.cells.gridweb/mainweb/useclientpageheight) { get; set; } | Obtient ou définit si gridweb utilise la hauteur de la page cliente comme hauteur de contrôle, convient lorsque la valeur est définie sur Height="100%", la valeur par défaut est false |
| [ValidationsTable](../../aspose.cells.gridweb/mainweb/validationstable) { get; } |  |
| [ViewPanelScrollLeft](../../aspose.cells.gridweb/mainweb/viewpanelscrollleft) { get; set; } | Obtient ou définit la position de la barre de défilement du panneau d'affichage de la grille. |
| [ViewPanelScrollTop](../../aspose.cells.gridweb/mainweb/viewpanelscrolltop) { get; set; } | Obtient ou définit la position de la barre de défilement du panneau d'affichage de la grille. |
| [ViewTableStyle](../../aspose.cells.gridweb/mainweb/viewtablestyle) { get; set; } | Obtient ou définit le style du panneau d'affichage des données. |
| [WebWorksheets](../../aspose.cells.gridweb/mainweb/webworksheets) { get; } |  |
| override [Width](../../aspose.cells.gridweb/mainweb/width) { get; set; } | Obtient ou définit la largeur ( System.Web.UI.WebControl.Unit ) du contrôle. |
| [WorkSheets](../../aspose.cells.gridweb/mainweb/worksheets) { get; } |  |
| [XhtmlMode](../../aspose.cells.gridweb/mainweb/xhtmlmode) { get; set; } |  |
| static [PictureCachePath](../../aspose.cells.gridweb/mainweb/picturecachepath) { get; set; } | Obtient ou définit le chemin de stockage des images pour le classeur, toutes les formes, les images seront stockées dans ce répertoire, le chemin par défaut est acwcache sous le répertoire de base de l'application actuelle les utilisateurs doivent implémenter un service de planification pour nettoyer les fichiers qui sont sortis du temps de session. |

## Méthodes

| Nom | La description |
| --- | --- |
| [CalculateFormula](../../aspose.cells.gridweb/mainweb/calculateformula)() | Calcule le résultat des formules. |
| override [DataBind](../../aspose.cells.gridweb/mainweb/databind)() | Liez le contrôle et tous ses contrôles enfants à sa source de données. |
| override [Dispose](../../aspose.cells.gridweb/mainweb/dispose)() |  |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile#importexcelfile)(Stream) | Importations à partir d'un flux de fichiers Excel, y compris le flux de fichiers de disque ou le flux de mémoire. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile#importexcelfile_1)(string) | Importe à partir d'un fichier Excel. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile#loadcsvfile)(Stream) | Charge les données d'un flux de fichiers CSV. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile#loadcsvfile_1)(string) | Charge les données d'un fichier CSV. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile#loadhtmlfile)(Stream) | Charge les données d'un flux de fichiers HTML. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile#loadhtmlfile_1)(string) | Charge les données d'un fichier HTML. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile#loadspreadsheetmlfile)(Stream) | Charge les données d'un flux de fichiers SpreadSheetML. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile#loadspreadsheetmlfile_1)(string) | Charge les données d'un fichier SpreadSheetML. |
| [RefreshChartShape](../../aspose.cells.gridweb/mainweb/refreshchartshape)() | actualise toute l'image du graphique pour la feuille de calcul active . |
| override [RenderBeginTag](../../aspose.cells.gridweb/mainweb/renderbegintag)(HtmlTextWriter) |  |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile#savecsvfile)(Stream) | Enregistre les données dans un flux de fichiers CSV. |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile#savecsvfile_1)(string) | Enregistre les données dans un fichier CSV. |
| [SaveCustomStyleFile](../../aspose.cells.gridweb/mainweb/savecustomstylefile)(string) | Enregistre les données de style actuelles du contrôle dans un fichier xml. Peut être utilisé pour créer votre fichier de style personnalisé. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile#savehtmlfile)(Stream) | Enregistre les données dans un flux de fichiers HTML. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile#savehtmlfile_1)(string) | Enregistre les données dans un fichier HTML. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile#savespreadsheetmlfile)(Stream) | Enregistre les données dans un flux de fichiers SpreadSheetML. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile#savespreadsheetmlfile_1)(string) | Enregistre les données dans un fichier SpreadSheetML. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile)(Stream) | Enregistre les feuilles de calcul dans un fichier Excel. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile_3)(string) | Enregistre les feuilles de calcul dans un fichier Excel au format Excel 2003. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile_1)(Stream, GridSaveFormat) | Enregistre les feuilles de calcul dans un fichier Excel. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile_2)(Stream, GridSaveOptions) | Enregistre les feuilles de calcul dans un fichier Excel. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile_4)(string, GridSaveFormat) | Enregistre les feuilles de calcul dans un fichier Excel. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile#savetoexcelfile_5)(string, GridSaveOptions) | Enregistre les feuilles de calcul dans un fichier Excel. |
| [SetCustomStyle](../../aspose.cells.gridweb/mainweb/setcustomstyle)(Stream) | définit le fichier de style personnalisé à partir du flux, y compris le flux de fichier de disque ou le flux de mémoire. |

### Voir également

* class [ExtWebControl](../extwebcontrol)
* espace de noms [Aspose.Cells.GridWeb](../../aspose.cells.gridweb)
* Assemblée [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
