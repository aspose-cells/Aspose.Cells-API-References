---
title: "GridWebBean"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta il bean Java GridWeb"
type: docs
url: /it/java/com.aspose.gridweb/gridwebbean/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.WebControl](../../com.aspose.gridweb/webcontrol), [com.aspose.gridweb.ExtWebControl](../../com.aspose.gridweb/extwebcontrol), [com.aspose.gridweb.MainWeb](../../com.aspose.gridweb/mainweb)
```
public class GridWebBean extends MainWeb
```

Rappresenta il bean Java GridWeb
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [GridWebBean()](#GridWebBean--) | il costruttore predefinito di GridWebBean |
## Campi

| Campo | Descrizione |
| --- | --- |
| [AfterColumnFilter](#AfterColumnFilter) | Si verifica dopo che la colonna è stata filtrata. |
| [AjaxCallFinished](#AjaxCallFinished) | Viene attivato quando l'aggiornamento ajax del controllo è terminato. |
| [BeforeColumnFilter](#BeforeColumnFilter) | Si verifica prima che la colonna venga filtrata. |
| [CellClickOnAjax](#CellClickOnAjax) | Si verifica quando la cella viene cliccata, e è necessario eseguire un ajaxcallback per questo evento. |
| [CellClientUpdate](#CellClientUpdate) | Si verifica quando avviene un aggiornamento della cella client. |
| [CellCommand](#CellCommand) | Si verifica quando il collegamento ipertestuale del comando di una cella viene cliccato. |
| [CellDoubleClick](#CellDoubleClick) | Si verifica quando la cella viene doppio-cliccata. |
| [CellModifiedOnAjax](#CellModifiedOnAjax) | Si verifica quando la cella viene modificata in ajaxcall. |
| [ColumnDeleted](#ColumnDeleted) | Si verifica quando l'utente elimina una colonna dal menu lato client. |
| [ColumnDeleting](#ColumnDeleting) | Si verifica quando l'utente sta tentando di eliminare una colonna dal menu lato client. |
| [ColumnDoubleClick](#ColumnDoubleClick) | Si verifica quando l'intestazione della colonna viene doppio-cliccata. |
| [ColumnInserted](#ColumnInserted) | Si verifica quando l'utente inserisce una colonna dal menu lato client. |
| [CustomCommand](#CustomCommand) | Si verifica quando l'utente clicca un pulsante di comando personalizzato. |
| [LoadCustomData](#LoadCustomData) | Viene attivato quando la SessionMode del controllo è impostata su Custom e deve caricare i dati del foglio. |
| [PageIndexChanged](#PageIndexChanged) | Si verifica quando l'indice della pagina del foglio del controllo è cambiato. |
| [RowDeleted](#RowDeleted) | Si verifica quando l'utente ha eliminato una riga dal menu lato client. |
| [RowDeleting](#RowDeleting) | Si verifica quando l'utente sta tentando di eliminare una riga dal menu lato client. |
| [RowDoubleClick](#RowDoubleClick) | Si verifica quando l'intestazione della riga viene doppio cliccata. |
| [RowInserted](#RowInserted) | Si verifica quando l'utente inserisce una riga dal menu lato client. |
| [SaveCommand](#SaveCommand) | Si verifica quando il pulsante "save" viene cliccato. |
| [SheetAdded](#SheetAdded) | Si verifica quando l'utente aggiunge un foglio di lavoro dal menu della barra degli strumenti. |
| [SheetTabClick](#SheetTabClick) | Si verifica quando la scheda del foglio viene cliccata. |
| [SubmitCommand](#SubmitCommand) | Si verifica quando il pulsante "submit" viene cliccato. |
| [UndoCommand](#UndoCommand) | Si verifica quando il pulsante "undo" viene cliccato. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [calculateFormula()](#calculateFormula--) | Calcola il risultato delle formule. |
| [createChildControls()](#createChildControls--) | Implementa CreateChildControls da WebControl, utilizzato internamente solo. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getACWClientPath()](#getACWClientPath--) | Ottiene il percorso web dei file script/immagine del controllo. |
| [getACWLanguageFileUrl()](#getACWLanguageFileUrl--) | Ottiene l'URL web del file lingua del controllo. |
| [getActiveCell()](#getActiveCell--) | Ottiene la cella attiva del foglio corrente. |
| [getActiveCellBgColor()](#getActiveCellBgColor--) | Specifica il colore di sfondo della cella attiva. |
| [getActiveCellColor()](#getActiveCellColor--) | Specifica il colore della cella attiva. |
| [getActiveHeaderBgColor()](#getActiveHeaderBgColor--) | Specifica il colore di sfondo dell'intestazione della riga/colonna attiva. |
| [getActiveHeaderColor()](#getActiveHeaderColor--) | Specifica il colore dell'intestazione della riga/colonna attiva. |
| [getActiveSheet()](#getActiveSheet--) | Ottiene il foglio attivo |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | Ottiene l'indice del foglio attivo. |
| [getActiveTabStyle()](#getActiveTabStyle--) | Specifica lo stile della scheda attiva. |
| [getAutoRefreshChart()](#getAutoRefreshChart--) | Ottiene se l'immagine del grafico viene aggiornata durante l'aggiornamento del valore della cella; il valore predefinito è true. |
| [getBackColor()](#getBackColor--) | Ottiene il BackColor nel WebControl |
| [getBeanID()](#getBeanID--) | ottieni l'id html del bean |
| [getBorderColor()](#getBorderColor--) | Ottiene il BorderColor nel WebControl |
| [getBorderStyle()](#getBorderStyle--) | Ottiene il BorderStyle nel WebControl |
| [getBorderWidth()](#getBorderWidth--) | Ottiene il BorderWidth nel WebControl |
| [getBottomTableStyle()](#getBottomTableStyle--) | Ottiene lo stile della barra inferiore del controllo. |
| [getClass()](#getClass--) |  |
| [getCssClass()](#getCssClass--) | Ottiene la CssClass nel WebControl |
| [getCurrentPageIndex()](#getCurrentPageIndex--) | Ottiene l'indice della pagina corrente in modalità paginazione. |
| [getCustomCalculationEngine()](#getCustomCalculationEngine--) | Rappresenta il motore di calcolo personalizzato dell'utente per estendere il motore di calcolo predefinito di Aspose.Cells. |
| [getCustomCommandButtons()](#getCustomCommandButtons--) | Ottiene la raccolta dei pulsanti di comando personalizzati |
| [getCustomStyleFileName()](#getCustomStyleFileName--) | Ottiene il nome del file di stile personalizzato. |
| [getDPI()](#getDPI--) | Ottiene /Imposta il DPI della macchina. |
| [getDefaultFontName()](#getDefaultFontName--) | Ottiene il nome del carattere predefinito del controllo. |
| [getDefaultFontSize()](#getDefaultFontSize--) | Ottiene la dimensione predefinita del carattere del controllo. |
| [getDefaultGridLineColor()](#getDefaultGridLineColor--) | Ottiene il colore predefinito della linea della griglia. |
| [getDisplayCellTip()](#getDisplayCellTip--) | Ottiene se mostrare i suggerimenti. Il valore predefinito è true. |
| [getEditMode()](#getEditMode--) | Ottiene la modalità di modifica del controllo. |
| [getEnableAJAX()](#getEnableAJAX--) | Ottiene se utilizzare la chiamata AJAX. Il valore predefinito è true. |
| [getEnableAsync()](#getEnableAsync--) | Ottiene se caricare i dati delle celle in modo asincrono, suggerito per un foglio con più di 10000 celle. |
| [getEnableClientColumnOperations()](#getEnableClientColumnOperations--) | Ottiene se abilitare le operazioni di colonna lato client. |
| [getEnableClientFreeze()](#getEnableClientFreeze--) | Ottiene se abilitare le operazioni di congelamento lato client. |
| [getEnableClientMergeOperations()](#getEnableClientMergeOperations--) | Ottiene se abilitare le operazioni di unione lato client. |
| [getEnableClientResizeColumnRow()](#getEnableClientResizeColumnRow--) | Ottiene se abilitare il ridimensionamento di colonne e righe lato client. |
| [getEnableClientRowOperations()](#getEnableClientRowOperations--) | Ottiene se abilitare le operazioni di riga lato client. |
| [getEnableDoubleClickEvent()](#getEnableDoubleClickEvent--) | Ottiene se abilitare l'evento di doppio clic lato cliente. |
| [getEnableMetalLightEffect()](#getEnableMetalLightEffect--) | Ottiene se applicare l'effetto luce metallica. |
| [getEnablePaging()](#getEnablePaging--) | Ottiene se abilitare la modalità di paginazione del controllo. |
| [getEnableStyleDialogbox()](#getEnableStyleDialogbox--) | Ottiene se abilitare la finestra di dialogo stile lato client. |
| [getEnabled()](#getEnabled--) | Ottiene l'Enabled nel WebControl |
| [getFilteredPaging()](#getFilteredPaging--) | Ottiene se abilitare la paginazione dopo il filtraggio dei dati, avrà effetto quando EnablePaging è true. |
| [getFont()](#getFont--) | Ottiene il Font nel WebControl |
| [getForceValidation()](#getForceValidation--) | Ottiene se forzare la convalida lato cliente. |
| [getForeColor()](#getForeColor--) | Ottiene il ForeColor nel WebControl |
| [getFrameTableStyle()](#getFrameTableStyle--) | Ottiene lo stile del frame del controllo. |
| [getGoonDefaultSaveOperation()](#getGoonDefaultSaveOperation--) | Ottiene se GridWeb eseguirà l'operazione di salvataggio predefinita, il valore predefinito è true. |
| [getHTMLBody()](#getHTMLBody--) | il codice html del bean per il corpo html, deve essere ottenuto dopo la chiamata del metodo init e prepareRender |
| [getHTMLHead()](#getHTMLHead--) | il codice HTML del bean per l'intestazione HTML, deve essere ottenuto dopo la chiamata del metodo init e prepareRender |
| [getHeaderBarHeight()](#getHeaderBarHeight--) | Ottiene l'altezza (System.Web.UI.WebControl.Unit) della barra dell'intestazione superiore del controllo. |
| [getHeaderBarStyle()](#getHeaderBarStyle--) | Ottiene lo stile della barra dell'intestazione. |
| [getHeaderBarTableStyle()](#getHeaderBarTableStyle--) | Ottiene lo stile della barra dell'intestazione del controllo. |
| [getHeaderBarWidth()](#getHeaderBarWidth--) | Ottiene la larghezza( System.Web.UI.WebControl.Unit ) o la barra dell'intestazione sinistra del controllo. |
| [getHeight()](#getHeight--) | Ottiene l'altezza( System.Web.UI.WebControl.Unit ) del controllo. |
| [getIgnoreStyleWithNoData()](#getIgnoreStyleWithNoData--) | Ottiene se GridWeb ignora la visualizzazione di righe o colonne che non contengono valori di cella ma sono comunque formattate. |
| [getLoadOptions()](#getLoadOptions--) | Rappresenta le opzioni di caricamento per GridWeb. |
| [getMaxColumn()](#getMaxColumn--) | Ottiene l'indice massimo della colonna visualizzata (basato su zero) del foglio web. |
| [getMaxRow()](#getMaxRow--) | Ottiene l'indice massimo della riga visualizzata (basato su zero) del foglio web. |
| [getMessage()](#getMessage--) | Ottiene il messaggio per la griglia. |
| [getMinColumn()](#getMinColumn--) | Ottiene l'indice minimo della colonna visualizzata (basato su zero) del foglio web. |
| [getMinRow()](#getMinRow--) | Ottiene l'indice minimo della riga visualizzata (basato su zero) del foglio web. |
| [getModifiedCells()](#getModifiedCells--) | Ottiene la raccolta delle celle modificate dal client. |
| [getNeedRenderGroupRows()](#getNeedRenderGroupRows--) | Ottiene se mostrare le righe di gruppo . |
| [getNoHScroll()](#getNoHScroll--) | Ottiene un valore che indica se la barra di scorrimento orizzontale è nascosta. |
| [getNoScroll()](#getNoScroll--) | Ottiene se mostrare la barra di scorrimento . |
| [getNoVScroll()](#getNoVScroll--) | Ottiene un valore che indica se la barra di scorrimento verticale è nascosta. |
| [getOnAjaxCallFinishedClientFunction()](#getOnAjaxCallFinishedClientFunction--) | Ottiene il nome della funzione lato client da chiamare quando la chiamata ajax è terminata. |
| [getOnCellErrorClientFunction()](#getOnCellErrorClientFunction--) | Ottiene il nome della funzione lato client da chiamare quando la convalida di una cella fallisce. |
| [getOnCellSelectedAjaxCallBackClientFunction()](#getOnCellSelectedAjaxCallBackClientFunction--) | Ottiene la funzione lato client da chiamare quando una cella è selezionata. |
| [getOnCellSelectedClientFunction()](#getOnCellSelectedClientFunction--) | Ottiene la funzione lato client da chiamare quando una cella è selezionata. |
| [getOnCellUnselectedClientFunction()](#getOnCellUnselectedClientFunction--) | Ottiene la funzione lato client da chiamare quando una cella è deselezionata. |
| [getOnCellUpdatedClientFunction()](#getOnCellUpdatedClientFunction--) | Ottiene il nome della funzione lato client da chiamare quando il valore di una cella viene aggiornato. |
| [getOnContextMenuShowClientFunction()](#getOnContextMenuShowClientFunction--) | Ottiene la funzione lato client da chiamare quando verrà mostrato il menu contestuale. |
| [getOnDoubleClickCellClientFunction()](#getOnDoubleClickCellClientFunction--) | Ottiene la funzione lato client da chiamare quando una cella viene doppio cliccata. |
| [getOnDoubleClickRowClientFunction()](#getOnDoubleClickRowClientFunction--) | Ottiene la funzione lato client da chiamare quando una riga viene doppio cliccata. |
| [getOnGridInitClientFunction()](#getOnGridInitClientFunction--) | Ottiene il nome della funzione lato client da chiamare quando la griglia è inizializzata. |
| [getOnPageChangeClientFunction()](#getOnPageChangeClientFunction--) | Ottiene la funzione lato client da chiamare dopo la modifica dell'indice di pagina. Ha effetto solo quando EnablePaging è true. |
| [getOnPageSubmitClientFunction()](#getOnPageSubmitClientFunction--) | Ottiene la funzione client da chiamare prima che la pagina venga inviata lato client. |
| [getOnShapeSelectedClientFunction()](#getOnShapeSelectedClientFunction--) | Ottiene la funzione lato client da chiamare quando una forma è selezionata. |
| [getOnSubmitClientFunction()](#getOnSubmitClientFunction--) | Ottiene la funzione client da chiamare prima che il controllo venga inviato lato client. |
| [getOnlyAuto()](#getOnlyAuto--) | Ottiene se adattare solo le righe la cui altezza non è personalizzata, il valore predefinito è false. |
| [getPageSize()](#getPageSize--) | Ottiene la dimensione della pagina in modalità paginazione. |
| [getPictureCachePath()](#getPictureCachePath--) | Ottiene il percorso di archiviazione delle immagini per la cartella di lavoro, tutte le forme e le immagini saranno memorizzate in questa directory, il percorso predefinito è acwcache nella directory base dell'applicazione corrente; gli utenti devono implementare un servizio di pianificazione per pulire i file fuori dal tempo di sessione. |
| [getPresetStyle()](#getPresetStyle--) | Ottiene lo stile predefinito. |
| [getRefreshValidation()](#getRefreshValidation--) | Ottiene se aggiornare il valore di convalida dopo che il valore della cella è cambiato. |
| [getRenderHiddenRow()](#getRenderHiddenRow--) | Ottiene se la riga nascosta viene renderizzata in GridControl, il valore predefinito è false. |
| [getRowHeightForCSV()](#getRowHeightForCSV--) | Ottiene il valore dell'altezza della riga in punti per il file csv, il valore predefinito è 14,5. |
| [getScrollBarArrowColor()](#getScrollBarArrowColor--) | Specifica il colore del pulsante freccia della barra di scorrimento. |
| [getScrollBarBaseColor()](#getScrollBarBaseColor--) | Specifica il colore della barra di scorrimento del controllo. |
| [getSelectCellBgColor()](#getSelectCellBgColor--) | Specifica il colore di sfondo delle celle selezionate nell'intervallo di selezione multipla. |
| [getSelectCellColor()](#getSelectCellColor--) | Specifica il colore delle celle selezionate nell'intervallo di selezione multipla. |
| [getSessionStorePath()](#getSessionStorePath--) | Ottiene il percorso di archiviazione della cache di sessione quando la modalità sessione è File o ViewState, ecc.: gridweb.SessionStorePath=\"c:/mytempdir/session\"; quindi i dati di sessione saranno memorizzati in c:/mytempdir/session. |
| [getSettings()](#getSettings--) | Rappresenta le impostazioni della cartella di lavoro. |
| [getShowAddButton()](#getShowAddButton--) | Ottiene se mostrare il pulsante aggiungi foglio di lavoro. |
| [getShowBottomBar()](#getShowBottomBar--) | Specifica se mostrare la barra dei comandi (include barra dei comandi e barra delle schede) nella parte inferiore del controllo. |
| [getShowCellEditBox()](#getShowCellEditBox--) | Indica se Gridweb mostra la barra degli strumenti della casella di modifica come in MS-EXCEL. Se abilitata, una casella di modifica per la cella corrente verrà visualizzata in Gridweb. |
| [getShowCommandBarAtTop()](#getShowCommandBarAtTop--) | Specifica se mostrare la barra dei comandi (include barra dei comandi e barra delle schede) nella parte superiore del controllo. |
| [getShowContextMenu()](#getShowContextMenu--) | Ottiene se mostrare il menu contestuale. Il valore predefinito è true. |
| [getShowDefaultGridLine()](#getShowDefaultGridLine--) | Ottiene se mostrare le linee di griglia predefinite delle celle. |
| [getShowHeaderBar()](#getShowHeaderBar--) | Ottiene se mostrare la barra dell'intestazione |
| [getShowLoading()](#getShowLoading--) | Specifica se mostrare una finestra di dialogo di caricamento durante il postback al server. |
| [getShowLoadingPosition()](#getShowLoadingPosition--) | Specifica la posizione sinistra, superiore (in px) per mostrare la finestra di dialogo di caricamento durante il postback al server, ecc. 100,200 indica che la posizione sinistra e superiore della finestra di dialogo di caricamento è a 100px,200px. |
| [getShowSaveButton()](#getShowSaveButton--) | Ottiene se mostrare il pulsante di salvataggio. |
| [getShowSubmitButton()](#getShowSubmitButton--) | Ottiene se mostrare il pulsante di invio. |
| [getShowTabBar()](#getShowTabBar--) | Ottiene se mostrare la barra delle schede. |
| [getShowTabNavigation()](#getShowTabNavigation--) | Ottiene se il pulsante di navigazione delle schede è mostrato, il valore predefinito è true. |
| [getShowUndoButton()](#getShowUndoButton--) | Ottiene se mostrare il pulsante di annullamento. |
| [getSpanWrap()](#getSpanWrap--) | Specifica se avvolgere il contenuto nello span di cella, il valore predefinito è true. |
| [getTabIndex()](#getTabIndex--) | Ottiene il TabIndex nel WebControl |
| [getTabStyle()](#getTabStyle--) | Ottiene lo stile della barra delle schede. |
| [getToolTip()](#getToolTip--) | Ottiene il ToolTip nel WebControl |
| [getUseClientPageHeight()](#getUseClientPageHeight--) | Ottiene se GridWeb utilizza l'altezza della pagina client come altezza del controllo, adatto quando si imposta Height=\"100%\", il valore predefinito è false. |
| [getViewPanelScrollLeft()](#getViewPanelScrollLeft--) | Ottiene la posizione della barra di scorrimento del pannello di visualizzazione della griglia. |
| [getViewPanelScrollTop()](#getViewPanelScrollTop--) | Ottiene la posizione della barra di scorrimento del pannello di visualizzazione della griglia. |
| [getViewTableStyle()](#getViewTableStyle--) | Ottiene lo stile del pannello di visualizzazione dei dati. |
| [getWidth()](#getWidth--) | Ottiene la larghezza (System.Web.UI.WebControl.Unit) del controllo. |
| [getWorkSheets()](#getWorkSheets--) | Ottiene la raccolta dei fogli di lavoro. |
| [getXhtmlMode()](#getXhtmlMode--) | Ottiene se utilizzare lo stile XHTML, il valore predefinito è true. |
| [hashCode()](#hashCode--) |  |
| [importExcelFile(InputStream stream)](#importExcelFile-java.io.InputStream-) | Importa da un flusso di file Excel, inclusi flusso di file su disco o flusso di memoria. |
| [importExcelFile(InputStream stream, String passwordtoOpen)](#importExcelFile-java.io.InputStream-java.lang.String-) | Importa da un flusso di file Excel, inclusi flusso di file su disco o flusso di memoria. |
| [importExcelFile(String fileName)](#importExcelFile-java.lang.String-) | Importa da un file Excel. |
| [importExcelFile(String fileName, String passwordtoOpen)](#importExcelFile-java.lang.String-java.lang.String-) | Importa da un file Excel. |
| [init()](#init--) | il bean deve essere inizializzato dalla richiesta servlet e dalla risposta della pagina corrente |
| [isCalculateFormula()](#isCalculateFormula--) | Ottiene se calcolare la formula dopo le modifiche al valore della cella o dopo l'importazione del file. |
| [loadCSVFile(InputStream stream)](#loadCSVFile-java.io.InputStream-) | Carica i dati da un flusso di file CSV. |
| [loadCSVFile(String fileName)](#loadCSVFile-java.lang.String-) | Carica i dati da un file CSV. |
| [loadHTMLFile(InputStream stream)](#loadHTMLFile-java.io.InputStream-) | Carica i dati da un flusso di file HTML. |
| [loadHTMLFile(String fileName)](#loadHTMLFile-java.lang.String-) | Carica i dati da un file HTML. |
| [loadSpreadSheetMLFile(InputStream stream)](#loadSpreadSheetMLFile-java.io.InputStream-) | Carica i dati da un flusso di file SpreadSheetML. |
| [loadSpreadSheetMLFile(String fileName)](#loadSpreadSheetMLFile-java.lang.String-) | Carica i dati da un file SpreadSheetML. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [prepareRender()](#prepareRender--) | il metodo deve essere chiamato prima del rendering del bean GridWeb |
| [refreshChartShape()](#refreshChartShape--) | Aggiorna tutte le immagini dei grafici per il foglio di lavoro attivo. |
| [saveCSVFile(OutputStream stream)](#saveCSVFile-java.io.OutputStream-) | Salva i dati in un flusso di file CSV. |
| [saveCSVFile(String targetFile)](#saveCSVFile-java.lang.String-) | Salva i dati in un file CSV. |
| [saveCustomStyleFile(String fileName)](#saveCustomStyleFile-java.lang.String-) | Salva i dati di stile corrente del controllo in un file XML. |
| [saveHTMLFile(OutputStream stream)](#saveHTMLFile-java.io.OutputStream-) | Salva i dati in un flusso di file HTML. |
| [saveHTMLFile(String targetFile)](#saveHTMLFile-java.lang.String-) | Salva i dati in un file HTML. |
| [saveSpreadSheetMLFile(OutputStream stream)](#saveSpreadSheetMLFile-java.io.OutputStream-) | Salva i dati in un flusso di file SpreadSheetML. |
| [saveSpreadSheetMLFile(String targetFile)](#saveSpreadSheetMLFile-java.lang.String-) | Salva i dati in un file SpreadSheetML. |
| [saveToExcelFile(OutputStream stream)](#saveToExcelFile-java.io.OutputStream-) | Salva i fogli di lavoro in un file Excel. |
| [saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions)](#saveToExcelFile-java.io.OutputStream-com.aspose.gridweb.GridSaveOptions-) | Salva i fogli di lavoro in un file Excel. |
| [saveToExcelFile(OutputStream stream, int format)](#saveToExcelFile-java.io.OutputStream-int-) | Salva i fogli di lavoro in un file Excel. |
| [saveToExcelFile(String targetFile)](#saveToExcelFile-java.lang.String-) | Salva i fogli di lavoro in un file Excel con formato Excel 2003. |
| [saveToExcelFile(String targetFile, GridSaveOptions saveOptions)](#saveToExcelFile-java.lang.String-com.aspose.gridweb.GridSaveOptions-) | Salva i fogli di lavoro in un file Excel. |
| [saveToExcelFile(String targetFile, int format)](#saveToExcelFile-java.lang.String-int-) | Salva i fogli di lavoro in un file Excel. |
| [setACWClientPath(String value)](#setACWClientPath-java.lang.String-) | Imposta il percorso web dei file script/immagine del controllo. |
| [setACWLanguageFileUrl(String value)](#setACWLanguageFileUrl-java.lang.String-) | Imposta l'URL web del file lingua del controllo. |
| [setActiveCell(GridCell value)](#setActiveCell-com.aspose.gridweb.GridCell-) | Imposta la cella attiva del foglio corrente. |
| [setActiveCellBgColor(Color value)](#setActiveCellBgColor-com.aspose.gridweb.Color-) | Specifica il colore di sfondo della cella attiva. |
| [setActiveCellColor(Color value)](#setActiveCellColor-com.aspose.gridweb.Color-) | Specifica il colore della cella attiva. |
| [setActiveHeaderBgColor(Color value)](#setActiveHeaderBgColor-com.aspose.gridweb.Color-) | Specifica il colore di sfondo dell'intestazione della riga/colonna attiva. |
| [setActiveHeaderColor(Color value)](#setActiveHeaderColor-com.aspose.gridweb.Color-) | Specifica il colore dell'intestazione della riga/colonna attiva. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | Imposta l'indice del foglio attivo. |
| [setActiveTabStyle(GridTableItemStyle value)](#setActiveTabStyle-com.aspose.gridweb.GridTableItemStyle-) | Specifica lo stile della scheda attiva. |
| [setAutoRefreshChart(boolean value)](#setAutoRefreshChart-boolean-) | Imposta se l'immagine del grafico viene aggiornata durante l'aggiornamento del valore della cella. Il valore predefinito è true. |
| [setBackColor(Color value)](#setBackColor-com.aspose.gridweb.Color-) | Imposta il BackColor nel WebControl |
| [setBeanID(String beanID)](#setBeanID-java.lang.String-) | imposta l'ID HTML del bean |
| [setBorderColor(Color value)](#setBorderColor-com.aspose.gridweb.Color-) | Imposta il BorderColor nel WebControl |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Imposta il BorderStyle nel WebControl |
| [setBorderWidth(Unit value)](#setBorderWidth-com.aspose.gridweb.Unit-) | Imposta la BorderWidth nel WebControl |
| [setBottomTableStyle(GridTableStyle value)](#setBottomTableStyle-com.aspose.gridweb.GridTableStyle-) | Imposta lo stile della barra inferiore del controllo. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Imposta se calcolare la formula dopo le modifiche al valore della cella o dopo l'importazione del file. |
| [setCssClass(String value)](#setCssClass-java.lang.String-) | Imposta la CssClass nel WebControl |
| [setCurrentPageIndex(int value)](#setCurrentPageIndex-int-) | Imposta l'indice della pagina corrente in modalità paginazione. |
| [setCustomCalculationEngine(GridAbstractCalculationEngine value)](#setCustomCalculationEngine-com.aspose.gridweb.GridAbstractCalculationEngine-) | Rappresenta il motore di calcolo personalizzato dell'utente per estendere il motore di calcolo predefinito di Aspose.Cells. |
| [setCustomStyle(InputStream stream)](#setCustomStyle-java.io.InputStream-) | Imposta il file di stile personalizzato da un flusso, includendo flusso di file su disco o flusso di memoria. |
| [setCustomStyleFileName(String value)](#setCustomStyleFileName-java.lang.String-) | Imposta il nome del file di stile personalizzato. |
| [setDPI(double value)](#setDPI-double-) | Ottiene /Imposta il DPI della macchina. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Imposta il nome del carattere predefinito del controllo. |
| [setDefaultFontSize(FontUnit value)](#setDefaultFontSize-com.aspose.gridweb.FontUnit-) | Imposta la dimensione predefinita del carattere del controllo. |
| [setDefaultGridLineColor(Color value)](#setDefaultGridLineColor-com.aspose.gridweb.Color-) | Imposta il colore predefinito della linea della griglia. |
| [setDisplayCellTip(boolean value)](#setDisplayCellTip-boolean-) | Imposta se mostrare i suggerimenti. Il valore predefinito è true. |
| [setEditMode(boolean value)](#setEditMode-boolean-) | Imposta la modalità di modifica del controllo. |
| [setEnableAJAX(boolean value)](#setEnableAJAX-boolean-) | Imposta se utilizzare chiamate AJAX. Il valore predefinito è true. |
| [setEnableAsync(boolean value)](#setEnableAsync-boolean-) | Imposta se caricare i dati delle celle in modo asincrono, consigliato per un foglio con più di 10000 celle. |
| [setEnableClientColumnOperations(boolean value)](#setEnableClientColumnOperations-boolean-) | Imposta se abilitare le operazioni di colonna lato client. |
| [setEnableClientFreeze(boolean value)](#setEnableClientFreeze-boolean-) | Imposta se abilitare le operazioni di congelamento lato client. |
| [setEnableClientMergeOperations(boolean value)](#setEnableClientMergeOperations-boolean-) | Imposta se abilitare le operazioni di unione lato client. |
| [setEnableClientResizeColumnRow(boolean value)](#setEnableClientResizeColumnRow-boolean-) | Imposta se abilitare il ridimensionamento di colonne e righe lato client. |
| [setEnableClientRowOperations(boolean value)](#setEnableClientRowOperations-boolean-) | Imposta se abilitare le operazioni di riga lato client. |
| [setEnableDoubleClickEvent(boolean value)](#setEnableDoubleClickEvent-boolean-) | Imposta se abilitare l'evento di doppio clic lato cliente. |
| [setEnableMetalLightEffect(boolean value)](#setEnableMetalLightEffect-boolean-) | Imposta se applicare l'effetto luce metallica. |
| [setEnablePaging(boolean value)](#setEnablePaging-boolean-) | Imposta se abilitare la modalità di paginazione del controllo. |
| [setEnableStyleDialogbox(boolean value)](#setEnableStyleDialogbox-boolean-) | Imposta se abilitare la finestra di dialogo di stile lato client. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Imposta l'Enabled nel WebControl |
| [setFilteredPaging(boolean value)](#setFilteredPaging-boolean-) | Imposta se abilitare la paginazione dopo il filtraggio dei dati; avrà effetto quando EnablePaging è true. |
| [setForceValidation(boolean value)](#setForceValidation-boolean-) | Imposta se forzare la convalida lato cliente. |
| [setForeColor(Color value)](#setForeColor-com.aspose.gridweb.Color-) | Imposta il ForeColor nel WebControl |
| [setFrameTableStyle(GridTableStyle value)](#setFrameTableStyle-com.aspose.gridweb.GridTableStyle-) | Imposta lo stile del frame del controllo. |
| [setGoonDefaultSaveOperation(boolean value)](#setGoonDefaultSaveOperation-boolean-) | Imposta se GridWeb eseguirà l'operazione di salvataggio predefinita; il valore predefinito è true. |
| [setHeaderBarHeight(Unit value)](#setHeaderBarHeight-com.aspose.gridweb.Unit-) | Imposta l'altezza (System.Web.UI.WebControl.Unit) della barra intestazione superiore del controllo. |
| [setHeaderBarStyle(GridTableItemStyle value)](#setHeaderBarStyle-com.aspose.gridweb.GridTableItemStyle-) | Imposta lo stile della barra intestazione. |
| [setHeaderBarTableStyle(GridTableStyle value)](#setHeaderBarTableStyle-com.aspose.gridweb.GridTableStyle-) | Imposta lo stile della barra intestazione del controllo. |
| [setHeaderBarWidth(Unit value)](#setHeaderBarWidth-com.aspose.gridweb.Unit-) | Imposta la larghezza (System.Web.UI.WebControl.Unit) della barra intestazione sinistra del controllo. |
| [setHeight(Unit value)](#setHeight-com.aspose.gridweb.Unit-) | Imposta l'altezza (System.Web.UI.WebControl.Unit) del controllo. |
| [setIgnoreStyleWithNoData(boolean value)](#setIgnoreStyleWithNoData-boolean-) | Imposta se GridWeb ignora la visualizzazione di righe o colonne che non contengono valori di cella ma sono comunque stilizzate. |
| [setLoadOptions(GridLoadOptions value)](#setLoadOptions-com.aspose.gridweb.GridLoadOptions-) | Rappresenta le opzioni di caricamento per GridWeb. |
| [setMaxColumn(int value)](#setMaxColumn-int-) | Imposta l'indice massimo di colonna visualizzata (basato su zero) del foglio web. |
| [setMaxRow(int value)](#setMaxRow-int-) | Imposta l'indice massimo di riga visualizzata (basato su zero) del foglio web. |
| [setMessage(String value)](#setMessage-java.lang.String-) | Imposta il messaggio per la griglia. |
| [setMinColumn(int value)](#setMinColumn-int-) | Imposta l'indice minimo di colonna visualizzata (basato su zero) del foglio web. |
| [setMinRow(int value)](#setMinRow-int-) | Imposta l'indice minimo di riga visualizzata (basato su zero) del foglio web. |
| [setNeedRenderGroupRows(boolean value)](#setNeedRenderGroupRows-boolean-) | Imposta se mostrare le righe di gruppo. |
| [setNoHScroll(boolean value)](#setNoHScroll-boolean-) | Imposta un valore che indica se la barra di scorrimento orizzontale è nascosta. |
| [setNoScroll(boolean value)](#setNoScroll-boolean-) | Imposta se mostrare la barra di scorrimento. |
| [setNoVScroll(boolean value)](#setNoVScroll-boolean-) | Imposta un valore che indica se la barra di scorrimento verticale è nascosta. |
| [setOnAjaxCallFinishedClientFunction(String value)](#setOnAjaxCallFinishedClientFunction-java.lang.String-) | Imposta il nome della funzione lato client da chiamare quando la chiamata ajax è terminata. |
| [setOnCellErrorClientFunction(String value)](#setOnCellErrorClientFunction-java.lang.String-) | Imposta il nome della funzione lato client da chiamare quando la convalida di una cella fallisce. |
| [setOnCellSelectedAjaxCallBackClientFunction(String value)](#setOnCellSelectedAjaxCallBackClientFunction-java.lang.String-) | Imposta la funzione lato client da chiamare quando una cella è selezionata. |
| [setOnCellSelectedClientFunction(String value)](#setOnCellSelectedClientFunction-java.lang.String-) | Imposta la funzione lato client da chiamare quando una cella è selezionata. |
| [setOnCellUnselectedClientFunction(String value)](#setOnCellUnselectedClientFunction-java.lang.String-) | Imposta la funzione lato client da chiamare quando una cella è deselezionata. |
| [setOnCellUpdatedClientFunction(String value)](#setOnCellUpdatedClientFunction-java.lang.String-) | Imposta il nome della funzione lato client da chiamare quando il valore di una cella viene aggiornato. |
| [setOnContextMenuShowClientFunction(String value)](#setOnContextMenuShowClientFunction-java.lang.String-) | Imposta la funzione lato client da chiamare quando verrà mostrato il menu contestuale. |
| [setOnDoubleClickCellClientFunction(String value)](#setOnDoubleClickCellClientFunction-java.lang.String-) | Imposta la funzione lato client da chiamare quando una cella viene doppio cliccata. |
| [setOnDoubleClickRowClientFunction(String value)](#setOnDoubleClickRowClientFunction-java.lang.String-) | Imposta la funzione lato client da chiamare quando una riga viene doppio cliccata. |
| [setOnGridInitClientFunction(String value)](#setOnGridInitClientFunction-java.lang.String-) | Imposta il nome della funzione lato client da chiamare quando la griglia viene inizializzata. |
| [setOnPageChangeClientFunction(String value)](#setOnPageChangeClientFunction-java.lang.String-) | Imposta la funzione lato client da chiamare dopo il cambio dell'indice di pagina. Ha effetto solo quando EnablePaging è true. |
| [setOnPageSubmitClientFunction(String value)](#setOnPageSubmitClientFunction-java.lang.String-) | Imposta la funzione client da chiamare prima che la pagina venga inviata lato client. |
| [setOnShapeSelectedClientFunction(String value)](#setOnShapeSelectedClientFunction-java.lang.String-) | Imposta la funzione lato client da chiamare quando una forma è selezionata. |
| [setOnSubmitClientFunction(String value)](#setOnSubmitClientFunction-java.lang.String-) | Imposta la funzione client da chiamare prima che il controllo venga inviato lato client. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Imposta se adattare solo le righe la cui altezza non è personalizzata; il valore predefinito è false. |
| [setPageSize(int value)](#setPageSize-int-) | Imposta la dimensione della pagina in modalità paginazione. |
| [setPictureCachePath(String value)](#setPictureCachePath-java.lang.String-) | Imposta il percorso di archiviazione delle immagini per la cartella di lavoro; tutte le forme e le immagini saranno memorizzate in questa directory. Il percorso predefinito è acwcache nella directory base dell'applicazione corrente. Gli utenti devono implementare un servizio di pianificazione per pulire i file scaduti dalla sessione. |
| [setPresetStyle(int value)](#setPresetStyle-int-) | Imposta lo stile predefinito. |
| [setRefreshValidation(boolean value)](#setRefreshValidation-boolean-) | Imposta se aggiornare il valore di convalida dopo le modifiche al valore della cella. |
| [setRenderHiddenRow(boolean value)](#setRenderHiddenRow-boolean-) | Imposta se la riga nascosta viene renderizzata in GridControl; il valore predefinito è false. |
| [setRowHeightForCSV(double value)](#setRowHeightForCSV-double-) | Imposta il valore dell'altezza della riga in punti per il file CSV; il valore predefinito è 14,5. |
| [setScrollBarArrowColor(Color value)](#setScrollBarArrowColor-com.aspose.gridweb.Color-) | Specifica il colore del pulsante freccia della barra di scorrimento. |
| [setScrollBarBaseColor(Color value)](#setScrollBarBaseColor-com.aspose.gridweb.Color-) | Specifica il colore della barra di scorrimento del controllo. |
| [setSelectCellBgColor(Color value)](#setSelectCellBgColor-com.aspose.gridweb.Color-) | Specifica il colore di sfondo delle celle selezionate nell'intervallo di selezione multipla. |
| [setSelectCellColor(Color value)](#setSelectCellColor-com.aspose.gridweb.Color-) | Specifica il colore delle celle selezionate nell'intervallo di selezione multipla. |
| [setSessionStorePath(String value)](#setSessionStorePath-java.lang.String-) | Imposta il percorso di memorizzazione della cache di sessione quando la modalità sessione è File o ViewState, ecc.: gridweb.SessionStorePath=\"c:/mytempdir/session\"; in tal caso i dati di sessione saranno memorizzati in c:/mytempdir/session. |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridweb.GridWorkbookSettings-) | Rappresenta le impostazioni della cartella di lavoro. |
| [setShowAddButton(boolean value)](#setShowAddButton-boolean-) | Imposta se mostrare il pulsante per aggiungere un foglio di lavoro. |
| [setShowBottomBar(boolean value)](#setShowBottomBar-boolean-) | Specifica se mostrare la barra dei comandi (include barra dei comandi e barra delle schede) nella parte inferiore del controllo. |
| [setShowCellEditBox(boolean value)](#setShowCellEditBox-boolean-) | Indica se Gridweb mostra la barra degli strumenti della casella di modifica come in MS-EXCEL. Se abilitata, una casella di modifica per la cella corrente verrà visualizzata in Gridweb. |
| [setShowCommandBarAtTop(boolean value)](#setShowCommandBarAtTop-boolean-) | Specifica se mostrare la barra dei comandi (include barra dei comandi e barra delle schede) nella parte superiore del controllo. |
| [setShowContextMenu(boolean value)](#setShowContextMenu-boolean-) | Imposta se mostrare il menu contestuale. Il valore predefinito è true. |
| [setShowDefaultGridLine(boolean value)](#setShowDefaultGridLine-boolean-) | Imposta se mostrare le linee di griglia predefinite delle celle. |
| [setShowHeaderBar(boolean value)](#setShowHeaderBar-boolean-) | Imposta se mostrare la barra dell'intestazione |
| [setShowLoading(boolean value)](#setShowLoading-boolean-) | Specifica se mostrare una finestra di dialogo di caricamento durante il postback al server. |
| [setShowLoadingPosition(String value)](#setShowLoadingPosition-java.lang.String-) | Specifica la posizione sinistra, superiore (in px) per mostrare la finestra di dialogo di caricamento durante il postback al server, ecc. 100,200 indica che la posizione sinistra e superiore della finestra di dialogo di caricamento è a 100px,200px. |
| [setShowSaveButton(boolean value)](#setShowSaveButton-boolean-) | Imposta se mostrare il pulsante di salvataggio. |
| [setShowSubmitButton(boolean value)](#setShowSubmitButton-boolean-) | Imposta se mostrare il pulsante di invio. |
| [setShowTabBar(boolean value)](#setShowTabBar-boolean-) | Imposta se mostrare la barra delle schede. |
| [setShowTabNavigation(boolean value)](#setShowTabNavigation-boolean-) | Imposta se il pulsante di navigazione delle schede è mostrato, il valore predefinito è true. |
| [setShowUndoButton(boolean value)](#setShowUndoButton-boolean-) | Imposta se mostrare il pulsante di annullamento. |
| [setSpanWrap(boolean value)](#setSpanWrap-boolean-) | Specifica se avvolgere il contenuto nello span di cella, il valore predefinito è true. |
| [setTabIndex(short value)](#setTabIndex-short-) | Imposta il TabIndex nel WebControl |
| [setTabStyle(GridTableItemStyle value)](#setTabStyle-com.aspose.gridweb.GridTableItemStyle-) | Imposta lo stile della barra delle schede. |
| [setToolTip(String value)](#setToolTip-java.lang.String-) | Imposta il ToolTip nel WebControl |
| [setUseClientPageHeight(boolean value)](#setUseClientPageHeight-boolean-) | Imposta se gridweb utilizza l'altezza della pagina client come altezza del controllo, adatto quando si imposta Height=\"100%\", il valore predefinito è false. |
| [setViewPanelScrollLeft(String value)](#setViewPanelScrollLeft-java.lang.String-) | Imposta la posizione della barra di scorrimento del pannello di visualizzazione della griglia. |
| [setViewPanelScrollTop(String value)](#setViewPanelScrollTop-java.lang.String-) | Imposta la posizione della barra di scorrimento del pannello di visualizzazione della griglia. |
| [setViewTableStyle(GridTableStyle value)](#setViewTableStyle-com.aspose.gridweb.GridTableStyle-) | Imposta lo stile del pannello di visualizzazione dei dati. |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Imposta la larghezza (System.Web.UI.WebControl.Unit) del controllo. |
| [setXhtmlMode(boolean value)](#setXhtmlMode-boolean-) | Imposta se utilizzare lo stile XHTML, il valore predefinito è true. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWebBean() {#GridWebBean--}
```
public GridWebBean()
```


il costruttore predefinito di GridWebBean

### AfterColumnFilter {#AfterColumnFilter}
```
public RowColumnEventHandler AfterColumnFilter
```


Si verifica dopo che la colonna è stata filtrata.

### AjaxCallFinished {#AjaxCallFinished}
```
public WorkbookEventHandler AjaxCallFinished
```


Viene attivato quando l'aggiornamento ajax del controllo è terminato. (EnableAJAX deve essere impostato su true)

### BeforeColumnFilter {#BeforeColumnFilter}
```
public RowColumnEventHandler BeforeColumnFilter
```


Si verifica prima che la colonna venga filtrata.

### CellClickOnAjax {#CellClickOnAjax}
```
public CellEventStringHandler CellClickOnAjax
```


Si verifica quando la cella viene cliccata, e è necessario eseguire un ajaxcallback per questo evento.

### CellClientUpdate {#CellClientUpdate}
```
public CellEventHandler CellClientUpdate
```


Si verifica quando avviene un aggiornamento di una cella client. Quando questo evento è attivato, il suo parametro e.Argument contiene il nome del comando.

### CellCommand {#CellCommand}
```
public CellEventHandler CellCommand
```


Si verifica quando si fa clic sul collegamento ipertestuale del comando di una cella. Quando questo evento è attivato, il suo parametro e.Argument contiene il nome del comando.

### CellDoubleClick {#CellDoubleClick}
```
public CellEventHandler CellDoubleClick
```


Si verifica quando la cella viene doppio-cliccata.

### CellModifiedOnAjax {#CellModifiedOnAjax}
```
public CellEventHandler CellModifiedOnAjax
```


Si verifica quando la cella viene modificata in ajaxcall.

### ColumnDeleted {#ColumnDeleted}
```
public RowColumnEventHandler ColumnDeleted
```


Si verifica quando l'utente elimina una colonna dal menu lato client.

### ColumnDeleting {#ColumnDeleting}
```
public RowColumnEventHandler ColumnDeleting
```


Si verifica quando l'utente tenta di eliminare una colonna dal menu lato client. È possibile gestire questo evento e impostare il parametro cancel su True per annullare l'operazione di eliminazione.

### ColumnDoubleClick {#ColumnDoubleClick}
```
public RowColumnEventHandler ColumnDoubleClick
```


Si verifica quando l'intestazione della colonna viene doppio-cliccata.

### ColumnInserted {#ColumnInserted}
```
public RowColumnEventHandler ColumnInserted
```


Si verifica quando l'utente inserisce una colonna dal menu lato client.

### CustomCommand {#CustomCommand}
```
public CustomCommandEventHandler CustomCommand
```


Si verifica quando l'utente clicca un pulsante di comando personalizzato.

### LoadCustomData {#LoadCustomData}
```
public WorkbookEventHandler LoadCustomData
```


Viene attivato quando SessionMode del controllo è impostato su Custom e deve caricare i dati del foglio. È possibile gestire questo evento in modalità Sessione Personalizzata per caricare i dati del foglio da file o database.

### PageIndexChanged {#PageIndexChanged}
```
public WorkbookEventHandler PageIndexChanged
```


Si verifica quando l'indice della pagina del foglio del controllo è cambiato.

### RowDeleted {#RowDeleted}
```
public RowColumnEventHandler RowDeleted
```


Si verifica quando l'utente ha eliminato una riga dal menu lato client.

### RowDeleting {#RowDeleting}
```
public RowColumnEventHandler RowDeleting
```


Si verifica quando l'utente tenta di eliminare una riga dal menu lato client. È possibile gestire questo evento e lanciare un'eccezione RejectDeleteException per annullare l'operazione di eliminazione.

### RowDoubleClick {#RowDoubleClick}
```
public RowColumnEventHandler RowDoubleClick
```


Si verifica quando l'intestazione della riga viene doppio cliccata.

### RowInserted {#RowInserted}
```
public RowColumnEventHandler RowInserted
```


Si verifica quando l'utente inserisce una riga dal menu lato client.

### SaveCommand {#SaveCommand}
```
public WorkbookEventHandler SaveCommand
```


Si verifica quando il pulsante "save" viene cliccato.

### SheetAdded {#SheetAdded}
```
public SheetEventHandler SheetAdded
```


Si verifica quando l'utente aggiunge un foglio di lavoro dal menu della barra degli strumenti.

### SheetTabClick {#SheetTabClick}
```
public WorkbookEventHandler SheetTabClick
```


Si verifica quando la scheda del foglio viene cliccata.

### SubmitCommand {#SubmitCommand}
```
public WorkbookEventHandler SubmitCommand
```


Si verifica quando il pulsante "submit" viene cliccato.

### UndoCommand {#UndoCommand}
```
public WorkbookEventHandler UndoCommand
```


Si verifica quando il pulsante "undo" viene cliccato.

### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


Calcola il risultato delle formule.

### createChildControls() {#createChildControls--}
```
public void createChildControls()
```


Implementa CreateChildControls da WebControl, utilizzato internamente solo.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getACWClientPath() {#getACWClientPath--}
```
public String getACWClientPath()
```


Ottiene il percorso web dei file script/immagine del controllo. Per esempio: \"http://localhost/acw\\_client\". È possibile impostare questo valore anche nel file web.config. Aggiungere questa sezione alla sezione `<configuration>`:
`<appSettings>`
`<add key=\"aspose.cells.gridweb.acw_client_path\" value=\"/acw_client/\" />`
`</appSettings>`


**Returns:**
java.lang.String
### getACWLanguageFileUrl() {#getACWLanguageFileUrl--}
```
public String getACWLanguageFileUrl()
```


Ottiene l'URL web del file di lingua del controllo. Per esempio: \"/acw\\_client/lang\\_en.js\".
Per impostazione predefinita, viene utilizzato un file inglese integrato.


**Returns:**
java.lang.String
### getActiveCell() {#getActiveCell--}
```
public GridCell getActiveCell()
```


Ottiene la cella attiva del foglio corrente. Modificata per essere scrivibile dalla versione 1.9.0.1.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getActiveCellBgColor() {#getActiveCellBgColor--}
```
public Color getActiveCellBgColor()
```


Specifica il colore di sfondo della cella attiva.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveCellColor() {#getActiveCellColor--}
```
public Color getActiveCellColor()
```


Specifica il colore della cella attiva.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveHeaderBgColor() {#getActiveHeaderBgColor--}
```
public Color getActiveHeaderBgColor()
```


Specifica il colore di sfondo dell'intestazione della riga/colonna attiva.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveHeaderColor() {#getActiveHeaderColor--}
```
public Color getActiveHeaderColor()
```


Specifica il colore dell'intestazione della riga/colonna attiva.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveSheet() {#getActiveSheet--}
```
public GridWorksheet getActiveSheet()
```


Ottiene il foglio attivo

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet)
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


Ottiene l'indice del foglio attivo. Uguale a WebWorksheets.ActiveSheetIndex.

**Returns:**
int
### getActiveTabStyle() {#getActiveTabStyle--}
```
public GridTableItemStyle getActiveTabStyle()
```


Specifica lo stile della scheda attiva.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getAutoRefreshChart() {#getAutoRefreshChart--}
```
public boolean getAutoRefreshChart()
```


Ottiene se l'immagine del grafico viene aggiornata durante l'aggiornamento del valore della cella; il valore predefinito è true.

**Returns:**
boolean
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


Ottiene il BackColor nel WebControl

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBeanID() {#getBeanID--}
```
public String getBeanID()
```


ottieni l'id html del bean

**Returns:**
java.lang.String
### getBorderColor() {#getBorderColor--}
```
public Color getBorderColor()
```


Ottiene il BorderColor nel WebControl

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Ottiene il BorderStyle nel WebControl

Vedi [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Returns:**
int
### getBorderWidth() {#getBorderWidth--}
```
public Unit getBorderWidth()
```


Ottiene il BorderWidth nel WebControl

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getBottomTableStyle() {#getBottomTableStyle--}
```
public GridTableStyle getBottomTableStyle()
```


Ottiene lo stile della barra inferiore del controllo.

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


Ottiene la CssClass nel WebControl

**Returns:**
java.lang.String
### getCurrentPageIndex() {#getCurrentPageIndex--}
```
public int getCurrentPageIndex()
```


Ottiene l'indice della pagina corrente in modalità paginazione.

**Remarks**

Quando è in modalità di paginazione, il controllo visualizzerà una volta PageSize righe di dati e mostrerà il controllo di selezione della pagina nella barra delle schede.

**Returns:**
int
### getCustomCalculationEngine() {#getCustomCalculationEngine--}
```
public GridAbstractCalculationEngine getCustomCalculationEngine()
```


Rappresenta il motore di calcolo personalizzato dell'utente per estendere il motore di calcolo predefinito di Aspose.Cells.

**Returns:**
[GridAbstractCalculationEngine](../../com.aspose.gridweb/gridabstractcalculationengine)
### getCustomCommandButtons() {#getCustomCommandButtons--}
```
public CustomCommandButtonCollection getCustomCommandButtons()
```


Ottiene la raccolta dei pulsanti di comando personalizzati

**Returns:**
[CustomCommandButtonCollection](../../com.aspose.gridweb/customcommandbuttoncollection)
### getCustomStyleFileName() {#getCustomStyleFileName--}
```
public String getCustomStyleFileName()
```


Ottiene il nome del file di stile personalizzato.

**Remarks**

Il file di stile personalizzato è un file XML. Quando imposti il nome del file, il file verrà caricato immediatamente. Ecco il contenuto del "stile predefinito standard" ------------------------------------------------------- <Aspose.Cells.GridWeb.ViewerStyleTemplate runat="server" HeaderBarWidth="30pt" ScrollBarBaseColor="" FrameTableStyle-BorderStyle="Solid" FrameTableStyle-LeftBorderStyle-BorderWidth="" FrameTableStyle-LeftBorderStyle-BorderColor="" FrameTableStyle-RightBorderStyle-BorderWidth="" FrameTableStyle-RightBorderStyle-BorderColor="" FrameTableStyle-BorderWidth="1px" FrameTableStyle-CellSpacing="0" FrameTableStyle-BorderColor="Gray" FrameTableStyle-CellPadding="0" FrameTableStyle-TopBorderStyle-BorderWidth="" FrameTableStyle-TopBorderStyle-BorderColor="" FrameTableStyle-BottomBorderStyle-BorderWidth="" FrameTableStyle-BottomBorderStyle-BorderColor="" HeaderBarStyle-LeftBorderStyle-BorderStyle="Solid" HeaderBarStyle-LeftBorderStyle-BorderWidth="1px" HeaderBarStyle-LeftBorderStyle-BorderColor="White" HeaderBarStyle-VerticalAlign="Middle" HeaderBarStyle-RightBorderStyle-BorderStyle="Solid" HeaderBarStyle-RightBorderStyle-BorderWidth="1px" HeaderBarStyle-RightBorderStyle-BorderColor="Gray" HeaderBarStyle-BorderWidth="1px" HeaderBarStyle-Font-Size="10pt" HeaderBarStyle-BorderColor="Gray" HeaderBarStyle-BorderStyle="Solid" HeaderBarStyle-HorizontalAlign="Center" HeaderBarStyle-ForeColor="Black" HeaderBarStyle-TopBorderStyle-BorderStyle="Solid" HeaderBarStyle-TopBorderStyle-BorderWidth="1px" HeaderBarStyle-TopBorderStyle-BorderColor="White" HeaderBarStyle-BackColor="\#E0E0E0" HeaderBarStyle-BottomBorderStyle-BorderStyle="Solid" HeaderBarStyle-BottomBorderStyle-BorderWidth="1px" HeaderBarStyle-BottomBorderStyle-BorderColor="Gray" ViewTableStyle-LeftBorderStyle-BorderWidth="" ViewTableStyle-LeftBorderStyle-BorderColor="" ViewTableStyle-LayoutFixed="Fixed" ViewTableStyle-RightBorderStyle-BorderWidth="" ViewTableStyle-RightBorderStyle-BorderColor="" ViewTableStyle-BorderWidth="0px" ViewTableStyle-CellSpacing="0" ViewTableStyle-CellPadding="0" ViewTableStyle-TopBorderStyle-BorderWidth="" ViewTableStyle-TopBorderStyle-BorderColor="" ViewTableStyle-BottomBorderStyle-BorderWidth="" ViewTableStyle-BottomBorderStyle-BorderColor="" BottomTableStyle-LeftBorderStyle-BorderWidth="" BottomTableStyle-LeftBorderStyle-BorderColor="" BottomTableStyle-LayoutFixed="Fixed" BottomTableStyle-RightBorderStyle-BorderWidth="" BottomTableStyle-RightBorderStyle-BorderColor="" BottomTableStyle-BorderWidth="0px" BottomTableStyle-CellSpacing="0" BottomTableStyle-CellPadding="1" BottomTableStyle-TopBorderStyle-BorderStyle="Solid" BottomTableStyle-TopBorderStyle-BorderWidth="1px" BottomTableStyle-TopBorderStyle-BorderColor="Gray" BottomTableStyle-BottomBorderStyle-BorderWidth="" BottomTableStyle-BottomBorderStyle-BorderColor="" HeaderBarHeight="15pt" ActiveTabStyle-LeftBorderStyle-BorderWidth="" ActiveTabStyle-LeftBorderStyle-BorderColor="" ActiveTabStyle-RightBorderStyle-BorderWidth="" ActiveTabStyle-RightBorderStyle-BorderColor="" ActiveTabStyle-Height="15pt" ActiveTabStyle-BorderWidth="1px" ActiveTabStyle-Font-Size="10pt" ActiveTabStyle-BorderColor="Gray" ActiveTabStyle-ForeColor="Black" ActiveTabStyle-TopBorderStyle-BorderWidth="" ActiveTabStyle-TopBorderStyle-BorderColor="" ActiveTabStyle-BackColor="White" ActiveTabStyle-BottomBorderStyle-BorderWidth="" ActiveTabStyle-BottomBorderStyle-BorderColor="" HeaderBarTableStyle-LeftBorderStyle-BorderWidth="" HeaderBarTableStyle-LeftBorderStyle-BorderColor="" HeaderBarTableStyle-LayoutFixed="Fixed" HeaderBarTableStyle-RightBorderStyle-BorderWidth="" HeaderBarTableStyle-RightBorderStyle-BorderColor="" HeaderBarTableStyle-BorderWidth="0px" HeaderBarTableStyle-CellSpacing="0" HeaderBarTableStyle-BorderCollapse="Separate" HeaderBarTableStyle-CellPadding="0" HeaderBarTableStyle-TopBorderStyle-BorderWidth="" HeaderBarTableStyle-TopBorderStyle-BorderColor="" HeaderBarTableStyle-BottomBorderStyle-BorderWidth="" HeaderBarTableStyle-BottomBorderStyle-BorderColor="" TabStyle-LeftBorderStyle-BorderWidth="" TabStyle-LeftBorderStyle-BorderColor="" TabStyle-RightBorderStyle-BorderWidth="" TabStyle-RightBorderStyle-BorderColor="" TabStyle-Height="15pt" TabStyle-BorderWidth="1px" TabStyle-Font-Size="10pt" TabStyle-BorderColor="Gray" TabStyle-ForeColor="Black" TabStyle-TopBorderStyle-BorderWidth="" TabStyle-TopBorderStyle-BorderColor="" TabStyle-BackColor="\#E0E0E0" TabStyle-BottomBorderStyle-BorderWidth="" TabStyle-BottomBorderStyle-BorderColor="" ScrollBarArrowColor=""></Aspose.Cells.GridWeb.ViewerStyleTemplate>

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


Ottiene /Imposta il DPI della macchina.

**Remarks**

**Returns:**
double
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Ottiene il nome del carattere predefinito del controllo.

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


Ottiene la dimensione predefinita del carattere del controllo.

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


Ottiene il colore predefinito della linea della griglia.

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


Ottiene se mostrare i suggerimenti. Il valore predefinito è true.

**Returns:**
boolean
### getEditMode() {#getEditMode--}
```
public boolean getEditMode()
```


Ottiene la modalità di modifica del controllo.

**Remarks**

Quando impostato su true, le celle del controllo sono modificabili e le icone "save" e "undo" vengono visualizzate. Quando impostato su false, le celle del controllo sono di sola lettura e le icone "save" e "undo" non vengono visualizzate.

**Returns:**
boolean
### getEnableAJAX() {#getEnableAJAX--}
```
public boolean getEnableAJAX()
```


Ottiene se utilizzare la chiamata AJAX. Il valore predefinito è true.

**Returns:**
boolean
### getEnableAsync() {#getEnableAsync--}
```
public boolean getEnableAsync()
```


Ottiene se caricare i dati delle celle in modo asincrono, suggerito per un foglio con più di 10000 celle.

**Returns:**
boolean
### getEnableClientColumnOperations() {#getEnableClientColumnOperations--}
```
public boolean getEnableClientColumnOperations()
```


Ottiene se abilitare le operazioni di colonna lato client.

**Remarks**

Quando impostato su true, l'utente può utilizzare il menu contestuale per aggiungere/rimuovere colonne.

**Returns:**
boolean
### getEnableClientFreeze() {#getEnableClientFreeze--}
```
public boolean getEnableClientFreeze()
```


Ottiene se abilitare le operazioni di congelamento lato client.

**Remarks**

Quando impostato su true, l'utente può utilizzare il menu contestuale per bloccare/sbloccare i riquadri.

**Returns:**
boolean
### getEnableClientMergeOperations() {#getEnableClientMergeOperations--}
```
public boolean getEnableClientMergeOperations()
```


Ottiene se abilitare le operazioni di unione lato client.

**Remarks**

Quando impostato su true, l'utente può utilizzare il menu contestuale per unire/separare le celle.

**Returns:**
boolean
### getEnableClientResizeColumnRow() {#getEnableClientResizeColumnRow--}
```
public boolean getEnableClientResizeColumnRow()
```


Ottiene se abilitare il ridimensionamento di colonne e righe lato client.

**Remarks**

Quando impostato su true, l'utente può ridimensionare la colonna e la riga sul lato client.

**Returns:**
boolean
### getEnableClientRowOperations() {#getEnableClientRowOperations--}
```
public boolean getEnableClientRowOperations()
```


Ottiene se abilitare le operazioni di riga lato client.

**Remarks**

Quando impostato su true, l'utente può utilizzare il menu contestuale per aggiungere/rimuovere righe.

**Returns:**
boolean
### getEnableDoubleClickEvent() {#getEnableDoubleClickEvent--}
```
public boolean getEnableDoubleClickEvent()
```


Ottiene se abilitare l'evento di doppio clic lato cliente.

**Remarks**

Quando impostato su true, il controllo riceverà gli eventi di doppio clic dal lato client e potrai gestire questi eventi sul lato server. Altrimenti il controllo ignorerà tutti gli eventi di doppio clic.

**Returns:**
boolean
### getEnableMetalLightEffect() {#getEnableMetalLightEffect--}
```
public boolean getEnableMetalLightEffect()
```


Ottiene se applicare l'effetto luce metallica.

**Returns:**
boolean
### getEnablePaging() {#getEnablePaging--}
```
public boolean getEnablePaging()
```


Ottiene se abilitare la modalità di paginazione del controllo.

**Remarks**

Quando impostato su true, il controllo visualizzerà una volta PageSize righe di dati e mostrerà il controllo di selezione pagina nella barra delle schede.

**Returns:**
boolean
### getEnableStyleDialogbox() {#getEnableStyleDialogbox--}
```
public boolean getEnableStyleDialogbox()
```


Ottiene se abilitare la finestra di dialogo stile lato client.

**Remarks**

Quando impostato su true, l'utente può utilizzare la finestra di dialogo stile per impostare lo stile di una cella selezionando "Format Cell..." dal menu a comparsa.

**Returns:**
boolean
### getEnabled() {#getEnabled--}
```
public boolean getEnabled()
```


Ottiene l'Enabled nel WebControl

**Returns:**
boolean
### getFilteredPaging() {#getFilteredPaging--}
```
public boolean getFilteredPaging()
```


Ottiene se abilitare la paginazione dopo il filtraggio dei dati, avrà effetto quando EnablePaging è true.

**Remarks**

Quando impostato su true, il controllo paginerà in base ai dati filtrati; il valore predefinito è false.

**Returns:**
boolean
### getFont() {#getFont--}
```
public FontInfo getFont()
```


Ottiene il Font nel WebControl

**Returns:**
[FontInfo](../../com.aspose.gridweb/fontinfo)
### getForceValidation() {#getForceValidation--}
```
public boolean getForceValidation()
```


Ottiene se forzare la convalida lato cliente.

**Remarks**

Quando impostato su true, i dati non verranno inviati al server finché tutti i campi di input non saranno validi.

**Returns:**
boolean
### getForeColor() {#getForeColor--}
```
public Color getForeColor()
```


Ottiene il ForeColor nel WebControl

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getFrameTableStyle() {#getFrameTableStyle--}
```
public GridTableStyle getFrameTableStyle()
```


Ottiene lo stile del frame del controllo.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getGoonDefaultSaveOperation() {#getGoonDefaultSaveOperation--}
```
public boolean getGoonDefaultSaveOperation()
```


Ottiene se GridWeb eseguirà l'operazione di salvataggio predefinita, il valore predefinito è true.

**Returns:**
boolean
### getHTMLBody() {#getHTMLBody--}
```
public String getHTMLBody()
```


il codice html del bean per il corpo html, deve essere ottenuto dopo la chiamata del metodo init e prepareRender

**Returns:**
java.lang.String
### getHTMLHead() {#getHTMLHead--}
```
public String getHTMLHead()
```


il codice HTML del bean per l'intestazione HTML, deve essere ottenuto dopo la chiamata del metodo init e prepareRender

**Returns:**
java.lang.String
### getHeaderBarHeight() {#getHeaderBarHeight--}
```
public Unit getHeaderBarHeight()
```


Ottiene l'altezza (System.Web.UI.WebControl.Unit) della barra dell'intestazione superiore del controllo.

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


Ottiene lo stile della barra dell'intestazione.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getHeaderBarTableStyle() {#getHeaderBarTableStyle--}
```
public GridTableStyle getHeaderBarTableStyle()
```


Ottiene lo stile della barra dell'intestazione del controllo.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getHeaderBarWidth() {#getHeaderBarWidth--}
```
public Unit getHeaderBarWidth()
```


Ottiene la larghezza( System.Web.UI.WebControl.Unit ) o la barra dell'intestazione sinistra del controllo.

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


Ottiene l'altezza( System.Web.UI.WebControl.Unit ) del controllo.

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


Restituisce se GridWeb ignora la visualizzazione di righe o colonne che non contengono valori di cella ma sono comunque formattate. Se impostato su true, le prestazioni saranno migliori. Il valore predefinito è false, il che significa che se l'ultima riga/colonna consecutiva non ha valori di cella ma è formattata, verrà comunque visualizzata. Questa opzione è valida solo quando EnableAsync è false. Questa opzione non ha effetto quando EnableAsync è true, il che significa che GridWeb mostrerà tutte le righe/colonne con stile.

**Returns:**
boolean
### getLoadOptions() {#getLoadOptions--}
```
public GridLoadOptions getLoadOptions()
```


Rappresenta le opzioni di caricamento per GridWeb.

**Returns:**
[GridLoadOptions](../../com.aspose.gridweb/gridloadoptions)
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Restituisce l'indice massimo di colonna visualizzata (basato su zero) del foglio web. Il controllo utilizza il valore più grande tra MaxColumn e la colonna massima dei dati del foglio.

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


Restituisce l'indice massimo di riga visualizzata (basato su zero) del foglio web. Il controllo utilizza il valore più grande tra MaxRow e la riga massima dei dati del foglio.

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


Ottiene il messaggio per la griglia.

**Returns:**
java.lang.String
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


Restituisce l'indice minimo di colonna visualizzata (basato su zero) del foglio web. Il controllo utilizza il valore più piccolo tra MinColumn e la colonna minima dei dati del foglio.

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


Restituisce l'indice minimo di riga visualizzata (basato su zero) del foglio web. Il controllo utilizza il valore più piccolo tra MinRow e la riga minima dei dati del foglio.

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


Ottiene la raccolta delle celle modificate dal client.

**Returns:**
java.util.ArrayList
### getNeedRenderGroupRows() {#getNeedRenderGroupRows--}
```
public boolean getNeedRenderGroupRows()
```


Ottiene se mostrare le righe di gruppo .

**Returns:**
boolean
### getNoHScroll() {#getNoHScroll--}
```
public boolean getNoHScroll()
```


Ottiene un valore che indica se la barra di scorrimento orizzontale è nascosta.

**Returns:**
boolean
### getNoScroll() {#getNoScroll--}
```
public boolean getNoScroll()
```


Ottiene se mostrare la barra di scorrimento .

**Returns:**
boolean
### getNoVScroll() {#getNoVScroll--}
```
public boolean getNoVScroll()
```


Ottiene un valore che indica se la barra di scorrimento verticale è nascosta.

**Returns:**
boolean
### getOnAjaxCallFinishedClientFunction() {#getOnAjaxCallFinishedClientFunction--}
```
public String getOnAjaxCallFinishedClientFunction()
```


Restituisce il nome della funzione lato client da chiamare quando ajaxcall è terminato. La funzione client dovrebbe essere dichiarata così:
function GridAjaxcallFinished()
\{
alert(this.id+" ajaxcall finished ");
\}

Nota: è possibile utilizzare il puntatore "this" nella funzione client per fare riferimento al controllo grid che genera l'evento.

**Returns:**
java.lang.String
### getOnCellErrorClientFunction() {#getOnCellErrorClientFunction--}
```
public String getOnCellErrorClientFunction()
```


Restituisce il nome della funzione lato client da chiamare quando la convalida di una cella fallisce. La funzione client dovrebbe essere dichiarata così:
function MyOnCellError(cell)
\{
alert(this.getCellValueByCell(cell));
\}

Nota: è possibile utilizzare il puntatore "this" nella funzione client per fare riferimento al controllo grid che genera l'evento.

**Returns:**
java.lang.String
### getOnCellSelectedAjaxCallBackClientFunction() {#getOnCellSelectedAjaxCallBackClientFunction--}
```
public String getOnCellSelectedAjaxCallBackClientFunction()
```


Ottiene la funzione lato client da chiamare quando una cella è selezionata. La funzione client dovrebbe essere dichiarata così:
function MyOnSelectCellAjaxCallBack(cell,customerdata)
\{

\}

Nota: è possibile utilizzare il puntatore "this" nella funzione client per fare riferimento al controllo grid che genera l'evento.

**Returns:**
java.lang.String
### getOnCellSelectedClientFunction() {#getOnCellSelectedClientFunction--}
```
public String getOnCellSelectedClientFunction()
```


Ottiene la funzione lato client da chiamare quando una cella è selezionata. La funzione client dovrebbe essere dichiarata così:
function MyOnSelectCell(cell)
\{
GridWeb1.setCellValueByCell(cell, "test");
\}

Nota: è possibile utilizzare il puntatore "this" nella funzione client per fare riferimento al controllo grid che genera l'evento.

**Returns:**
java.lang.String
### getOnCellUnselectedClientFunction() {#getOnCellUnselectedClientFunction--}
```
public String getOnCellUnselectedClientFunction()
```


Ottiene la funzione lato client da chiamare quando una cella è deselezionata. La funzione client dovrebbe essere dichiarata così:
function MyOnUnselectCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

Nota: è possibile utilizzare il puntatore "this" nella funzione client per fare riferimento al controllo grid che genera l'evento.

**Returns:**
java.lang.String
### getOnCellUpdatedClientFunction() {#getOnCellUpdatedClientFunction--}
```
public String getOnCellUpdatedClientFunction()
```


Ottiene il nome della funzione lato client da chiamare quando il valore di una cella viene aggiornato. La funzione client dovrebbe essere dichiarata così:
function MyOnCellUpdated(cell)
\{
alert(this.getCellValueByCell(cell));
\}

Nota: è possibile utilizzare il puntatore "this" nella funzione client per fare riferimento al controllo grid che genera l'evento.

**Returns:**
java.lang.String
### getOnContextMenuShowClientFunction() {#getOnContextMenuShowClientFunction--}
```
public String getOnContextMenuShowClientFunction()
```


Ottiene la funzione lato client da chiamare quando verrà mostrato il menu contestuale. La funzione client dovrebbe essere dichiarata così:
function onContextMenuShow()
\{
var menu = event.srcElement;
menu.setItemVisibility("Delete", "block");
menu.setItemVisibility("Update", "none");
\}

Nota: è possibile utilizzare il puntatore "this" nella funzione client per fare riferimento al controllo grid che genera l'evento.

**Returns:**
java.lang.String
### getOnDoubleClickCellClientFunction() {#getOnDoubleClickCellClientFunction--}
```
public String getOnDoubleClickCellClientFunction()
```


Ottiene la funzione lato client da chiamare quando una cella viene doppio cliccata. La funzione client dovrebbe essere dichiarata così:
function MyOnDoubleClickCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

Nota: è possibile utilizzare il puntatore "this" nella funzione client per fare riferimento al controllo grid che genera l'evento.

**Returns:**
java.lang.String
### getOnDoubleClickRowClientFunction() {#getOnDoubleClickRowClientFunction--}
```
public String getOnDoubleClickRowClientFunction()
```


Ottiene la funzione lato client da chiamare quando una riga viene doppio cliccata. La funzione client dovrebbe essere dichiarata così:
function MyOnRowDoubleClick(row)
\{
alert(row);
\}

Nota: è possibile utilizzare il puntatore "this" nella funzione client per fare riferimento al controllo grid che genera l'evento.

**Returns:**
java.lang.String
### getOnGridInitClientFunction() {#getOnGridInitClientFunction--}
```
public String getOnGridInitClientFunction()
```


Ottiene il nome della funzione lato client da chiamare quando la griglia viene inizializzata. La funzione client dovrebbe essere dichiarata così:
function MyOnGridInit(grid)
\{
alert("La griglia è inizializzata: " + grid.id);
\}

Nota: è possibile utilizzare il puntatore "this" nella funzione client per fare riferimento al controllo grid che genera l'evento.

**Returns:**
java.lang.String
### getOnPageChangeClientFunction() {#getOnPageChangeClientFunction--}
```
public String getOnPageChangeClientFunction()
```


Ottiene la funzione lato client da chiamare dopo il cambiamento dell'indice di pagina. Ha effetto solo quando EnablePaging è true. La funzione client dovrebbe essere dichiarata così:
function MyOnPageChange(index)
\{
console.log("la pagina corrente è:"+index);
\}

Nota: è possibile utilizzare il puntatore "this" nella funzione client per fare riferimento al controllo grid che genera l'evento.

**Returns:**
java.lang.String
### getOnPageSubmitClientFunction() {#getOnPageSubmitClientFunction--}
```
public String getOnPageSubmitClientFunction()
```


Ottiene la funzione client da chiamare prima che la pagina venga inviata lato client.

**Returns:**
java.lang.String
### getOnShapeSelectedClientFunction() {#getOnShapeSelectedClientFunction--}
```
public String getOnShapeSelectedClientFunction()
```


Ottiene la funzione lato client da chiamare quando una forma è selezionata. La funzione client dovrebbe essere dichiarata così:
function MyOnSelectShape(shape)
\{
var name=shape.getAttribute("namevalue")
var text=shape.getAttribute("textvalue")
var value=shape.getAttribute("controlvalue")
var type=shape.getAttribute("msotype")
\}

Nota: è possibile utilizzare il puntatore "this" nella funzione client per fare riferimento al controllo grid che genera l'evento.

**Returns:**
java.lang.String
### getOnSubmitClientFunction() {#getOnSubmitClientFunction--}
```
public String getOnSubmitClientFunction()
```


Ottiene la funzione client da chiamare prima che il controllo venga inviato lato client. La funzione client dovrebbe essere dichiarata così:
function MyOnSubmit(arg, cancelEdit)
\{
return true;
\}
L'arg è l'argomento di invio, contiene il comando da inviare al server. Il cancelEdit è un valore booleano che indica se il controllo ha scartato l'input dell'utente prima dell'invio. Il controllo continuerà a inviare se la funzione restituisce true.
Nota: è possibile utilizzare il puntatore "this" nella funzione client per fare riferimento al controllo grid che genera l'evento.

**Returns:**
java.lang.String
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


Ottiene se adattare solo le righe la cui altezza non è personalizzata, il valore predefinito è false.

**Returns:**
boolean
### getPageSize() {#getPageSize--}
```
public int getPageSize()
```


Ottiene la dimensione della pagina in modalità paginazione.

**Remarks**

Quando è in modalità di paginazione, il controllo visualizzerà una volta PageSize righe di dati e mostrerà il controllo di selezione della pagina nella barra delle schede.

**Returns:**
int
### getPictureCachePath() {#getPictureCachePath--}
```
public static String getPictureCachePath()
```


Ottiene il percorso di archiviazione delle immagini per la cartella di lavoro, tutte le forme e le immagini saranno memorizzate in questa directory, il percorso predefinito è acwcache nella directory base dell'applicazione corrente; gli utenti devono implementare un servizio di pianificazione per pulire i file fuori dal tempo di sessione.

**Returns:**
java.lang.String
### getPresetStyle() {#getPresetStyle--}
```
public int getPresetStyle()
```


Ottiene lo stile predefinito.

Vedi [PresetStyle](../../com.aspose.gridweb/presetstyle).

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


Ottiene se aggiornare il valore di convalida dopo che il valore della cella è cambiato.

**Returns:**
boolean
### getRenderHiddenRow() {#getRenderHiddenRow--}
```
public boolean getRenderHiddenRow()
```


Ottiene se la riga nascosta è renderizzata in GridControl, il valore predefinito è false. Se devi rendere visibile la riga nascosta in seguito, dovrai impostarla su true.

**Returns:**
boolean
### getRowHeightForCSV() {#getRowHeightForCSV--}
```
public double getRowHeightForCSV()
```


Ottiene il valore dell'altezza della riga in punti per il file csv, il valore predefinito è 14,5.

**Returns:**
double
### getScrollBarArrowColor() {#getScrollBarArrowColor--}
```
public Color getScrollBarArrowColor()
```


Specifica il colore del pulsante freccia della barra di scorrimento.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getScrollBarBaseColor() {#getScrollBarBaseColor--}
```
public Color getScrollBarBaseColor()
```


Specifica il colore della barra di scorrimento del controllo.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCellBgColor() {#getSelectCellBgColor--}
```
public Color getSelectCellBgColor()
```


Specifica il colore di sfondo delle celle selezionate nell'intervallo di selezione multipla.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCellColor() {#getSelectCellColor--}
```
public Color getSelectCellColor()
```


Specifica il colore delle celle selezionate nell'intervallo di selezione multipla.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSessionStorePath() {#getSessionStorePath--}
```
public String getSessionStorePath()
```


Ottiene il percorso di archiviazione della cache di sessione quando la modalità sessione è File o ViewState, ecc.: gridweb.SessionStorePath=\"c:/mytempdir/session\"; quindi i dati di sessione saranno memorizzati in c:/mytempdir/session.

**Returns:**
java.lang.String
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


Rappresenta le impostazioni della cartella di lavoro.

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridweb/gridworkbooksettings)
### getShowAddButton() {#getShowAddButton--}
```
public boolean getShowAddButton()
```


Ottiene se mostrare il pulsante aggiungi foglio di lavoro.

**Returns:**
boolean
### getShowBottomBar() {#getShowBottomBar--}
```
public boolean getShowBottomBar()
```


Specifica se mostrare la barra dei comandi (include barra dei comandi e barra delle schede) nella parte inferiore del controllo.

**Returns:**
boolean
### getShowCellEditBox() {#getShowCellEditBox--}
```
public boolean getShowCellEditBox()
```


Indica se Gridweb mostra la barra degli strumenti della casella di modifica come in MS-EXCEL. Se abilitata, una casella di modifica per la cella corrente verrà visualizzata in Gridweb. Se attiviamo questa funzionalità, è necessario importare la libreria jquery js nei tuoi file aspx per supportare la nuova funzionalità. Qualsiasi versione recente di jquery va bene, ecc.

**Returns:**
boolean
### getShowCommandBarAtTop() {#getShowCommandBarAtTop--}
```
public boolean getShowCommandBarAtTop()
```


Specifica se mostrare la barra dei comandi (include barra dei comandi e barra delle schede) nella parte superiore del controllo.

**Returns:**
boolean
### getShowContextMenu() {#getShowContextMenu--}
```
public boolean getShowContextMenu()
```


Ottiene se mostrare il menu contestuale. Il valore predefinito è true.

**Returns:**
boolean
### getShowDefaultGridLine() {#getShowDefaultGridLine--}
```
public boolean getShowDefaultGridLine()
```


Ottiene se mostrare le linee di griglia predefinite delle celle.

**Returns:**
boolean
### getShowHeaderBar() {#getShowHeaderBar--}
```
public boolean getShowHeaderBar()
```


Ottiene se mostrare la barra dell'intestazione

**Returns:**
boolean
### getShowLoading() {#getShowLoading--}
```
public boolean getShowLoading()
```


Specifica se mostrare una finestra di dialogo di caricamento durante il postback al server.

**Returns:**
boolean
### getShowLoadingPosition() {#getShowLoadingPosition--}
```
public String getShowLoadingPosition()
```


Specifica la posizione sinistra, superiore (in px) per mostrare la finestra di dialogo di caricamento durante il postback al server, ecc. 100,200 indica che la posizione sinistra e superiore della finestra di dialogo di caricamento è a 100px,200px.

**Returns:**
java.lang.String
### getShowSaveButton() {#getShowSaveButton--}
```
public boolean getShowSaveButton()
```


Ottiene se mostrare il pulsante di salvataggio.

**Returns:**
boolean
### getShowSubmitButton() {#getShowSubmitButton--}
```
public boolean getShowSubmitButton()
```


Ottiene se mostrare il pulsante di invio.

**Returns:**
boolean
### getShowTabBar() {#getShowTabBar--}
```
public boolean getShowTabBar()
```


Ottiene se mostrare la barra delle schede.

**Returns:**
boolean
### getShowTabNavigation() {#getShowTabNavigation--}
```
public boolean getShowTabNavigation()
```


Ottiene se il pulsante di navigazione delle schede è mostrato, il valore predefinito è true.

**Returns:**
boolean
### getShowUndoButton() {#getShowUndoButton--}
```
public boolean getShowUndoButton()
```


Ottiene se mostrare il pulsante di annullamento.

**Returns:**
boolean
### getSpanWrap() {#getSpanWrap--}
```
public boolean getSpanWrap()
```


Specifica se avvolgere il contenuto nello span di cella, il valore predefinito è true.

**Returns:**
boolean
### getTabIndex() {#getTabIndex--}
```
public short getTabIndex()
```


Ottiene il TabIndex nel WebControl

**Returns:**
short
### getTabStyle() {#getTabStyle--}
```
public GridTableItemStyle getTabStyle()
```


Ottiene lo stile della barra delle schede.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getToolTip() {#getToolTip--}
```
public String getToolTip()
```


Ottiene il ToolTip nel WebControl

**Returns:**
java.lang.String
### getUseClientPageHeight() {#getUseClientPageHeight--}
```
public boolean getUseClientPageHeight()
```


Ottiene se GridWeb utilizza l'altezza della pagina client come altezza del controllo, adatto quando si imposta Height=\"100%\", il valore predefinito è false.

**Returns:**
boolean
### getViewPanelScrollLeft() {#getViewPanelScrollLeft--}
```
public String getViewPanelScrollLeft()
```


Ottiene la posizione della barra di scorrimento del pannello di visualizzazione della griglia.

**Returns:**
java.lang.String
### getViewPanelScrollTop() {#getViewPanelScrollTop--}
```
public String getViewPanelScrollTop()
```


Ottiene la posizione della barra di scorrimento del pannello di visualizzazione della griglia.

**Returns:**
java.lang.String
### getViewTableStyle() {#getViewTableStyle--}
```
public GridTableStyle getViewTableStyle()
```


Ottiene lo stile del pannello di visualizzazione dei dati.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


Ottiene la larghezza (System.Web.UI.WebControl.Unit) del controllo.

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


Ottiene la raccolta dei fogli di lavoro.

**Returns:**
[GridWorksheetCollection](../../com.aspose.gridweb/gridworksheetcollection)
### getXhtmlMode() {#getXhtmlMode--}
```
public boolean getXhtmlMode()
```


Ottiene se utilizzare lo stile XHTML, il valore predefinito è true.

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


Importa da un flusso di file Excel, inclusi flusso di file su disco o flusso di memoria.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.InputStream | Il flusso del file Excel, inclusi flusso da file su disco o flusso in memoria. |

### importExcelFile(InputStream stream, String passwordtoOpen) {#importExcelFile-java.io.InputStream-java.lang.String-}
```
public void importExcelFile(InputStream stream, String passwordtoOpen)
```


Importa da un flusso di file Excel, inclusi flusso di file su disco o flusso di memoria.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.InputStream | Il flusso del file Excel, inclusi flusso da file su disco o flusso in memoria. |
| passwordtoOpen | java.lang.String | la password di apertura per il file che è crittografato. |

### importExcelFile(String fileName) {#importExcelFile-java.lang.String-}
```
public void importExcelFile(String fileName)
```


Importa da un file Excel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Il nome del file Excel. |

### importExcelFile(String fileName, String passwordtoOpen) {#importExcelFile-java.lang.String-java.lang.String-}
```
public void importExcelFile(String fileName, String passwordtoOpen)
```


Importa da un file Excel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Il nome del file Excel. |
| passwordtoOpen | java.lang.String | la password di apertura per il file che è crittografato. |

### init() {#init--}
```
public void init()
```


il bean deve essere inizializzato dalla richiesta servlet e dalla risposta della pagina corrente

### isCalculateFormula() {#isCalculateFormula--}
```
public boolean isCalculateFormula()
```


Ottiene se calcolare la formula dopo le modifiche al valore della cella o dopo l'importazione del file. Il valore predefinito è true.

**Returns:**
boolean
### loadCSVFile(InputStream stream) {#loadCSVFile-java.io.InputStream-}
```
public void loadCSVFile(InputStream stream)
```


Carica i dati da un flusso di file CSV.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.InputStream | Il flusso del file. |

### loadCSVFile(String fileName) {#loadCSVFile-java.lang.String-}
```
public void loadCSVFile(String fileName)
```


Carica i dati da un file CSV.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Il nome del file. |

### loadHTMLFile(InputStream stream) {#loadHTMLFile-java.io.InputStream-}
```
public void loadHTMLFile(InputStream stream)
```


Carica i dati da un flusso di file HTML.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.InputStream | Il flusso del file. |

### loadHTMLFile(String fileName) {#loadHTMLFile-java.lang.String-}
```
public void loadHTMLFile(String fileName)
```


Carica i dati da un file HTML.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Il nome del file. |

### loadSpreadSheetMLFile(InputStream stream) {#loadSpreadSheetMLFile-java.io.InputStream-}
```
public void loadSpreadSheetMLFile(InputStream stream)
```


Carica i dati da un flusso di file SpreadSheetML.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.InputStream | Il flusso del file. |

### loadSpreadSheetMLFile(String fileName) {#loadSpreadSheetMLFile-java.lang.String-}
```
public void loadSpreadSheetMLFile(String fileName)
```


Carica i dati da un file SpreadSheetML.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Il nome del file. |

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


il metodo deve essere chiamato prima del rendering del bean GridWeb

### refreshChartShape() {#refreshChartShape--}
```
public void refreshChartShape()
```


Aggiorna tutte le immagini dei grafici per il foglio di lavoro attivo.

### saveCSVFile(OutputStream stream) {#saveCSVFile-java.io.OutputStream-}
```
public void saveCSVFile(OutputStream stream)
```


Salva i dati in un flusso di file CSV.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream | Il flusso del file. |

### saveCSVFile(String targetFile) {#saveCSVFile-java.lang.String-}
```
public void saveCSVFile(String targetFile)
```


Salva i dati in un file CSV.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| targetFile | java.lang.String | Il nome del file. |

### saveCustomStyleFile(String fileName) {#saveCustomStyleFile-java.lang.String-}
```
public void saveCustomStyleFile(String fileName)
```


Salva i dati di stile correnti del controllo in un file xml. Può essere usato per creare il tuo file di stile personalizzato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Il nome del file di stile. |

### saveHTMLFile(OutputStream stream) {#saveHTMLFile-java.io.OutputStream-}
```
public void saveHTMLFile(OutputStream stream)
```


Salva i dati in un flusso di file HTML.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream | Il flusso del file. |

### saveHTMLFile(String targetFile) {#saveHTMLFile-java.lang.String-}
```
public void saveHTMLFile(String targetFile)
```


Salva i dati in un file HTML.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| targetFile | java.lang.String | Il nome del file. |

### saveSpreadSheetMLFile(OutputStream stream) {#saveSpreadSheetMLFile-java.io.OutputStream-}
```
public void saveSpreadSheetMLFile(OutputStream stream)
```


Salva i dati in un flusso di file SpreadSheetML.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream | Il flusso del file. |

### saveSpreadSheetMLFile(String targetFile) {#saveSpreadSheetMLFile-java.lang.String-}
```
public void saveSpreadSheetMLFile(String targetFile)
```


Salva i dati in un file SpreadSheetML.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| targetFile | java.lang.String | Il nome del file. |

### saveToExcelFile(OutputStream stream) {#saveToExcelFile-java.io.OutputStream-}
```
public void saveToExcelFile(OutputStream stream)
```


Salva i fogli di lavoro in un file Excel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream | Il flusso su cui scrivere. |

### saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions) {#saveToExcelFile-java.io.OutputStream-com.aspose.gridweb.GridSaveOptions-}
```
public void saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions)
```


Salva i fogli di lavoro in un file Excel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream | Il flusso su cui scrivere. |
| saveOptions | [GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions) | Le opzioni di salvataggio. |

### saveToExcelFile(OutputStream stream, int format) {#saveToExcelFile-java.io.OutputStream-int-}
```
public void saveToExcelFile(OutputStream stream, int format)
```


Salva i fogli di lavoro in un file Excel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.OutputStream | Il flusso su cui scrivere. |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat). Il formato del file (Excel2003, Excel2007, CSV, SpreadsheetML) |

### saveToExcelFile(String targetFile) {#saveToExcelFile-java.lang.String-}
```
public void saveToExcelFile(String targetFile)
```


Salva i fogli di lavoro in un file Excel con formato Excel 2003.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| targetFile | java.lang.String | Il nome del file di destinazione su cui scrivere. |

### saveToExcelFile(String targetFile, GridSaveOptions saveOptions) {#saveToExcelFile-java.lang.String-com.aspose.gridweb.GridSaveOptions-}
```
public void saveToExcelFile(String targetFile, GridSaveOptions saveOptions)
```


Salva i fogli di lavoro in un file Excel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| targetFile | java.lang.String | Il nome del file di destinazione su cui scrivere. |
| saveOptions | [GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions) | Le opzioni di salvataggio. |

### saveToExcelFile(String targetFile, int format) {#saveToExcelFile-java.lang.String-int-}
```
public void saveToExcelFile(String targetFile, int format)
```


Salva i fogli di lavoro in un file Excel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| targetFile | java.lang.String | Il nome del file di destinazione su cui scrivere. |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat). Il formato del file (Excel2003, Excel2007, CSV, SpreadsheetML) |

### setACWClientPath(String value) {#setACWClientPath-java.lang.String-}
```
public void setACWClientPath(String value)
```


Imposta il percorso web dei file script/immagine del controllo. Per esempio: "http://localhost/acw\_client". È possibile impostare questo valore anche nel file web.config. Aggiungere questa sezione alla sezione `<configuration>`:
`<appSettings>`
`<add key=\"aspose.cells.gridweb.acw_client_path\" value=\"/acw_client/\" />`
`</appSettings>`


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setACWLanguageFileUrl(String value) {#setACWLanguageFileUrl-java.lang.String-}
```
public void setACWLanguageFileUrl(String value)
```


Imposta l'URL web del file di lingua del controllo. Per esempio: "/acw\_client/lang\_en.js".
Per impostazione predefinita, viene utilizzato un file inglese integrato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setActiveCell(GridCell value) {#setActiveCell-com.aspose.gridweb.GridCell-}
```
public void setActiveCell(GridCell value)
```


Imposta la cella attiva del foglio corrente. Modificato per essere scrivibile dalla versione 1.9.0.1.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [GridCell](../../com.aspose.gridweb/gridcell) |  |

### setActiveCellBgColor(Color value) {#setActiveCellBgColor-com.aspose.gridweb.Color-}
```
public void setActiveCellBgColor(Color value)
```


Specifica il colore di sfondo della cella attiva.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveCellColor(Color value) {#setActiveCellColor-com.aspose.gridweb.Color-}
```
public void setActiveCellColor(Color value)
```


Specifica il colore della cella attiva.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveHeaderBgColor(Color value) {#setActiveHeaderBgColor-com.aspose.gridweb.Color-}
```
public void setActiveHeaderBgColor(Color value)
```


Specifica il colore di sfondo dell'intestazione della riga/colonna attiva.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveHeaderColor(Color value) {#setActiveHeaderColor-com.aspose.gridweb.Color-}
```
public void setActiveHeaderColor(Color value)
```


Specifica il colore dell'intestazione della riga/colonna attiva.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


Imposta l'indice del foglio attivo. Uguale a WebWorksheets.ActiveSheetIndex.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setActiveTabStyle(GridTableItemStyle value) {#setActiveTabStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setActiveTabStyle(GridTableItemStyle value)
```


Specifica lo stile della scheda attiva.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setAutoRefreshChart(boolean value) {#setAutoRefreshChart-boolean-}
```
public void setAutoRefreshChart(boolean value)
```


Imposta se l'immagine del grafico viene aggiornata durante l'aggiornamento del valore della cella. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setBackColor(Color value) {#setBackColor-com.aspose.gridweb.Color-}
```
public void setBackColor(Color value)
```


Imposta il BackColor nel WebControl

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBeanID(String beanID) {#setBeanID-java.lang.String-}
```
public void setBeanID(String beanID)
```


imposta l'ID HTML del bean

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| beanID | java.lang.String |  |

### setBorderColor(Color value) {#setBorderColor-com.aspose.gridweb.Color-}
```
public void setBorderColor(Color value)
```


Imposta il BorderColor nel WebControl

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


Imposta il BorderStyle nel WebControl

Vedi [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setBorderWidth(Unit value) {#setBorderWidth-com.aspose.gridweb.Unit-}
```
public void setBorderWidth(Unit value)
```


Imposta la BorderWidth nel WebControl

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setBottomTableStyle(GridTableStyle value) {#setBottomTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setBottomTableStyle(GridTableStyle value)
```


Imposta lo stile della barra inferiore del controllo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


Imposta se calcolare la formula dopo le modifiche al valore della cella o dopo l'importazione del file. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCssClass(String value) {#setCssClass-java.lang.String-}
```
public void setCssClass(String value)
```


Imposta la CssClass nel WebControl

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCurrentPageIndex(int value) {#setCurrentPageIndex-int-}
```
public void setCurrentPageIndex(int value)
```


Imposta l'indice della pagina corrente in modalità paginazione.

**Remarks**

Quando è in modalità di paginazione, il controllo visualizzerà una volta PageSize righe di dati e mostrerà il controllo di selezione della pagina nella barra delle schede.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setCustomCalculationEngine(GridAbstractCalculationEngine value) {#setCustomCalculationEngine-com.aspose.gridweb.GridAbstractCalculationEngine-}
```
public void setCustomCalculationEngine(GridAbstractCalculationEngine value)
```


Rappresenta il motore di calcolo personalizzato dell'utente per estendere il motore di calcolo predefinito di Aspose.Cells.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [GridAbstractCalculationEngine](../../com.aspose.gridweb/gridabstractcalculationengine) |  |

### setCustomStyle(InputStream stream) {#setCustomStyle-java.io.InputStream-}
```
public void setCustomStyle(InputStream stream)
```


Imposta il file di stile personalizzato da un flusso, includendo flusso di file su disco o flusso di memoria.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.InputStream | Il flusso del file, inclusi flusso da disco o flusso in memoria. |

### setCustomStyleFileName(String value) {#setCustomStyleFileName-java.lang.String-}
```
public void setCustomStyleFileName(String value)
```


Imposta il nome del file di stile personalizzato.

**Remarks**

Il file di stile personalizzato è un file XML. Quando imposti il nome del file, il file verrà caricato immediatamente. Ecco il contenuto del "stile predefinito standard" ------------------------------------------------------- <Aspose.Cells.GridWeb.ViewerStyleTemplate runat="server" HeaderBarWidth="30pt" ScrollBarBaseColor="" FrameTableStyle-BorderStyle="Solid" FrameTableStyle-LeftBorderStyle-BorderWidth="" FrameTableStyle-LeftBorderStyle-BorderColor="" FrameTableStyle-RightBorderStyle-BorderWidth="" FrameTableStyle-RightBorderStyle-BorderColor="" FrameTableStyle-BorderWidth="1px" FrameTableStyle-CellSpacing="0" FrameTableStyle-BorderColor="Gray" FrameTableStyle-CellPadding="0" FrameTableStyle-TopBorderStyle-BorderWidth="" FrameTableStyle-TopBorderStyle-BorderColor="" FrameTableStyle-BottomBorderStyle-BorderWidth="" FrameTableStyle-BottomBorderStyle-BorderColor="" HeaderBarStyle-LeftBorderStyle-BorderStyle="Solid" HeaderBarStyle-LeftBorderStyle-BorderWidth="1px" HeaderBarStyle-LeftBorderStyle-BorderColor="White" HeaderBarStyle-VerticalAlign="Middle" HeaderBarStyle-RightBorderStyle-BorderStyle="Solid" HeaderBarStyle-RightBorderStyle-BorderWidth="1px" HeaderBarStyle-RightBorderStyle-BorderColor="Gray" HeaderBarStyle-BorderWidth="1px" HeaderBarStyle-Font-Size="10pt" HeaderBarStyle-BorderColor="Gray" HeaderBarStyle-BorderStyle="Solid" HeaderBarStyle-HorizontalAlign="Center" HeaderBarStyle-ForeColor="Black" HeaderBarStyle-TopBorderStyle-BorderStyle="Solid" HeaderBarStyle-TopBorderStyle-BorderWidth="1px" HeaderBarStyle-TopBorderStyle-BorderColor="White" HeaderBarStyle-BackColor="\#E0E0E0" HeaderBarStyle-BottomBorderStyle-BorderStyle="Solid" HeaderBarStyle-BottomBorderStyle-BorderWidth="1px" HeaderBarStyle-BottomBorderStyle-BorderColor="Gray" ViewTableStyle-LeftBorderStyle-BorderWidth="" ViewTableStyle-LeftBorderStyle-BorderColor="" ViewTableStyle-LayoutFixed="Fixed" ViewTableStyle-RightBorderStyle-BorderWidth="" ViewTableStyle-RightBorderStyle-BorderColor="" ViewTableStyle-BorderWidth="0px" ViewTableStyle-CellSpacing="0" ViewTableStyle-CellPadding="0" ViewTableStyle-TopBorderStyle-BorderWidth="" ViewTableStyle-TopBorderStyle-BorderColor="" ViewTableStyle-BottomBorderStyle-BorderWidth="" ViewTableStyle-BottomBorderStyle-BorderColor="" BottomTableStyle-LeftBorderStyle-BorderWidth="" BottomTableStyle-LeftBorderStyle-BorderColor="" BottomTableStyle-LayoutFixed="Fixed" BottomTableStyle-RightBorderStyle-BorderWidth="" BottomTableStyle-RightBorderStyle-BorderColor="" BottomTableStyle-BorderWidth="0px" BottomTableStyle-CellSpacing="0" BottomTableStyle-CellPadding="1" BottomTableStyle-TopBorderStyle-BorderStyle="Solid" BottomTableStyle-TopBorderStyle-BorderWidth="1px" BottomTableStyle-TopBorderStyle-BorderColor="Gray" BottomTableStyle-BottomBorderStyle-BorderWidth="" BottomTableStyle-BottomBorderStyle-BorderColor="" HeaderBarHeight="15pt" ActiveTabStyle-LeftBorderStyle-BorderWidth="" ActiveTabStyle-LeftBorderStyle-BorderColor="" ActiveTabStyle-RightBorderStyle-BorderWidth="" ActiveTabStyle-RightBorderStyle-BorderColor="" ActiveTabStyle-Height="15pt" ActiveTabStyle-BorderWidth="1px" ActiveTabStyle-Font-Size="10pt" ActiveTabStyle-BorderColor="Gray" ActiveTabStyle-ForeColor="Black" ActiveTabStyle-TopBorderStyle-BorderWidth="" ActiveTabStyle-TopBorderStyle-BorderColor="" ActiveTabStyle-BackColor="White" ActiveTabStyle-BottomBorderStyle-BorderWidth="" ActiveTabStyle-BottomBorderStyle-BorderColor="" HeaderBarTableStyle-LeftBorderStyle-BorderWidth="" HeaderBarTableStyle-LeftBorderStyle-BorderColor="" HeaderBarTableStyle-LayoutFixed="Fixed" HeaderBarTableStyle-RightBorderStyle-BorderWidth="" HeaderBarTableStyle-RightBorderStyle-BorderColor="" HeaderBarTableStyle-BorderWidth="0px" HeaderBarTableStyle-CellSpacing="0" HeaderBarTableStyle-BorderCollapse="Separate" HeaderBarTableStyle-CellPadding="0" HeaderBarTableStyle-TopBorderStyle-BorderWidth="" HeaderBarTableStyle-TopBorderStyle-BorderColor="" HeaderBarTableStyle-BottomBorderStyle-BorderWidth="" HeaderBarTableStyle-BottomBorderStyle-BorderColor="" TabStyle-LeftBorderStyle-BorderWidth="" TabStyle-LeftBorderStyle-BorderColor="" TabStyle-RightBorderStyle-BorderWidth="" TabStyle-RightBorderStyle-BorderColor="" TabStyle-Height="15pt" TabStyle-BorderWidth="1px" TabStyle-Font-Size="10pt" TabStyle-BorderColor="Gray" TabStyle-ForeColor="Black" TabStyle-TopBorderStyle-BorderWidth="" TabStyle-TopBorderStyle-BorderColor="" TabStyle-BackColor="\#E0E0E0" TabStyle-BottomBorderStyle-BorderWidth="" TabStyle-BottomBorderStyle-BorderColor="" ScrollBarArrowColor=""></Aspose.Cells.GridWeb.ViewerStyleTemplate>

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setDPI(double value) {#setDPI-double-}
```
public static void setDPI(double value)
```


Ottiene /Imposta il DPI della macchina.

**Remarks**

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Imposta il nome del carattere predefinito del controllo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setDefaultFontSize(FontUnit value) {#setDefaultFontSize-com.aspose.gridweb.FontUnit-}
```
public void setDefaultFontSize(FontUnit value)
```


Imposta la dimensione predefinita del carattere del controllo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [FontUnit](../../com.aspose.gridweb/fontunit) |  |

### setDefaultGridLineColor(Color value) {#setDefaultGridLineColor-com.aspose.gridweb.Color-}
```
public void setDefaultGridLineColor(Color value)
```


Imposta il colore predefinito della linea della griglia.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setDisplayCellTip(boolean value) {#setDisplayCellTip-boolean-}
```
public void setDisplayCellTip(boolean value)
```


Imposta se mostrare i suggerimenti. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEditMode(boolean value) {#setEditMode-boolean-}
```
public void setEditMode(boolean value)
```


Imposta la modalità di modifica del controllo.

**Remarks**

Quando impostato su true, le celle del controllo sono modificabili e le icone "save" e "undo" vengono visualizzate. Quando impostato su false, le celle del controllo sono di sola lettura e le icone "save" e "undo" non vengono visualizzate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEnableAJAX(boolean value) {#setEnableAJAX-boolean-}
```
public void setEnableAJAX(boolean value)
```


Imposta se utilizzare chiamate AJAX. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEnableAsync(boolean value) {#setEnableAsync-boolean-}
```
public void setEnableAsync(boolean value)
```


Imposta se caricare i dati delle celle in modo asincrono, consigliato per un foglio con più di 10000 celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEnableClientColumnOperations(boolean value) {#setEnableClientColumnOperations-boolean-}
```
public void setEnableClientColumnOperations(boolean value)
```


Imposta se abilitare le operazioni di colonna lato client.

**Remarks**

Quando impostato su true, l'utente può utilizzare il menu contestuale per aggiungere/rimuovere colonne.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEnableClientFreeze(boolean value) {#setEnableClientFreeze-boolean-}
```
public void setEnableClientFreeze(boolean value)
```


Imposta se abilitare le operazioni di congelamento lato client.

**Remarks**

Quando impostato su true, l'utente può utilizzare il menu contestuale per bloccare/sbloccare i riquadri.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEnableClientMergeOperations(boolean value) {#setEnableClientMergeOperations-boolean-}
```
public void setEnableClientMergeOperations(boolean value)
```


Imposta se abilitare le operazioni di unione lato client.

**Remarks**

Quando impostato su true, l'utente può utilizzare il menu contestuale per unire/separare le celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEnableClientResizeColumnRow(boolean value) {#setEnableClientResizeColumnRow-boolean-}
```
public void setEnableClientResizeColumnRow(boolean value)
```


Imposta se abilitare il ridimensionamento di colonne e righe lato client.

**Remarks**

Quando impostato su true, l'utente può ridimensionare la colonna e la riga sul lato client.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEnableClientRowOperations(boolean value) {#setEnableClientRowOperations-boolean-}
```
public void setEnableClientRowOperations(boolean value)
```


Imposta se abilitare le operazioni di riga lato client.

**Remarks**

Quando impostato su true, l'utente può utilizzare il menu contestuale per aggiungere/rimuovere righe.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEnableDoubleClickEvent(boolean value) {#setEnableDoubleClickEvent-boolean-}
```
public void setEnableDoubleClickEvent(boolean value)
```


Imposta se abilitare l'evento di doppio clic lato cliente.

**Remarks**

Quando impostato su true, il controllo riceverà gli eventi di doppio clic dal lato client e potrai gestire questi eventi sul lato server. Altrimenti il controllo ignorerà tutti gli eventi di doppio clic.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEnableMetalLightEffect(boolean value) {#setEnableMetalLightEffect-boolean-}
```
public void setEnableMetalLightEffect(boolean value)
```


Imposta se applicare l'effetto luce metallica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEnablePaging(boolean value) {#setEnablePaging-boolean-}
```
public void setEnablePaging(boolean value)
```


Imposta se abilitare la modalità di paginazione del controllo.

**Remarks**

Quando impostato su true, il controllo visualizzerà una volta PageSize righe di dati e mostrerà il controllo di selezione pagina nella barra delle schede.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEnableStyleDialogbox(boolean value) {#setEnableStyleDialogbox-boolean-}
```
public void setEnableStyleDialogbox(boolean value)
```


Imposta se abilitare la finestra di dialogo di stile lato client.

**Remarks**

Quando impostato su true, l'utente può utilizzare la finestra di dialogo stile per impostare lo stile di una cella selezionando "Format Cell..." dal menu a comparsa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


Imposta l'Enabled nel WebControl

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFilteredPaging(boolean value) {#setFilteredPaging-boolean-}
```
public void setFilteredPaging(boolean value)
```


Imposta se abilitare la paginazione dopo il filtraggio dei dati; avrà effetto quando EnablePaging è true.

**Remarks**

Quando impostato su true, il controllo paginerà in base ai dati filtrati; il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setForceValidation(boolean value) {#setForceValidation-boolean-}
```
public void setForceValidation(boolean value)
```


Imposta se forzare la convalida lato cliente.

**Remarks**

Quando impostato su true, i dati non verranno inviati al server finché tutti i campi di input non saranno validi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setForeColor(Color value) {#setForeColor-com.aspose.gridweb.Color-}
```
public void setForeColor(Color value)
```


Imposta il ForeColor nel WebControl

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setFrameTableStyle(GridTableStyle value) {#setFrameTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setFrameTableStyle(GridTableStyle value)
```


Imposta lo stile del frame del controllo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setGoonDefaultSaveOperation(boolean value) {#setGoonDefaultSaveOperation-boolean-}
```
public void setGoonDefaultSaveOperation(boolean value)
```


Imposta se GridWeb eseguirà l'operazione di salvataggio predefinita; il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHeaderBarHeight(Unit value) {#setHeaderBarHeight-com.aspose.gridweb.Unit-}
```
public void setHeaderBarHeight(Unit value)
```


Imposta l'altezza (System.Web.UI.WebControl.Unit) della barra intestazione superiore del controllo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHeaderBarStyle(GridTableItemStyle value) {#setHeaderBarStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setHeaderBarStyle(GridTableItemStyle value)
```


Imposta lo stile della barra intestazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setHeaderBarTableStyle(GridTableStyle value) {#setHeaderBarTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setHeaderBarTableStyle(GridTableStyle value)
```


Imposta lo stile della barra intestazione del controllo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setHeaderBarWidth(Unit value) {#setHeaderBarWidth-com.aspose.gridweb.Unit-}
```
public void setHeaderBarWidth(Unit value)
```


Imposta la larghezza (System.Web.UI.WebControl.Unit) della barra intestazione sinistra del controllo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHeight(Unit value) {#setHeight-com.aspose.gridweb.Unit-}
```
public void setHeight(Unit value)
```


Imposta l'altezza (System.Web.UI.WebControl.Unit) del controllo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setIgnoreStyleWithNoData(boolean value) {#setIgnoreStyleWithNoData-boolean-}
```
public void setIgnoreStyleWithNoData(boolean value)
```


Imposta se GridWeb ignora la visualizzazione di righe o colonne che non contengono valori di cella ma sono comunque formattate. Se impostato su true, le prestazioni saranno migliori. Il valore predefinito è false, il che significa che se l'ultima riga/colonna consecutiva non ha valori di cella ma è formattata, verrà comunque mostrata. Questa opzione è valida solo quando EnableAsync è false. Questa opzione non ha effetto quando EnableAsync è true, il che significa che GridWeb mostrerà tutte le righe/colonne con stile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setLoadOptions(GridLoadOptions value) {#setLoadOptions-com.aspose.gridweb.GridLoadOptions-}
```
public void setLoadOptions(GridLoadOptions value)
```


Rappresenta le opzioni di caricamento per GridWeb.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [GridLoadOptions](../../com.aspose.gridweb/gridloadoptions) |  |

### setMaxColumn(int value) {#setMaxColumn-int-}
```
public void setMaxColumn(int value)
```


Imposta l'indice massimo di colonna da visualizzare (basato su zero) del foglio web. Il controllo utilizza il valore più grande tra MaxColumn e la colonna massima dei dati del foglio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMaxRow(int value) {#setMaxRow-int-}
```
public void setMaxRow(int value)
```


Imposta l'indice massimo di riga da visualizzare (basato su zero) del foglio web. Il controllo utilizza il valore più grande tra MaxRow e la riga massima dei dati del foglio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMessage(String value) {#setMessage-java.lang.String-}
```
public void setMessage(String value)
```


Imposta il messaggio per la griglia.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setMinColumn(int value) {#setMinColumn-int-}
```
public void setMinColumn(int value)
```


Imposta l'indice minimo di colonna da visualizzare (basato su zero) del foglio web. Il controllo utilizza il valore più piccolo tra MinColumn e la colonna minima dei dati del foglio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMinRow(int value) {#setMinRow-int-}
```
public void setMinRow(int value)
```


Imposta l'indice minimo di riga da visualizzare (basato su zero) del foglio web. Il controllo utilizza il valore più piccolo tra MinRow e la riga minima dei dati del foglio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setNeedRenderGroupRows(boolean value) {#setNeedRenderGroupRows-boolean-}
```
public void setNeedRenderGroupRows(boolean value)
```


Imposta se mostrare le righe di gruppo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setNoHScroll(boolean value) {#setNoHScroll-boolean-}
```
public void setNoHScroll(boolean value)
```


Imposta un valore che indica se la barra di scorrimento orizzontale è nascosta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setNoScroll(boolean value) {#setNoScroll-boolean-}
```
public void setNoScroll(boolean value)
```


Imposta se mostrare la barra di scorrimento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setNoVScroll(boolean value) {#setNoVScroll-boolean-}
```
public void setNoVScroll(boolean value)
```


Imposta un valore che indica se la barra di scorrimento verticale è nascosta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setOnAjaxCallFinishedClientFunction(String value) {#setOnAjaxCallFinishedClientFunction-java.lang.String-}
```
public void setOnAjaxCallFinishedClientFunction(String value)
```


Imposta il nome della funzione lato client da chiamare quando ajaxcall è terminato. La funzione client dovrebbe essere dichiarata così:
function GridAjaxcallFinished()
\{
alert(this.id+" ajaxcall finished ");
\}

Nota: è possibile utilizzare il puntatore "this" nella funzione client per fare riferimento al controllo grid che genera l'evento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setOnCellErrorClientFunction(String value) {#setOnCellErrorClientFunction-java.lang.String-}
```
public void setOnCellErrorClientFunction(String value)
```


Imposta il nome della funzione lato client da chiamare quando la convalida di una cella fallisce. La funzione client dovrebbe essere dichiarata così:
function MyOnCellError(cell)
\{
alert(this.getCellValueByCell(cell));
\}

Nota: è possibile utilizzare il puntatore "this" nella funzione client per fare riferimento al controllo grid che genera l'evento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setOnCellSelectedAjaxCallBackClientFunction(String value) {#setOnCellSelectedAjaxCallBackClientFunction-java.lang.String-}
```
public void setOnCellSelectedAjaxCallBackClientFunction(String value)
```


Imposta la funzione lato client da chiamare quando una cella è selezionata. La funzione client dovrebbe essere dichiarata così:
function MyOnSelectCellAjaxCallBack(cell,customerdata)
\{

\}

Nota: è possibile utilizzare il puntatore "this" nella funzione client per fare riferimento al controllo grid che genera l'evento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setOnCellSelectedClientFunction(String value) {#setOnCellSelectedClientFunction-java.lang.String-}
```
public void setOnCellSelectedClientFunction(String value)
```


Imposta la funzione lato client da chiamare quando una cella è selezionata. La funzione client dovrebbe essere dichiarata così:
function MyOnSelectCell(cell)
\{
GridWeb1.setCellValueByCell(cell, "test");
\}

Nota: è possibile utilizzare il puntatore "this" nella funzione client per fare riferimento al controllo grid che genera l'evento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setOnCellUnselectedClientFunction(String value) {#setOnCellUnselectedClientFunction-java.lang.String-}
```
public void setOnCellUnselectedClientFunction(String value)
```


Imposta la funzione lato client da chiamare quando una cella è deselezionata. La funzione client dovrebbe essere dichiarata così:
function MyOnUnselectCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

Nota: è possibile utilizzare il puntatore "this" nella funzione client per fare riferimento al controllo grid che genera l'evento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setOnCellUpdatedClientFunction(String value) {#setOnCellUpdatedClientFunction-java.lang.String-}
```
public void setOnCellUpdatedClientFunction(String value)
```


Imposta il nome della funzione lato client da chiamare quando il valore di una cella viene aggiornato. La funzione client dovrebbe essere dichiarata così:
function MyOnCellUpdated(cell)
\{
alert(this.getCellValueByCell(cell));
\}

Nota: è possibile utilizzare il puntatore "this" nella funzione client per fare riferimento al controllo grid che genera l'evento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setOnContextMenuShowClientFunction(String value) {#setOnContextMenuShowClientFunction-java.lang.String-}
```
public void setOnContextMenuShowClientFunction(String value)
```


Imposta la funzione lato client da chiamare quando il menu contestuale verrà mostrato. La funzione client dovrebbe essere dichiarata così:
function onContextMenuShow()
\{
var menu = event.srcElement;
menu.setItemVisibility("Delete", "block");
menu.setItemVisibility("Update", "none");
\}

Nota: è possibile utilizzare il puntatore "this" nella funzione client per fare riferimento al controllo grid che genera l'evento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setOnDoubleClickCellClientFunction(String value) {#setOnDoubleClickCellClientFunction-java.lang.String-}
```
public void setOnDoubleClickCellClientFunction(String value)
```


Imposta la funzione lato client da chiamare quando una cella viene doppio cliccata. La funzione client dovrebbe essere dichiarata così:
function MyOnDoubleClickCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

Nota: è possibile utilizzare il puntatore "this" nella funzione client per fare riferimento al controllo grid che genera l'evento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setOnDoubleClickRowClientFunction(String value) {#setOnDoubleClickRowClientFunction-java.lang.String-}
```
public void setOnDoubleClickRowClientFunction(String value)
```


Imposta la funzione lato client da chiamare quando una riga viene doppio cliccata. La funzione client dovrebbe essere dichiarata così:
function MyOnRowDoubleClick(row)
\{
alert(row);
\}

Nota: è possibile utilizzare il puntatore "this" nella funzione client per fare riferimento al controllo grid che genera l'evento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setOnGridInitClientFunction(String value) {#setOnGridInitClientFunction-java.lang.String-}
```
public void setOnGridInitClientFunction(String value)
```


Imposta il nome della funzione lato client da chiamare quando la griglia è inizializzata. La funzione client dovrebbe essere dichiarata così:
function MyOnGridInit(grid)
\{
alert("La griglia è inizializzata: " + grid.id);
\}

Nota: è possibile utilizzare il puntatore "this" nella funzione client per fare riferimento al controllo grid che genera l'evento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setOnPageChangeClientFunction(String value) {#setOnPageChangeClientFunction-java.lang.String-}
```
public void setOnPageChangeClientFunction(String value)
```


Imposta la funzione lato client da chiamare dopo la modifica dell'indice di pagina. Ha effetto solo quando EnablePaging è true. La funzione client dovrebbe essere dichiarata così:
function MyOnPageChange(index)
\{
console.log("la pagina corrente è:"+index);
\}

Nota: è possibile utilizzare il puntatore "this" nella funzione client per fare riferimento al controllo grid che genera l'evento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setOnPageSubmitClientFunction(String value) {#setOnPageSubmitClientFunction-java.lang.String-}
```
public void setOnPageSubmitClientFunction(String value)
```


Imposta la funzione client da chiamare prima che la pagina venga inviata lato client.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setOnShapeSelectedClientFunction(String value) {#setOnShapeSelectedClientFunction-java.lang.String-}
```
public void setOnShapeSelectedClientFunction(String value)
```


Imposta la funzione lato client da chiamare quando una forma è selezionata. La funzione client dovrebbe essere dichiarata così:
function MyOnSelectShape(shape)
\{
var name=shape.getAttribute("namevalue")
var text=shape.getAttribute("textvalue")
var value=shape.getAttribute("controlvalue")
var type=shape.getAttribute("msotype")
\}

Nota: è possibile utilizzare il puntatore "this" nella funzione client per fare riferimento al controllo grid che genera l'evento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setOnSubmitClientFunction(String value) {#setOnSubmitClientFunction-java.lang.String-}
```
public void setOnSubmitClientFunction(String value)
```


Imposta la funzione client da chiamare prima che il controllo venga inviato lato client. La funzione client dovrebbe essere dichiarata così:
function MyOnSubmit(arg, cancelEdit)
\{
return true;
\}
L'arg è l'argomento di invio, contiene il comando da inviare al server. Il cancelEdit è un valore booleano che indica se il controllo ha scartato l'input dell'utente prima dell'invio. Il controllo continuerà a inviare se la funzione restituisce true.
Nota: è possibile utilizzare il puntatore "this" nella funzione client per fare riferimento al controllo grid che genera l'evento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


Imposta se adattare solo le righe la cui altezza non è personalizzata; il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPageSize(int value) {#setPageSize-int-}
```
public void setPageSize(int value)
```


Imposta la dimensione della pagina in modalità paginazione.

**Remarks**

Quando è in modalità di paginazione, il controllo visualizzerà una volta PageSize righe di dati e mostrerà il controllo di selezione della pagina nella barra delle schede.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPictureCachePath(String value) {#setPictureCachePath-java.lang.String-}
```
public static void setPictureCachePath(String value)
```


Imposta il percorso di archiviazione delle immagini per la cartella di lavoro; tutte le forme e le immagini saranno memorizzate in questa directory. Il percorso predefinito è acwcache nella directory base dell'applicazione corrente. Gli utenti devono implementare un servizio di pianificazione per pulire i file scaduti dalla sessione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setPresetStyle(int value) {#setPresetStyle-int-}
```
public void setPresetStyle(int value)
```


Imposta lo stile predefinito.

Vedi [PresetStyle](../../com.aspose.gridweb/presetstyle).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setRefreshValidation(boolean value) {#setRefreshValidation-boolean-}
```
public void setRefreshValidation(boolean value)
```


Imposta se aggiornare il valore di convalida dopo le modifiche al valore della cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRenderHiddenRow(boolean value) {#setRenderHiddenRow-boolean-}
```
public void setRenderHiddenRow(boolean value)
```


Imposta se la riga nascosta viene renderizzata in GridControl, il valore predefinito è false. Se è necessario rendere visibile la riga nascosta in seguito, impostarla su true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRowHeightForCSV(double value) {#setRowHeightForCSV-double-}
```
public void setRowHeightForCSV(double value)
```


Imposta il valore dell'altezza della riga in punti per il file CSV; il valore predefinito è 14,5.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setScrollBarArrowColor(Color value) {#setScrollBarArrowColor-com.aspose.gridweb.Color-}
```
public void setScrollBarArrowColor(Color value)
```


Specifica il colore del pulsante freccia della barra di scorrimento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setScrollBarBaseColor(Color value) {#setScrollBarBaseColor-com.aspose.gridweb.Color-}
```
public void setScrollBarBaseColor(Color value)
```


Specifica il colore della barra di scorrimento del controllo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSelectCellBgColor(Color value) {#setSelectCellBgColor-com.aspose.gridweb.Color-}
```
public void setSelectCellBgColor(Color value)
```


Specifica il colore di sfondo delle celle selezionate nell'intervallo di selezione multipla.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSelectCellColor(Color value) {#setSelectCellColor-com.aspose.gridweb.Color-}
```
public void setSelectCellColor(Color value)
```


Specifica il colore delle celle selezionate nell'intervallo di selezione multipla.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSessionStorePath(String value) {#setSessionStorePath-java.lang.String-}
```
public void setSessionStorePath(String value)
```


Imposta il percorso di memorizzazione della cache di sessione quando la modalità sessione è File o ViewState, ecc.: gridweb.SessionStorePath=\"c:/mytempdir/session\"; in tal caso i dati di sessione saranno memorizzati in c:/mytempdir/session.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridweb.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


Rappresenta le impostazioni della cartella di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridweb/gridworkbooksettings) |  |

### setShowAddButton(boolean value) {#setShowAddButton-boolean-}
```
public void setShowAddButton(boolean value)
```


Imposta se mostrare il pulsante per aggiungere un foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowBottomBar(boolean value) {#setShowBottomBar-boolean-}
```
public void setShowBottomBar(boolean value)
```


Specifica se mostrare la barra dei comandi (include barra dei comandi e barra delle schede) nella parte inferiore del controllo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowCellEditBox(boolean value) {#setShowCellEditBox-boolean-}
```
public void setShowCellEditBox(boolean value)
```


Indica se Gridweb mostra la barra degli strumenti della casella di modifica come in MS-EXCEL. Se abilitata, una casella di modifica per la cella corrente verrà visualizzata in Gridweb. Se attiviamo questa funzionalità, è necessario importare la libreria jquery js nei tuoi file aspx per supportare la nuova funzionalità. Qualsiasi versione recente di jquery va bene, ecc.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowCommandBarAtTop(boolean value) {#setShowCommandBarAtTop-boolean-}
```
public void setShowCommandBarAtTop(boolean value)
```


Specifica se mostrare la barra dei comandi (include barra dei comandi e barra delle schede) nella parte superiore del controllo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowContextMenu(boolean value) {#setShowContextMenu-boolean-}
```
public void setShowContextMenu(boolean value)
```


Imposta se mostrare il menu contestuale. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowDefaultGridLine(boolean value) {#setShowDefaultGridLine-boolean-}
```
public void setShowDefaultGridLine(boolean value)
```


Imposta se mostrare le linee di griglia predefinite delle celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowHeaderBar(boolean value) {#setShowHeaderBar-boolean-}
```
public void setShowHeaderBar(boolean value)
```


Imposta se mostrare la barra dell'intestazione

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowLoading(boolean value) {#setShowLoading-boolean-}
```
public void setShowLoading(boolean value)
```


Specifica se mostrare una finestra di dialogo di caricamento durante il postback al server.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowLoadingPosition(String value) {#setShowLoadingPosition-java.lang.String-}
```
public void setShowLoadingPosition(String value)
```


Specifica la posizione sinistra, superiore (in px) per mostrare la finestra di dialogo di caricamento durante il postback al server, ecc. 100,200 indica che la posizione sinistra e superiore della finestra di dialogo di caricamento è a 100px,200px.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setShowSaveButton(boolean value) {#setShowSaveButton-boolean-}
```
public void setShowSaveButton(boolean value)
```


Imposta se mostrare il pulsante di salvataggio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowSubmitButton(boolean value) {#setShowSubmitButton-boolean-}
```
public void setShowSubmitButton(boolean value)
```


Imposta se mostrare il pulsante di invio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowTabBar(boolean value) {#setShowTabBar-boolean-}
```
public void setShowTabBar(boolean value)
```


Imposta se mostrare la barra delle schede.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowTabNavigation(boolean value) {#setShowTabNavigation-boolean-}
```
public void setShowTabNavigation(boolean value)
```


Imposta se il pulsante di navigazione delle schede è mostrato, il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowUndoButton(boolean value) {#setShowUndoButton-boolean-}
```
public void setShowUndoButton(boolean value)
```


Imposta se mostrare il pulsante di annullamento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSpanWrap(boolean value) {#setSpanWrap-boolean-}
```
public void setSpanWrap(boolean value)
```


Specifica se avvolgere il contenuto nello span di cella, il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setTabIndex(short value) {#setTabIndex-short-}
```
public void setTabIndex(short value)
```


Imposta il TabIndex nel WebControl

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | short |  |

### setTabStyle(GridTableItemStyle value) {#setTabStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setTabStyle(GridTableItemStyle value)
```


Imposta lo stile della barra delle schede.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setToolTip(String value) {#setToolTip-java.lang.String-}
```
public void setToolTip(String value)
```


Imposta il ToolTip nel WebControl

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setUseClientPageHeight(boolean value) {#setUseClientPageHeight-boolean-}
```
public void setUseClientPageHeight(boolean value)
```


Imposta se gridweb utilizza l'altezza della pagina client come altezza del controllo, adatto quando si imposta Height=\"100%\", il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setViewPanelScrollLeft(String value) {#setViewPanelScrollLeft-java.lang.String-}
```
public void setViewPanelScrollLeft(String value)
```


Imposta la posizione della barra di scorrimento del pannello di visualizzazione della griglia.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setViewPanelScrollTop(String value) {#setViewPanelScrollTop-java.lang.String-}
```
public void setViewPanelScrollTop(String value)
```


Imposta la posizione della barra di scorrimento del pannello di visualizzazione della griglia.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setViewTableStyle(GridTableStyle value) {#setViewTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setViewTableStyle(GridTableStyle value)
```


Imposta lo stile del pannello di visualizzazione dei dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


Imposta la larghezza (System.Web.UI.WebControl.Unit) del controllo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setXhtmlMode(boolean value) {#setXhtmlMode-boolean-}
```
public void setXhtmlMode(boolean value)
```


Imposta se utilizzare lo stile XHTML, il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

