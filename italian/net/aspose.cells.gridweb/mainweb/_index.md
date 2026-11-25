---
title: "Classe MainWeb"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridWeb.MainWeb. Classe genitore del controllo GridWeb. Solo uso interno"
type: docs
url: /it/net/aspose.cells.gridweb/mainweb/
---
## MainWeb class

Classe genitore del controllo GridWeb. Solo uso interno.

```csharp
public class MainWeb : ExtWebControl, INamingContainer, IPostBackDataHandler, 
    IPostBackEventHandler, ISerializable
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [MainWeb](mainweb/)() | Il costruttore predefinito del controllo MainWeb. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb/mainweb/activecell/) { get; set; } | Ottiene o imposta la cella attiva del foglio corrente. Modificata per essere scrivibile dalla versione 1.9.0.1. |
| [ActiveCellBgColor](../../aspose.cells.gridweb/mainweb/activecellbgcolor/) { get; set; } | Specifica il colore di sfondo della cella attiva. |
| [ActiveCellColor](../../aspose.cells.gridweb/mainweb/activecellcolor/) { get; set; } | Specifica il colore della cella attiva. |
| [ActiveHeaderBgColor](../../aspose.cells.gridweb/mainweb/activeheaderbgcolor/) { get; set; } | Specifica il colore di sfondo dell'intestazione di riga/colonna attiva. |
| [ActiveHeaderColor](../../aspose.cells.gridweb/mainweb/activeheadercolor/) { get; set; } | Specifica il colore dell'intestazione di riga/colonna attiva. |
| [ActiveSheet](../../aspose.cells.gridweb/mainweb/activesheet/) { get; } | Ottiene il foglio attivo |
| [ActiveSheetIndex](../../aspose.cells.gridweb/mainweb/activesheetindex/) { get; set; } | Ottiene o imposta l'indice del foglio attivo. Uguale a WebWorksheets.ActiveSheetIndex. |
| [ActiveTabStyle](../../aspose.cells.gridweb/mainweb/activetabstyle/) { get; set; } | Specifica lo stile della scheda attiva. |
| [ACWClientPath](../../aspose.cells.gridweb/mainweb/acwclientpath/) { get; set; } | Ottiene o imposta il percorso web dei file script/immagine del controllo. Per esempio: "http://localhost/acw_client". È inoltre possibile impostare questo valore nel file web.config. Aggiungere questa sezione alla sezione `<configuration>`:`<appSettings>``<add key="aspose.cells.gridweb.acw_client_path" value="/acw_client/" />``</appSettings>` |
| [ACWLanguageFileUrl](../../aspose.cells.gridweb/mainweb/acwlanguagefileurl/) { get; set; } | Ottiene o imposta l'URL web del file lingua del controllo. Per esempio: "/acw_client/lang_en.js". Per impostazione predefinita, viene utilizzato un file inglese integrato. |
| [AutoRefreshChart](../../aspose.cells.gridweb/mainweb/autorefreshchart/) { get; set; } | Ottiene o imposta se l'immagine del grafico viene aggiornata durante l'aggiornamento del valore della cella. Il valore predefinito è true |
| [BottomTableStyle](../../aspose.cells.gridweb/mainweb/bottomtablestyle/) { get; set; } | Ottiene o imposta lo stile della barra inferiore del controllo. |
| [CurrentPageIndex](../../aspose.cells.gridweb/mainweb/currentpageindex/) { get; set; } | Ottiene o imposta l'indice della pagina corrente in modalità paginazione. |
| [CustomCalculationEngine](../../aspose.cells.gridweb/mainweb/customcalculationengine/) { get; set; } | Rappresenta il motore di calcolo personalizzato dell'utente per estendere il motore di calcolo predefinito di **Aspose.Cells**. |
| [CustomCommandButtons](../../aspose.cells.gridweb/mainweb/customcommandbuttons/) { get; } | Ottiene la raccolta dei pulsanti di comando personalizzati |
| [CustomStyleFileName](../../aspose.cells.gridweb/mainweb/customstylefilename/) { get; set; } | Ottiene o imposta il nome del file di stile personalizzato. |
| [DefaultFontName](../../aspose.cells.gridweb/mainweb/defaultfontname/) { get; set; } | Ottiene o imposta il nome del carattere predefinito del controllo. |
| [DefaultFontSize](../../aspose.cells.gridweb/mainweb/defaultfontsize/) { get; set; } | Ottiene o imposta la dimensione del carattere predefinita del controllo. |
| [DefaultGridLineColor](../../aspose.cells.gridweb/mainweb/defaultgridlinecolor/) { get; set; } | Ottiene o imposta il colore della linea di griglia predefinita. |
| [DisplayCellTip](../../aspose.cells.gridweb/mainweb/displaycelltip/) { get; set; } | Ottiene o imposta se mostrare i suggerimenti. il valore predefinito è true. |
| [EditMode](../../aspose.cells.gridweb/mainweb/editmode/) { get; set; } | Ottiene o imposta la modalità di modifica del controllo. |
| [EnableAJAX](../../aspose.cells.gridweb/mainweb/enableajax/) { get; set; } | Ottiene o imposta se utilizzare la chiamata AJAX. il valore predefinito è true. |
| [EnableAsync](../../aspose.cells.gridweb/mainweb/enableasync/) { get; set; } | Ottiene o imposta se caricare i dati delle celle in modo asincrono, si consiglia di applicarlo per un foglio con più di 10000 celle. |
| [EnableClientColumnOperations](../../aspose.cells.gridweb/mainweb/enableclientcolumnoperations/) { get; set; } | Ottiene o imposta se abilitare le operazioni di colonna lato client. |
| [EnableClientFreeze](../../aspose.cells.gridweb/mainweb/enableclientfreeze/) { get; set; } | Ottiene o imposta se abilitare le operazioni di congelamento lato client. |
| [EnableClientMergeOperations](../../aspose.cells.gridweb/mainweb/enableclientmergeoperations/) { get; set; } | Ottiene o imposta se abilitare le operazioni di unione lato client. |
| [EnableClientResizeColumnRow](../../aspose.cells.gridweb/mainweb/enableclientresizecolumnrow/) { get; set; } | Ottiene o imposta se abilitare il ridimensionamento di colonne e righe lato client. |
| [EnableClientRowOperations](../../aspose.cells.gridweb/mainweb/enableclientrowoperations/) { get; set; } | Ottiene o imposta se abilitare le operazioni di riga lato client. |
| [EnableDoubleClickEvent](../../aspose.cells.gridweb/mainweb/enabledoubleclickevent/) { get; set; } | Ottiene o imposta se abilitare l'evento di doppio clic lato cliente. |
| [EnableMetalLightEffect](../../aspose.cells.gridweb/mainweb/enablemetallighteffect/) { get; set; } | Ottiene o imposta se applicare l'effetto luce metallica. |
| [EnablePaging](../../aspose.cells.gridweb/mainweb/enablepaging/) { get; set; } | Ottiene o imposta se abilitare la modalità di paginazione del controllo. |
| [EnableStyleDialogbox](../../aspose.cells.gridweb/mainweb/enablestyledialogbox/) { get; set; } | Ottiene o imposta se abilitare la finestra di dialogo di stile lato client. |
| [FilteredPaging](../../aspose.cells.gridweb/mainweb/filteredpaging/) { get; set; } | Ottiene o imposta se abilitare la paginazione dopo il filtraggio dei dati, avrà effetto quando EnablePaging è true. |
| [ForceValidation](../../aspose.cells.gridweb/mainweb/forcevalidation/) { get; set; } | Ottiene o imposta se forzare la convalida lato cliente. |
| [FrameTableStyle](../../aspose.cells.gridweb/mainweb/frametablestyle/) { get; set; } | Ottiene o imposta lo stile del frame del controllo. |
| [GoonDefaultSaveOperation](../../aspose.cells.gridweb/mainweb/goondefaultsaveoperation/) { get; set; } | Ottiene o imposta se GridWeb eseguirà l'operazione di salvataggio predefinita, il valore predefinito è true. |
| [HeaderBarHeight](../../aspose.cells.gridweb/mainweb/headerbarheight/) { get; set; } | Ottiene o imposta l'altezza (System.Web.UI.WebControl.Unit) della barra dell'intestazione superiore del controllo. |
| [HeaderBarStyle](../../aspose.cells.gridweb/mainweb/headerbarstyle/) { get; set; } | Ottiene o imposta lo stile della barra dell'intestazione. |
| [HeaderBarTableStyle](../../aspose.cells.gridweb/mainweb/headerbartablestyle/) { get; set; } | Ottiene o imposta lo stile della barra dell'intestazione del controllo. |
| [HeaderBarWidth](../../aspose.cells.gridweb/mainweb/headerbarwidth/) { get; set; } | Ottiene o imposta la larghezza( System.Web.UI.WebControl.Unit ) o la barra dell'intestazione sinistra del controllo. |
| override [Height](../../aspose.cells.gridweb/mainweb/height/) { get; set; } | Ottiene o imposta l'altezza( System.Web.UI.WebControl.Unit ) del controllo. |
| [IgnoreStyleWithNoData](../../aspose.cells.gridweb/mainweb/ignorestylewithnodata/) { get; set; } | Ottiene o imposta se GridWeb ignora la visualizzazione di righe o colonne che non contengono valori di cella ma sono comunque formattate. Se impostato su true, le prestazioni saranno migliori. Il valore predefinito è false, il che significa che se l'ultima riga/colonna consecutiva non ha valori di cella ma è formattata, verrà comunque visualizzata. Questa opzione è valida solo quando EnableAsync è false. Questa opzione non ha effetto quando EnableAsync è true, il che significa che GridWeb mostrerà tutte le righe/colonne con stile. |
| [IsCalculateFormula](../../aspose.cells.gridweb/mainweb/iscalculateformula/) { get; set; } | Ottiene o imposta se calcolare la formula dopo le modifiche al valore della cella o dopo l'importazione del file. Il valore predefinito è true. |
| [IsPostBack](../../aspose.cells.gridweb/mainweb/ispostback/) { get; } | Ottiene un valore che indica se gridweb è caricato in risposta a un postback client, o se viene caricato e accesso per la prima volta. |
| [LoadOptions](../../aspose.cells.gridweb/mainweb/loadoptions/) { get; set; } | Rappresenta le opzioni di caricamento per GridWeb. |
| [MaxColumn](../../aspose.cells.gridweb/mainweb/maxcolumn/) { get; set; } | Ottiene o imposta l'indice massimo di visualizzazione della colonna (basato su zero) del foglio web. Il controllo utilizza il valore più grande tra MaxColumn e la colonna massima dei dati del foglio. |
| [MaxRow](../../aspose.cells.gridweb/mainweb/maxrow/) { get; set; } | Ottiene o imposta l'indice massimo di visualizzazione della riga (basato su zero) del foglio web. Il controllo utilizza il valore più grande tra MaxRow e la riga massima dei dati del foglio. |
| [Message](../../aspose.cells.gridweb/mainweb/message/) { get; set; } | Ottiene o imposta il messaggio per la griglia. |
| [MinColumn](../../aspose.cells.gridweb/mainweb/mincolumn/) { get; set; } | Ottiene o imposta l'indice minimo di visualizzazione della colonna (basato su zero) del foglio web. Il controllo utilizza il valore più piccolo tra MinColumn e la colonna minima dei dati del foglio. |
| [MinRow](../../aspose.cells.gridweb/mainweb/minrow/) { get; set; } | Ottiene o imposta l'indice minimo di visualizzazione della riga (basato su zero) del foglio web. Il controllo utilizza il valore più piccolo tra MinRow e la riga minima dei dati del foglio. |
| [ModifiedCells](../../aspose.cells.gridweb/mainweb/modifiedcells/) { get; } | Ottiene la collezione delle celle modificate dal client. |
| [NeedRenderGroupRows](../../aspose.cells.gridweb/mainweb/needrendergrouprows/) { get; set; } | Ottiene o imposta se mostrare le righe di gruppo. |
| [NoHScroll](../../aspose.cells.gridweb/mainweb/nohscroll/) { get; set; } | Ottiene o imposta un valore che indica se la barra di scorrimento orizzontale è nascosta. |
| [NoScroll](../../aspose.cells.gridweb/mainweb/noscroll/) { get; set; } | Ottiene o imposta se mostrare la barra di scorrimento. |
| [NoVScroll](../../aspose.cells.gridweb/mainweb/novscroll/) { get; set; } | Ottiene o imposta un valore che indica se la barra di scorrimento verticale è nascosta. |
| [OnAjaxCallFinishedClientFunction](../../aspose.cells.gridweb/mainweb/onajaxcallfinishedclientfunction/) { get; set; } | Ottiene o imposta il nome della funzione lato client da chiamare quando ajaxcall è terminato. La funzione client deve essere dichiarata così: function GridAjaxcallFinished() { alert(this.id+\" ajaxcall finished \"); }Nota: è possibile utilizzare il puntatore \"this\" nella funzione client per fare riferimento al controllo della griglia che genera l'evento. |
| [OnCellErrorClientFunction](../../aspose.cells.gridweb/mainweb/oncellerrorclientfunction/) { get; set; } | Ottiene o imposta il nome della funzione lato client da chiamare quando la convalida di una cella fallisce. La funzione client deve essere dichiarata così: function MyOnCellError(cell) { alert(this.getCellValueByCell(cell)); }Nota: è possibile utilizzare il puntatore \"this\" nella funzione client per fare riferimento al controllo della griglia che genera l'evento. |
| [OnCellSelectedAjaxCallBackClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedajaxcallbackclientfunction/) { get; set; } | Ottiene o imposta la funzione lato client da chiamare quando una cella è selezionata. La funzione client deve essere dichiarata così: function MyOnSelectCellAjaxCallBack(cell,customerdata) { }Nota: è possibile utilizzare il puntatore \"this\" nella funzione client per fare riferimento al controllo della griglia che genera l'evento. |
| [OnCellSelectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedclientfunction/) { get; set; } | Ottiene o imposta la funzione lato client da chiamare quando una cella è selezionata. La funzione client deve essere dichiarata così: function MyOnSelectCell(cell) { GridWeb1.setCellValueByCell(cell, \"test\"); }Nota: è possibile utilizzare il puntatore \"this\" nella funzione client per fare riferimento al controllo della griglia che genera l'evento. |
| [OnCellUnselectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellunselectedclientfunction/) { get; set; } | Ottiene o imposta la funzione lato client da chiamare quando una cella è deselezionata. La funzione client deve essere dichiarata così: function MyOnUnselectCell(cell) { this.setCellValueByCell(cell, \"test\"); }Nota: è possibile utilizzare il puntatore \"this\" nella funzione client per fare riferimento al controllo della griglia che genera l'evento. |
| [OnCellUpdatedClientFunction](../../aspose.cells.gridweb/mainweb/oncellupdatedclientfunction/) { get; set; } | Ottiene o imposta il nome della funzione lato client da chiamare quando il valore di una cella viene aggiornato. La funzione client deve essere dichiarata così: function MyOnCellUpdated(cell) { alert(this.getCellValueByCell(cell)); }Nota: è possibile utilizzare il puntatore \"this\" nella funzione client per fare riferimento al controllo della griglia che genera l'evento. |
| [OnContextMenuShowClientFunction](../../aspose.cells.gridweb/mainweb/oncontextmenushowclientfunction/) { get; set; } | Ottiene o imposta la funzione lato client da chiamare quando il menu contestuale verrà mostrato. La funzione client dovrebbe essere dichiarata così: function onContextMenuShow() { var menu = event.srcElement; menu.setItemVisibility("Delete", "block"); menu.setItemVisibility("Update", "none"); }Nota: è possibile utilizzare il puntatore "this" nella funzione client per puntare al controllo grid che genera l'evento. |
| [OnDoubleClickCellClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickcellclientfunction/) { get; set; } | Ottiene o imposta la funzione lato client da chiamare quando una cella viene doppio cliccata. La funzione client dovrebbe essere dichiarata così: function MyOnDoubleClickCell(cell) { this.setCellValueByCell(cell, "test"); }Nota: è possibile utilizzare il puntatore "this" nella funzione client per puntare al controllo grid che genera l'evento. |
| [OnDoubleClickRowClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickrowclientfunction/) { get; set; } | Ottiene o imposta la funzione lato client da chiamare quando una riga viene doppio cliccata. La funzione client dovrebbe essere dichiarata così: function MyOnRowDoubleClick(row) { alert(row); }Nota: è possibile utilizzare il puntatore "this" nella funzione client per puntare al controllo grid che genera l'evento. |
| [OnGridInitClientFunction](../../aspose.cells.gridweb/mainweb/ongridinitclientfunction/) { get; set; } | Ottiene o imposta il nome della funzione lato client da chiamare quando la griglia è inizializzata. La funzione client dovrebbe essere dichiarata così: function MyOnGridInit(grid) { alert("The grid is initialized: " + grid.id); }Nota: è possibile utilizzare il puntatore "this" nella funzione client per puntare al controllo grid che genera l'evento. |
| [OnlyAuto](../../aspose.cells.gridweb/mainweb/onlyauto/) { get; set; } | Ottiene o imposta se adattare solo le righe la cui altezza non è personalizzata, il valore predefinito è false |
| [OnPageChangeClientFunction](../../aspose.cells.gridweb/mainweb/onpagechangeclientfunction/) { get; set; } | Ottiene o imposta la funzione lato client da chiamare dopo il cambiamento dell'indice di pagina. Ha effetto solo quando EnablePaging è true. La funzione client dovrebbe essere dichiarata così: function MyOnPageChange(index) { console.log("current page is:"+index); }Nota: è possibile utilizzare il puntatore "this" nella funzione client per puntare al controllo grid che genera l'evento. |
| [OnPageSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onpagesubmitclientfunction/) { get; set; } | Ottiene o imposta la funzione client da chiamare prima che la pagina sia inviata lato client. |
| [OnShapeSelectedClientFunction](../../aspose.cells.gridweb/mainweb/onshapeselectedclientfunction/) { get; set; } | Ottiene o imposta la funzione lato client da chiamare quando una forma è selezionata. La funzione client dovrebbe essere dichiarata così: function MyOnSelectShape(shape) { var name=shape.getAttribute("namevalue") var text=shape.getAttribute("textvalue") var value=shape.getAttribute("controlvalue") var type=shape.getAttribute("msotype") }Nota: è possibile utilizzare il puntatore "this" nella funzione client per puntare al controllo grid che genera l'evento. |
| [OnSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onsubmitclientfunction/) { get; set; } | Ottiene o imposta la funzione client da chiamare prima che il controllo sia inviato lato client. La funzione client dovrebbe essere dichiarata così: function MyOnSubmit(arg, cancelEdit) { return true;} L'arg è l'argomento di invio, contiene il comando da postare al server. Il cancelEdit è un valore booleano che indica se il controllo ha scartato l'input dell'utente prima dell'invio. Il controllo continuerà a inviare se la funzione restituisce true. Nota: è possibile utilizzare il puntatore "this" nella funzione client per puntare al controllo grid che genera l'evento. |
| [PageSize](../../aspose.cells.gridweb/mainweb/pagesize/) { get; set; } | Ottiene o imposta la dimensione della pagina in modalità paginazione. |
| [PresetStyle](../../aspose.cells.gridweb/mainweb/presetstyle/) { get; set; } | Ottiene o imposta lo stile predefinito. |
| [RefreshValidation](../../aspose.cells.gridweb/mainweb/refreshvalidation/) { get; set; } | Ottiene o imposta se aggiornare il valore di validazione dopo le modifiche al valore della cella. |
| [RenderHiddenRow](../../aspose.cells.gridweb/mainweb/renderhiddenrow/) { get; set; } | Ottiene o imposta se la riga nascosta è renderizzata in GridControl, il valore predefinito è false. Se è necessario rendere visibile la riga nascosta in seguito, impostarlo su true. |
| [RowHeightForCSV](../../aspose.cells.gridweb/mainweb/rowheightforcsv/) { get; set; } | Ottiene o imposta il valore dell'altezza della riga in punti per il file csv, il valore predefinito è 14,5. |
| [ScrollBarArrowColor](../../aspose.cells.gridweb/mainweb/scrollbararrowcolor/) { get; set; } | Specifica il colore del pulsante freccia della barra di scorrimento. |
| [ScrollBarBaseColor](../../aspose.cells.gridweb/mainweb/scrollbarbasecolor/) { get; set; } | Specifica il colore della barra di scorrimento del controllo. |
| [SelectCellBgColor](../../aspose.cells.gridweb/mainweb/selectcellbgcolor/) { get; set; } | Specifica il colore di sfondo delle celle selezionate nell'intervallo a selezione multipla. |
| [SelectCellColor](../../aspose.cells.gridweb/mainweb/selectcellcolor/) { get; set; } | Specifica il colore delle celle selezionate nell'intervallo a selezione multipla. |
| [SessionMode](../../aspose.cells.gridweb/mainweb/sessionmode/) { get; set; } | Ottiene o imposta la modalità di sessione della griglia. |
| [SessionStorePath](../../aspose.cells.gridweb/mainweb/sessionstorepath/) { get; set; } | Ottiene o imposta il percorso di archiviazione della cache di sessione quando la modalità di sessione è File o ViewState, ecc: gridweb.SessionStorePath="c:/mytempdir/session"; quindi memorizzerà i dati di sessione in c:/mytempdir/session |
| [Settings](../../aspose.cells.gridweb/mainweb/settings/) { get; set; } | Rappresenta le impostazioni del workbook. |
| [ShowAddButton](../../aspose.cells.gridweb/mainweb/showaddbutton/) { get; set; } | Ottiene o imposta se mostrare il pulsante per aggiungere un foglio di lavoro. |
| [ShowBottomBar](../../aspose.cells.gridweb/mainweb/showbottombar/) { get; set; } | Specifica se mostrare la barra dei comandi (include barra dei comandi e barra delle schede) nella parte inferiore del controllo. |
| [ShowCellEditBox](../../aspose.cells.gridweb/mainweb/showcelleditbox/) { get; set; } | Indica se Gridweb mostra la barra degli strumenti della casella di modifica come in MS-EXCEL. Se abilitata, una casella di modifica per la cella corrente verrà visualizzata in Gridweb. Se abilitiamo questa funzionalità, è necessario importare la libreria jquery js nei file aspx per supportare questa nuova funzionalità. Qualsiasi versione recente di jquery va bene, ecc. |
| [ShowCommandBarAtTop](../../aspose.cells.gridweb/mainweb/showcommandbarattop/) { get; set; } | Specifica se mostrare la barra dei comandi (include la barra dei comandi e la barra delle schede) nella parte superiore del controllo. |
| [ShowContextMenu](../../aspose.cells.gridweb/mainweb/showcontextmenu/) { get; set; } | Ottiene o imposta se mostrare il menu contestuale. Il valore predefinito è true. |
| [ShowDefaultGridLine](../../aspose.cells.gridweb/mainweb/showdefaultgridline/) { get; set; } | Ottiene o imposta se mostrare le linee della griglia predefinite delle celle. |
| [ShowHeaderBar](../../aspose.cells.gridweb/mainweb/showheaderbar/) { get; set; } | Ottiene o imposta se mostrare la barra dell'intestazione |
| [ShowLoading](../../aspose.cells.gridweb/mainweb/showloading/) { get; set; } | Specifica se mostrare una finestra di dialogo di caricamento durante il postback al server. |
| [ShowLoadingPosition](../../aspose.cells.gridweb/mainweb/showloadingposition/) { get; set; } | Specifica la posizione sinistra, superiore (in px) per mostrare la finestra di dialogo di caricamento durante il postback al server, ecc. 100,200 indica che la posizione sinistra, superiore della finestra di dialogo è 100px,200px. |
| [ShowSaveButton](../../aspose.cells.gridweb/mainweb/showsavebutton/) { get; set; } | Ottiene o imposta se mostrare il pulsante di salvataggio. |
| [ShowSubmitButton](../../aspose.cells.gridweb/mainweb/showsubmitbutton/) { get; set; } | Ottiene o imposta se mostrare il pulsante di invio. |
| [ShowTabBar](../../aspose.cells.gridweb/mainweb/showtabbar/) { get; set; } | Ottiene o imposta se mostrare la barra delle schede. |
| [ShowTabNavigation](../../aspose.cells.gridweb/mainweb/showtabnavigation/) { get; set; } | Ottiene o imposta se il pulsante di navigazione delle schede è mostrato, il valore predefinito è true. |
| [ShowUndoButton](../../aspose.cells.gridweb/mainweb/showundobutton/) { get; set; } | Ottiene o imposta se mostrare il pulsante di annullamento. |
| [SpanWrap](../../aspose.cells.gridweb/mainweb/spanwrap/) { get; set; } | Specifica se avvolgere il contenuto nello span della cella. Il valore predefinito è true. |
| [TabStyle](../../aspose.cells.gridweb/mainweb/tabstyle/) { get; set; } | Ottiene o imposta lo stile della barra delle schede. |
| [UseClientPageHeight](../../aspose.cells.gridweb/mainweb/useclientpageheight/) { get; set; } | Ottiene o imposta se GridWeb utilizza l'altezza della pagina client come altezza del controllo, adatto quando si imposta Height=\"100%\", valore predefinito è false |
| [ViewPanelScrollLeft](../../aspose.cells.gridweb/mainweb/viewpanelscrollleft/) { get; set; } | Ottiene o imposta la posizione della barra di scorrimento del pannello di visualizzazione della griglia. |
| [ViewPanelScrollTop](../../aspose.cells.gridweb/mainweb/viewpanelscrolltop/) { get; set; } | Ottiene o imposta la posizione della barra di scorrimento del pannello di visualizzazione della griglia. |
| [ViewTableStyle](../../aspose.cells.gridweb/mainweb/viewtablestyle/) { get; set; } | Ottiene o imposta lo stile del pannello di visualizzazione dei dati. |
| [WebWorksheets](../../aspose.cells.gridweb/mainweb/webworksheets/) { get; } |  |
| override [Width](../../aspose.cells.gridweb/mainweb/width/) { get; set; } | Ottiene o imposta la larghezza (System.Web.UI.WebControl.Unit) del controllo. |
| [WorkSheets](../../aspose.cells.gridweb/mainweb/worksheets/) { get; } | Ottiene o imposta la raccolta dei fogli di lavoro. |
| [XhtmlMode](../../aspose.cells.gridweb/mainweb/xhtmlmode/) { get; set; } | Ottiene o imposta se utilizzare lo stile XHTML, il valore predefinito è true. |
| static [DPI](../../aspose.cells.gridweb/mainweb/dpi/) { get; set; } | Ottiene / imposta i DPI della macchina. |
| static [PictureCachePath](../../aspose.cells.gridweb/mainweb/picturecachepath/) { get; set; } | Ottiene o imposta il percorso di archiviazione delle immagini per la cartella di lavoro, tutte le forme e le immagini saranno memorizzate in questa directory, il percorso predefinito è acwcache nella Directory Base dell'applicazione corrente; gli utenti devono implementare un servizio di pianificazione per pulire i file fuori dal tempo di sessione. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CalculateFormula](../../aspose.cells.gridweb/mainweb/calculateformula/)() | Calcola il risultato delle formule. |
| override [DataBind](../../aspose.cells.gridweb/mainweb/databind/)() | Associa il controllo e tutti i suoi controlli figlio alla sua origine dati. |
| override [Dispose](../../aspose.cells.gridweb/mainweb/dispose/)() |  |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile)(Stream) | Importa da un flusso di file Excel, includendo flusso da disco o flusso di memoria. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_2)(string) | Importa da un file Excel. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_1)(Stream, string) | Importa da un flusso di file Excel, includendo flusso da disco o flusso di memoria. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_3)(string, string) | Importa da un file Excel. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile/#loadcsvfile)(Stream) | Carica i dati da un flusso di file CSV. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile/#loadcsvfile_1)(string) | Carica i dati da un file CSV. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile/#loadhtmlfile)(Stream) | Carica i dati da un flusso di file HTML. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile/#loadhtmlfile_1)(string) | Carica i dati da un file HTML. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile/#loadspreadsheetmlfile)(Stream) | Carica i dati da un flusso di file SpreadSheetML. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile/#loadspreadsheetmlfile_1)(string) | Carica i dati da un file SpreadSheetML. |
| [RefreshChartShape](../../aspose.cells.gridweb/mainweb/refreshchartshape/)() | Aggiorna tutte le immagini dei grafici per il foglio di lavoro attivo. |
| override [RenderBeginTag](../../aspose.cells.gridweb/mainweb/renderbegintag/)(HtmlTextWriter) |  |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile/#savecsvfile)(Stream) | Salva i dati in un flusso di file CSV. |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile/#savecsvfile_1)(string) | Salva i dati in un file CSV. |
| [SaveCustomStyleFile](../../aspose.cells.gridweb/mainweb/savecustomstylefile/)(string) | Salva i dati di stile correnti del controllo in un file xml. Può essere utilizzato per creare il tuo file di stile personalizzato. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile/#savehtmlfile)(Stream) | Salva i dati in un flusso di file HTML. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile/#savehtmlfile_1)(string) | Salva i dati in un file HTML. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile/#savespreadsheetmlfile)(Stream) | Salva i dati in un flusso di file SpreadSheetML. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile/#savespreadsheetmlfile_1)(string) | Salva i dati in un file SpreadSheetML. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile)(Stream) | Salva i fogli di lavoro in un file Excel. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_3)(string) | Salva i fogli di lavoro in un file Excel con formato Excel 2003. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_1)(Stream, GridSaveFormat) | Salva i fogli di lavoro in un file Excel. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_2)(Stream, GridSaveOptions) | Salva i fogli di lavoro in un file Excel. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_4)(string, GridSaveFormat) | Salva i fogli di lavoro in un file Excel. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_5)(string, GridSaveOptions) | Salva i fogli di lavoro in un file Excel. |
| [SetCustomStyle](../../aspose.cells.gridweb/mainweb/setcustomstyle/)(Stream) | Imposta il file di stile personalizzato da uno stream, includendo lo stream di file su disco o lo stream di memoria. |

## Eventi

| Nome | Descrizione |
| --- | --- |
| event [AfterColumnFilter](../../aspose.cells.gridweb/mainweb/aftercolumnfilter/) | Si verifica dopo che la colonna è filtrata. |
| event [AjaxCallFinished](../../aspose.cells.gridweb/mainweb/ajaxcallfinished/) | Viene attivato quando l'aggiornamento ajax del controllo è terminato. (EnableAJAX deve essere impostato su true) |
| event [BeforeColumnFilter](../../aspose.cells.gridweb/mainweb/beforecolumnfilter/) | Si verifica prima che la colonna sia filtrata. |
| event [CellClickOnAjax](../../aspose.cells.gridweb/mainweb/cellclickonajax/) | Si verifica quando la cella viene cliccata e occorre eseguire un ajaxcallback per questo evento. |
| event [CellClientUpdate](../../aspose.cells.gridweb/mainweb/cellclientupdate/) | Si verifica quando avviene un aggiornamento della cella client. Quando questo evento è attivato, il suo parametro e.Argument contiene il nome del comando. |
| event [CellCommand](../../aspose.cells.gridweb/mainweb/cellcommand/) | Si verifica quando il collegamento ipertestuale del comando di una cella viene cliccato. Quando questo evento è attivato, il suo parametro e.Argument contiene il nome del comando. |
| event [CellDoubleClick](../../aspose.cells.gridweb/mainweb/celldoubleclick/) | Si verifica quando la cella viene doppio cliccata. |
| event [CellError](../../aspose.cells.gridweb/mainweb/cellerror/) | Si verifica quando c'è un errore di valore di input nella cella. |
| event [CellModifiedOnAjax](../../aspose.cells.gridweb/mainweb/cellmodifiedonajax/) | Si verifica quando la cella è modificata in ajaxcall. |
| event [ColumnDeleted](../../aspose.cells.gridweb/mainweb/columndeleted/) | Si verifica quando l'utente elimina una colonna dal menu lato client. |
| event [ColumnDeleting](../../aspose.cells.gridweb/mainweb/columndeleting/) | Si verifica quando l'utente sta tentando di eliminare una colonna dal menu lato client. È possibile gestire questo evento e impostare il parametro cancel su True per annullare l'operazione di eliminazione. |
| event [ColumnDoubleClick](../../aspose.cells.gridweb/mainweb/columndoubleclick/) | Si verifica quando l'intestazione della colonna viene doppio cliccata. |
| event [ColumnInserted](../../aspose.cells.gridweb/mainweb/columninserted/) | Si verifica quando l'utente inserisce una colonna dal menu lato client. |
| event [CustomCommand](../../aspose.cells.gridweb/mainweb/customcommand/) | Si verifica quando l'utente clicca un pulsante di comando personalizzato. |
| event [LoadCustomData](../../aspose.cells.gridweb/mainweb/loadcustomdata/) | Viene attivato quando la SessionMode del controllo è impostata su Custom e deve caricare i dati del foglio. È possibile gestire questo evento in modalità Custom Session per caricare i dati del foglio da file o database. |
| event [PageIndexChanged](../../aspose.cells.gridweb/mainweb/pageindexchanged/) | Si verifica quando l'indice della pagina del foglio del controllo è cambiato. |
| event [RowDeleted](../../aspose.cells.gridweb/mainweb/rowdeleted/) | Si verifica quando l'utente ha eliminato una riga dal menu lato client. |
| event [RowDeleting](../../aspose.cells.gridweb/mainweb/rowdeleting/) | Si verifica quando l'utente sta tentando di eliminare una riga dal menu lato client. È possibile gestire questo evento e lanciare un'eccezione RejectDeleteException per annullare l'operazione di eliminazione. |
| event [RowDoubleClick](../../aspose.cells.gridweb/mainweb/rowdoubleclick/) | Si verifica quando l'intestazione della riga viene doppio cliccata. |
| event [RowInserted](../../aspose.cells.gridweb/mainweb/rowinserted/) | Si verifica quando l'utente inserisce una riga dal menu lato client. |
| event [SaveCommand](../../aspose.cells.gridweb/mainweb/savecommand/) | Si verifica quando il pulsante "save" è cliccato. |
| event [SheetAdded](../../aspose.cells.gridweb/mainweb/sheetadded/) | Si verifica quando l'utente aggiunge un foglio di lavoro dal menu della barra degli strumenti. |
| event [SheetDataUpdated](../../aspose.cells.gridweb/mainweb/sheetdataupdated/) | Si verifica quando il controllo ha caricato i dati inviati e aggiornato i dati del foglio. |
| event [SheetTabClick](../../aspose.cells.gridweb/mainweb/sheettabclick/) | Si verifica quando la scheda del foglio è cliccata. |
| event [SubmitCommand](../../aspose.cells.gridweb/mainweb/submitcommand/) | Si verifica quando il pulsante "submit" è cliccato. |
| event [UndoCommand](../../aspose.cells.gridweb/mainweb/undocommand/) | Si verifica quando si fa clic sul pulsante "undo". |

### Esempi

```csharp
[C#]
	GridWeb GridWeb1 = new GridWeb();
//esegui la tua attività
```

### Vedi anche

* class [ExtWebControl](../extwebcontrol/)
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


