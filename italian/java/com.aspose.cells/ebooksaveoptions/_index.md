---
title: "EbookSaveOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le opzioni per il salvataggio del file ebook."
type: docs
url: /it/java/com.aspose.cells/ebooksaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions), [com.aspose.cells.HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions)
```
public class EbookSaveOptions extends HtmlSaveOptions
```

Rappresenta le opzioni per il salvataggio del file ebook.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [EbookSaveOptions()](#EbookSaveOptions--) | Crea le opzioni per salvare il file ebook. |
| [EbookSaveOptions(int saveFormat)](#EbookSaveOptions-int-) | Crea le opzioni per salvare il file ebook. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddGenericFont()](#getAddGenericFont--) | Indica se aggiungere un font generico alla proprietà CSS font-family. |
| [getAddTooltipText()](#getAddTooltipText--) | Indica se aggiungere il testo del tooltip quando i dati non possono essere visualizzati completamente. |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | La directory in cui verranno salvati i file allegati. |
| [getAttachedFilesUrlPrefix()](#getAttachedFilesUrlPrefix--) | Specifica il prefisso Url dei file allegati, come le immagini, nel file html. |
| [getCachedFileFolder()](#getCachedFileFolder--) | La cartella per i file temporanei che possono essere usati come cache dei dati. |
| [getCalculateFormula()](#getCalculateFormula--) | Indica se calcolare le formule prima di salvare il file html. |
| [getCellCssPrefix()](#getCellCssPrefix--) | Ottiene il prefisso del nome css, il valore predefinito è "". |
| [getCellNameAttribute()](#getCellNameAttribute--) | Specifica l'attributo che indica il CellName da scrivere. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Indica se verificare le restrizioni del file Excel quando l'utente modifica gli oggetti correlati alle celle. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Rendi il workbook vuoto dopo aver salvato il file. |
| [getCreateDirectory()](#getCreateDirectory--) | Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. |
| [getCssStyles()](#getCssStyles--) | Ottiene gli stili css aggiuntivi per il formattatore. |
| [getDataBarRenderMode()](#getDataBarRenderMode--) | Rappresenta la modalità di rendering di DataBar durante la conversione dei file Excel in file html. |
| [getDefaultFontName()](#getDefaultFontName--) | Specifica il nome del font predefinito per l'esportazione html; il font predefinito verrà usato quando il font dello stile non esiste. Se questa proprietà è null, Aspose.Cells utilizzerà un font universale che ha la stessa famiglia del font originale; il valore predefinito è null. |
| [getDisableCss()](#getDisableCss--) | Indica se applicare solo stili inline, senza fare affidamento su CSS. |
| [getDisableDownlevelRevealedComments()](#getDisableDownlevelRevealedComments--) | Indica se disabilitare i commenti condizionali Downlevel-revealed durante l'esportazione del file in html; il valore predefinito è false. |
| [getEmbeddedFontType()](#getEmbeddedFontType--) | Ottiene il tipo di incorporamento del file font nel file html. |
| [getEnableCssCustomProperties()](#getEnableCssCustomProperties--) | Ottimizza l'output html utilizzando le proprietà personalizzate CSS. |
| [getEncodeEntityAsCode()](#getEncodeEntityAsCode--) | Indica se le entità dei caratteri html vengono sostituite con il codice decimale. |
| [getEncoding()](#getEncoding--) | Se non impostato, utilizza Encoding.UTF8 come tipo di codifica predefinito. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indica se crittografare le proprietà del documento quando si salva come file .xls. |
| [getExcludeUnusedStyles()](#getExcludeUnusedStyles--) | Indica se escludere gli stili non utilizzati. |
| [getExportActiveWorksheetOnly()](#getExportActiveWorksheetOnly--) | Indica se esportare solo il foglio di lavoro attivo in un file html. |
| [getExportArea()](#getExportArea--) | Ottiene l'area CellArea da esportare del foglio di lavoro attivo corrente. |
| [getExportBogusRowData()](#getExportBogusRowData--) | Indica se esportare dati di riga inferiore falsi. |
| [getExportCellCoordinate()](#getExportCellCoordinate--) | Indica se esportare le coordinate Excel delle celle non vuote durante il salvataggio del file in html. |
| [getExportCommentsType()](#getExportCommentsType--) | Rappresenta il tipo di esportazione dei commenti nei file html. |
| [getExportDataOptions()](#getExportDataOptions--) | Indica la regola di esportazione dei dati del file html. Il valore predefinito è All. |
| [getExportDocumentProperties()](#getExportDocumentProperties--) | Indica se esportare le proprietà del documento. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito. |
| [getExportExtraHeadings()](#getExportExtraHeadings--) | Indica se esportare intestazioni extra quando la lunghezza del testo supera la colonna di visualizzazione massima. |
| [getExportFormula()](#getExportFormula--) | Indica se esportare le formule durante il salvataggio del file in html. |
| [getExportFrameScriptsAndProperties()](#getExportFrameScriptsAndProperties--) | Indicazione se esportare script di frame e proprietà del documento. |
| [getExportGridLines()](#getExportGridLines--) | Indicazione se esportare le linee della griglia. Il valore predefinito è false. |
| [getExportHeadings()](#getExportHeadings--) | Indica se esportare le intestazioni di righe e colonne del foglio durante il salvataggio in file HTML. |
| [getExportHiddenWorksheet()](#getExportHiddenWorksheet--) | Indicazione se esportare il contenuto del foglio di lavoro nascosto. Il valore predefinito è true. |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--) | Specifica se le immagini vengono salvate in formato Base64 in HTML, MHTML o EPUB. |
| [getExportNamedRangeAnchors()](#getExportNamedRangeAnchors--) | Indica se esportare gli elementi di ancoraggio per gli intervalli denominati durante il salvataggio come HTML. |
| [getExportObjectListener()](#getExportObjectListener--) | Ottiene l'ExportObjectListener per l'esportazione degli oggetti. |
| [getExportPageFooters()](#getExportPageFooters--) | Indica se esportare le intestazioni di pagina. |
| [getExportPageHeaders()](#getExportPageHeaders--) | Indica se esportare le intestazioni di pagina. |
| [getExportPrintAreaOnly()](#getExportPrintAreaOnly--) | Indica se esportare solo l'area di stampa nel file HTML. |
| [getExportRowColumnHeadings()](#getExportRowColumnHeadings--) | Indica se esportare le intestazioni di righe e colonne del foglio durante il salvataggio in file HTML. |
| [getExportSimilarBorderStyle()](#getExportSimilarBorderStyle--) | Indicazione se esportare lo stile di bordo simile quando lo stile di bordo non è supportato dai browser. |
| [getExportSingleTab()](#getExportSingleTab--) | Indica se esportare la singola scheda quando il file contiene un solo foglio di lavoro. |
| [getExportWorkbookProperties()](#getExportWorkbookProperties--) | Indicazione se esportare le proprietà della cartella di lavoro. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito. |
| [getExportWorksheetCSSSeparately()](#getExportWorksheetCSSSeparately--) | Indicazione se esportare il CSS del foglio di lavoro separatamente. Il valore predefinito è false. |
| [getExportWorksheetProperties()](#getExportWorksheetProperties--) | Indicazione se esportare le proprietà del foglio di lavoro. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito. |
| [getFilePathProvider()](#getFilePathProvider--) | Ottiene l'IFilePathProvider per esportare il Worksheet in HTML separatamente. |
| [getFormatDataIgnoreColumnWidth()](#getFormatDataIgnoreColumnWidth--) | Indicazione se mostrare tutti i dati formattati della cella quando supera la colonna. |
| [getHiddenColDisplayType()](#getHiddenColDisplayType--) | Colonna nascosta (la larghezza di questa colonna è 0) in Excel, prima di salvarla in formato HTML, se HtmlHiddenColDisplayType è "Remove", la colonna nascosta non verrà emessa; se il valore è "Hidden", la colonna verrà emessa ma sarà nascosta; il valore predefinito è "Hidden". |
| [getHiddenRowDisplayType()](#getHiddenRowDisplayType--) | Riga nascosta (l'altezza di questa riga è 0) in Excel, prima di salvarla in formato HTML, se HtmlHiddenRowDisplayType è "Remove", la riga nascosta non verrà emessa; se il valore è "Hidden", la riga verrà emessa ma sarà nascosta; il valore predefinito è "Hidden". |
| [getHideOverflowWrappedText()](#getHideOverflowWrappedText--) | Indica se nascondere il testo in overflow quando il formato della cella è impostato per andare a capo. |
| [getHtmlCrossStringType()](#getHtmlCrossStringType--) | Indica se una stringa che attraversa più celle verrà visualizzata nello stesso modo di MS Excel durante il salvataggio di un file Excel in formato HTML. |
| [getHtmlVersion()](#getHtmlVersion--) | Specifica la versione dello standard HTML da utilizzare durante il salvataggio nel formato HTML. |
| [getIgnoreInvisibleShapes()](#getIgnoreInvisibleShapes--) | Indica se esportare le forme non visibili |
| [getImageOptions()](#getImageOptions--) | Ottieni l'oggetto ImageOrPrintOptions prima dell'esportazione |
| [getImageScalable()](#getImageScalable--) | Indica se utilizzare unità scalabili per descrivere la larghezza dell'immagine quando si utilizzano unità scalabili per descrivere la larghezza della colonna. |
| [getLayoutMode()](#getLayoutMode--) | Ottiene la modalità di layout durante il salvataggio in HTML. |
| [getLinkTargetType()](#getLinkTargetType--) | Indicazione del tipo di attributo target nel link `<a>`. |
| [getMergeAreas()](#getMergeAreas--) | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. |
| [getMergeEmptyTdForcely()](#getMergeEmptyTdForcely--) | Indica se unire forzatamente gli elementi TD vuoti durante l'esportazione del file in HTML. |
| [getMergeEmptyTdType()](#getMergeEmptyTdType--) | L'opzione per unire celle vuote contigue (elementi td vuoti). Il valore predefinito è MergeEmptyTdType.Default. |
| [getOfficeMathOutputMode()](#getOfficeMathOutputMode--) | Indica come gli oggetti OfficeMath vengono esportati in HTML. Il valore predefinito è Image. |
| [getPageTitle()](#getPageTitle--) | Il titolo della pagina HTML. |
| [getParseHtmlTagInCell()](#getParseHtmlTagInCell--) | Indica se il tag HTML (come `<div></div>`) nella cella deve essere analizzato come valore della cella o preservato così com'è. |
| [getPresentationPreference()](#getPresentationPreference--) | Indicazione se il file HTML o MHT è la preferenza di presentazione. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indica se memorizzare nella cache i dati più recenti del grafico. |
| [getSaveAsSingleFile()](#getSaveAsSingleFile--) | Indica se salvare l'HTML come file unico. |
| [getSaveFormat()](#getSaveFormat--) | Ottiene il formato di salvataggio del file. |
| [getSheetSet()](#getSheetSet--) | Ottiene i fogli da renderizzare. |
| [getShowAllSheets()](#getShowAllSheets--) | Indica se mostrare tutti i fogli quando si salva come file HTML unico. |
| [getSortExternalNames()](#getSortExternalNames--) | Indica se ordinare i nomi definiti esterni prima di salvare il file. |
| [getSortNames()](#getSortNames--) | Indica se ordinare i nomi definiti prima di salvare il file. |
| [getSpaceMode()](#getSpaceMode--) | Indica come gli spazi vengono renderizzati nell'output HTML. |
| [getStreamProvider()](#getStreamProvider--) | Ottiene l'IStreamProvider per l'esportazione degli oggetti. |
| [getTableCssId()](#getTableCssId--) | Ottiene il prefisso del nome CSS di tipo, come tr, col, td e così via; sono contenuti nell'elemento table che ha l'attributo specifico TableCssId. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indica se aggiornare le impostazioni di SmartArt. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indica se convalidare le celle unite prima di salvare il file. |
| [getWarningCallback()](#getWarningCallback--) | Ottiene il callback di avviso. |
| [getWidthScalable()](#getWidthScalable--) | Indica se esportare la larghezza delle colonne in unità di scala in HTML. |
| [getWorksheetScalable()](#getWorksheetScalable--) | Indica se ingrandire o ridurre l'HTML tramite il livello di zoom del foglio di lavoro durante il salvataggio del file in HTML; il valore predefinito è false. |
| [hashCode()](#hashCode--) |  |
| [isBorderCollapsed()](#isBorderCollapsed--) | Indica se i bordi della tabella sono compressi. |
| [isExpImageToTempDir()](#isExpImageToTempDir--) | Indica se esportare i file immagine nella directory temporanea. |
| [isExportComments()](#isExportComments--) | Indica se esportare i commenti durante il salvataggio del file in HTML; il valore predefinito è false. |
| [isFullPathLink()](#isFullPathLink--) | Indicazione se utilizzare link con percorso completo in sheet00x.htm, filelist.xml e tabstrip.htm. |
| [isIECompatible()](#isIECompatible--) | Indicazione se l'HTML di output è compatibile con il browser IE. |
| [isJsBrowserCompatible()](#isJsBrowserCompatible--) | Indica se JavaScript è compatibile con i browser che non supportano JavaScript. |
| [isMobileCompatible()](#isMobileCompatible--) | Indica se l'HTML di output è compatibile con i dispositivi mobili. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddGenericFont(boolean value)](#setAddGenericFont-boolean-) | Indica se aggiungere un font generico alla proprietà CSS font-family. |
| [setAddTooltipText(boolean value)](#setAddTooltipText-boolean-) | Indica se aggiungere il testo del tooltip quando i dati non possono essere visualizzati completamente. |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | La directory in cui verranno salvati i file allegati. |
| [setAttachedFilesUrlPrefix(String value)](#setAttachedFilesUrlPrefix-java.lang.String-) | Specifica il prefisso Url dei file allegati, come le immagini, nel file html. |
| [setBorderCollapsed(boolean value)](#setBorderCollapsed-boolean-) | Indica se i bordi della tabella sono compressi. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | La cartella per i file temporanei che possono essere usati come cache dei dati. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Indica se calcolare le formule prima di salvare il file html. |
| [setCellCssPrefix(String value)](#setCellCssPrefix-java.lang.String-) | Imposta il prefisso del nome CSS; il valore predefinito è "". |
| [setCellNameAttribute(String value)](#setCellNameAttribute-java.lang.String-) | Specifica l'attributo che indica il CellName da scrivere. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Indica se verificare le restrizioni del file Excel quando l'utente modifica gli oggetti correlati alle celle. |
| [setClearData(boolean value)](#setClearData-boolean-) | Rendi il workbook vuoto dopo aver salvato il file. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. |
| [setCssStyles(String value)](#setCssStyles-java.lang.String-) | Imposta gli stili CSS aggiuntivi per il formattatore. |
| [setDataBarRenderMode(int value)](#setDataBarRenderMode-int-) | Rappresenta la modalità di rendering di DataBar durante la conversione dei file Excel in file html. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Specifica il nome del font predefinito per l'esportazione html; il font predefinito verrà usato quando il font dello stile non esiste. Se questa proprietà è null, Aspose.Cells utilizzerà un font universale che ha la stessa famiglia del font originale; il valore predefinito è null. |
| [setDisableCss(boolean value)](#setDisableCss-boolean-) | Indica se applicare solo stili inline, senza fare affidamento su CSS. |
| [setDisableDownlevelRevealedComments(boolean value)](#setDisableDownlevelRevealedComments-boolean-) | Indica se disabilitare i commenti condizionali Downlevel-revealed durante l'esportazione del file in html; il valore predefinito è false. |
| [setEmbeddedFontType(int value)](#setEmbeddedFontType-int-) | Imposta il tipo di incorporamento del file di font nel file HTML. |
| [setEnableCssCustomProperties(boolean value)](#setEnableCssCustomProperties-boolean-) | Ottimizza l'output html utilizzando le proprietà personalizzate CSS. |
| [setEncodeEntityAsCode(boolean value)](#setEncodeEntityAsCode-boolean-) | Indica se le entità dei caratteri html vengono sostituite con il codice decimale. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Se non impostato, utilizza Encoding.UTF8 come tipo di codifica predefinito. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indica se crittografare le proprietà del documento quando si salva come file .xls. |
| [setExcludeUnusedStyles(boolean value)](#setExcludeUnusedStyles-boolean-) | Indica se escludere gli stili non utilizzati. |
| [setExpImageToTempDir(boolean value)](#setExpImageToTempDir-boolean-) | Indica se esportare i file immagine nella directory temporanea. |
| [setExportActiveWorksheetOnly(boolean value)](#setExportActiveWorksheetOnly-boolean-) | Indica se esportare solo il foglio di lavoro attivo in un file html. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | Imposta l'area CellArea di esportazione del foglio di lavoro attivo corrente. |
| [setExportBogusRowData(boolean value)](#setExportBogusRowData-boolean-) | Indica se esportare dati di riga inferiore falsi. |
| [setExportCellCoordinate(boolean value)](#setExportCellCoordinate-boolean-) | Indica se esportare le coordinate Excel delle celle non vuote durante il salvataggio del file in html. |
| [setExportComments(boolean value)](#setExportComments-boolean-) | Indica se esportare i commenti durante il salvataggio del file in HTML; il valore predefinito è false. |
| [setExportCommentsType(int value)](#setExportCommentsType-int-) | Rappresenta il tipo di esportazione dei commenti nei file html. |
| [setExportDataOptions(int value)](#setExportDataOptions-int-) | Indica la regola di esportazione dei dati del file html. Il valore predefinito è All. |
| [setExportDocumentProperties(boolean value)](#setExportDocumentProperties-boolean-) | Indica se esportare le proprietà del documento. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito. |
| [setExportExtraHeadings(boolean value)](#setExportExtraHeadings-boolean-) | Indica se esportare intestazioni extra quando la lunghezza del testo supera la colonna di visualizzazione massima. |
| [setExportFormula(boolean value)](#setExportFormula-boolean-) | Indica se esportare le formule durante il salvataggio del file in html. |
| [setExportFrameScriptsAndProperties(boolean value)](#setExportFrameScriptsAndProperties-boolean-) | Indicazione se esportare script di frame e proprietà del documento. |
| [setExportGridLines(boolean value)](#setExportGridLines-boolean-) | Indicazione se esportare le linee della griglia. Il valore predefinito è false. |
| [setExportHeadings(boolean value)](#setExportHeadings-boolean-) | Indica se esportare le intestazioni di righe e colonne del foglio durante il salvataggio in file HTML. |
| [setExportHiddenWorksheet(boolean value)](#setExportHiddenWorksheet-boolean-) | Indicazione se esportare il contenuto del foglio di lavoro nascosto. Il valore predefinito è true. |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | Specifica se le immagini vengono salvate in formato Base64 in HTML, MHTML o EPUB. |
| [setExportNamedRangeAnchors(boolean value)](#setExportNamedRangeAnchors-boolean-) | Indica se esportare gli elementi di ancoraggio per gli intervalli denominati durante il salvataggio come HTML. |
| [setExportObjectListener(IExportObjectListener value)](#setExportObjectListener-com.aspose.cells.IExportObjectListener-) | Imposta l'ExportObjectListener per l'esportazione degli oggetti. |
| [setExportPageFooters(boolean value)](#setExportPageFooters-boolean-) | Indica se esportare le intestazioni di pagina. |
| [setExportPageHeaders(boolean value)](#setExportPageHeaders-boolean-) | Indica se esportare le intestazioni di pagina. |
| [setExportPrintAreaOnly(boolean value)](#setExportPrintAreaOnly-boolean-) | Indica se esportare solo l'area di stampa nel file HTML. |
| [setExportRowColumnHeadings(boolean value)](#setExportRowColumnHeadings-boolean-) | Indica se esportare le intestazioni di righe e colonne del foglio durante il salvataggio in file HTML. |
| [setExportSimilarBorderStyle(boolean value)](#setExportSimilarBorderStyle-boolean-) | Indicazione se esportare lo stile di bordo simile quando lo stile di bordo non è supportato dai browser. |
| [setExportSingleTab(boolean value)](#setExportSingleTab-boolean-) | Indica se esportare la singola scheda quando il file contiene un solo foglio di lavoro. |
| [setExportWorkbookProperties(boolean value)](#setExportWorkbookProperties-boolean-) | Indicazione se esportare le proprietà della cartella di lavoro. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito. |
| [setExportWorksheetCSSSeparately(boolean value)](#setExportWorksheetCSSSeparately-boolean-) | Indicazione se esportare il CSS del foglio di lavoro separatamente. Il valore predefinito è false. |
| [setExportWorksheetProperties(boolean value)](#setExportWorksheetProperties-boolean-) | Indicazione se esportare le proprietà del foglio di lavoro. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito. |
| [setFilePathProvider(IFilePathProvider value)](#setFilePathProvider-com.aspose.cells.IFilePathProvider-) | Imposta l'IFilePathProvider per l'esportazione del foglio di lavoro in HTML separatamente. |
| [setFormatDataIgnoreColumnWidth(boolean value)](#setFormatDataIgnoreColumnWidth-boolean-) | Indicazione se mostrare tutti i dati formattati della cella quando supera la colonna. |
| [setFullPathLink(boolean value)](#setFullPathLink-boolean-) | Indicazione se utilizzare link con percorso completo in sheet00x.htm, filelist.xml e tabstrip.htm. |
| [setHiddenColDisplayType(int value)](#setHiddenColDisplayType-int-) | Colonna nascosta (la larghezza di questa colonna è 0) in Excel, prima di salvarla in formato HTML, se HtmlHiddenColDisplayType è "Remove", la colonna nascosta non verrà emessa; se il valore è "Hidden", la colonna verrà emessa ma sarà nascosta; il valore predefinito è "Hidden". |
| [setHiddenRowDisplayType(int value)](#setHiddenRowDisplayType-int-) | Riga nascosta (l'altezza di questa riga è 0) in Excel, prima di salvarla in formato HTML, se HtmlHiddenRowDisplayType è "Remove", la riga nascosta non verrà emessa; se il valore è "Hidden", la riga verrà emessa ma sarà nascosta; il valore predefinito è "Hidden". |
| [setHideOverflowWrappedText(boolean value)](#setHideOverflowWrappedText-boolean-) | Indica se nascondere il testo in overflow quando il formato della cella è impostato per andare a capo. |
| [setHtmlCrossStringType(int value)](#setHtmlCrossStringType-int-) | Indica se una stringa che attraversa più celle verrà visualizzata nello stesso modo di MS Excel durante il salvataggio di un file Excel in formato HTML. |
| [setHtmlVersion(int value)](#setHtmlVersion-int-) | Specifica la versione dello standard HTML da utilizzare durante il salvataggio nel formato HTML. |
| [setIECompatible(boolean value)](#setIECompatible-boolean-) | Indicazione se l'HTML di output è compatibile con il browser IE. |
| [setIgnoreInvisibleShapes(boolean value)](#setIgnoreInvisibleShapes-boolean-) | Indica se esportare le forme non visibili |
| [setImageScalable(boolean value)](#setImageScalable-boolean-) | Indica se utilizzare unità scalabili per descrivere la larghezza dell'immagine quando si utilizzano unità scalabili per descrivere la larghezza della colonna. |
| [setJsBrowserCompatible(boolean value)](#setJsBrowserCompatible-boolean-) | Indica se JavaScript è compatibile con i browser che non supportano JavaScript. |
| [setLayoutMode(int value)](#setLayoutMode-int-) | Imposta la modalità di layout durante il salvataggio in HTML. |
| [setLinkTargetType(int value)](#setLinkTargetType-int-) | Indicazione del tipo di attributo target nel link `<a>`. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. |
| [setMergeEmptyTdForcely(boolean value)](#setMergeEmptyTdForcely-boolean-) | Indica se unire forzatamente gli elementi TD vuoti durante l'esportazione del file in HTML. |
| [setMergeEmptyTdType(int value)](#setMergeEmptyTdType-int-) | L'opzione per unire celle vuote contigue (elementi td vuoti). Il valore predefinito è MergeEmptyTdType.Default. |
| [setMobileCompatible(boolean value)](#setMobileCompatible-boolean-) | Indica se l'HTML di output è compatibile con i dispositivi mobili. |
| [setOfficeMathOutputMode(int value)](#setOfficeMathOutputMode-int-) | Indica come gli oggetti OfficeMath vengono esportati in HTML. Il valore predefinito è Image. |
| [setPageTitle(String value)](#setPageTitle-java.lang.String-) | Il titolo della pagina HTML. |
| [setParseHtmlTagInCell(boolean value)](#setParseHtmlTagInCell-boolean-) | Indica se il tag HTML (come `<div></div>`) nella cella deve essere analizzato come valore della cella o preservato così com'è. |
| [setPresentationPreference(boolean value)](#setPresentationPreference-boolean-) | Indicazione se il file HTML o MHT è la preferenza di presentazione. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indica se memorizzare nella cache i dati più recenti del grafico. |
| [setSaveAsSingleFile(boolean value)](#setSaveAsSingleFile-boolean-) | Indica se salvare l'HTML come file unico. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Imposta i fogli da rendere. |
| [setShowAllSheets(boolean value)](#setShowAllSheets-boolean-) | Indica se mostrare tutti i fogli quando si salva come file HTML unico. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indica se ordinare i nomi definiti esterni prima di salvare il file. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indica se ordinare i nomi definiti prima di salvare il file. |
| [setSpaceMode(int value)](#setSpaceMode-int-) | Indica come gli spazi vengono renderizzati nell'output HTML. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Imposta l'IStreamProvider per l'esportazione degli oggetti. |
| [setTableCssId(String value)](#setTableCssId-java.lang.String-) | Imposta il prefisso del nome CSS di tipo, come tr, col, td e così via; sono contenuti nell'elemento table che possiede l'attributo specifico TableCssId. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indica se aggiornare le impostazioni di SmartArt. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indica se convalidare le celle unite prima di salvare il file. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Imposta la callback di avviso. |
| [setWidthScalable(boolean value)](#setWidthScalable-boolean-) | Indica se esportare la larghezza delle colonne in unità di scala in HTML. |
| [setWorksheetScalable(boolean value)](#setWorksheetScalable-boolean-) | Indica se ingrandire o ridurre l'HTML tramite il livello di zoom del foglio di lavoro durante il salvataggio del file in HTML; il valore predefinito è false. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### EbookSaveOptions() {#EbookSaveOptions--}
```
public EbookSaveOptions()
```


Crea le opzioni per salvare il file ebook.

### EbookSaveOptions(int saveFormat) {#EbookSaveOptions-int-}
```
public EbookSaveOptions(int saveFormat)
```


Crea le opzioni per salvare il file ebook.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Il formato del file. Deve essere [SaveFormat.EPUB](../../com.aspose.cells/saveformat\#EPUB) o [SaveFormat.AZW\_3](../../com.aspose.cells/saveformat\#AZW-3). |

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
### getAddGenericFont() {#getAddGenericFont--}
```
public boolean getAddGenericFont()
```


Indica se aggiungere un font generico al CSS font-family. Il valore predefinito è true.

**Returns:**
boolean
### getAddTooltipText() {#getAddTooltipText--}
```
public boolean getAddTooltipText()
```


Indica se aggiungere il testo del tooltip quando i dati non possono essere visualizzati completamente. Il valore predefinito è false.

**Returns:**
boolean
### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}
```
public String getAttachedFilesDirectory()
```


La directory in cui verranno salvati i file allegati. Solo per il salvataggio in stream HTML.

**Returns:**
java.lang.String
### getAttachedFilesUrlPrefix() {#getAttachedFilesUrlPrefix--}
```
public String getAttachedFilesUrlPrefix()
```


Specifica il prefisso Url dei file allegati, come le immagini nel file HTML. Solo per il salvataggio in stream HTML.

**Returns:**
java.lang.String
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


La cartella per i file temporanei che possono essere usati come cache dei dati.

**Remarks**

Se la cartella non è stata specificata, il valore predefinito è [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Se il suo valore predefinito è null o vuoto, o è stato specificato come null o vuoto, allora non verrà utilizzato alcun file di cache durante il salvataggio del workbook.

**Returns:**
java.lang.String
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```


Indica se calcolare le formule prima di salvare il file html.

**Remarks**

Il valore predefinito è false.

**Returns:**
boolean
### getCellCssPrefix() {#getCellCssPrefix--}
```
public String getCellCssPrefix()
```


Ottiene il prefisso del nome css, il valore predefinito è "".

**Returns:**
java.lang.String
### getCellNameAttribute() {#getCellNameAttribute--}
```
public String getCellNameAttribute()
```


Specifica l'attributo che indica il CellName da scrivere. (ad esempio, se il valore è "id", allora per la cella "A1" l'output sarà: <td id='A1'>). Il valore predefinito è null.

**Returns:**
java.lang.String
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Ad esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando si inserisce un valore più lungo di 32K, verrà troncato.

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


Rendi il workbook vuoto dopo aver salvato il file.

**Returns:**
boolean
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file.

**Remarks**

Il valore predefinito è false.

**Returns:**
boolean
### getCssStyles() {#getCssStyles--}
```
public String getCssStyles()
```


Ottiene gli stili CSS aggiuntivi per il formatter. Funziona solo quando [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) è True. CssStyles="body \{ padding: 5px \}";

**Returns:**
java.lang.String
### getDataBarRenderMode() {#getDataBarRenderMode--}
```
public int getDataBarRenderMode()
```


Rappresenta la modalità di rendering di DataBar durante la conversione di file Excel in file HTML. Il valore predefinito è [DataBarRenderMode.BACKGROUND\_COLOR](../../com.aspose.cells/databarrendermode\#BACKGROUND-COLOR).

Vedi [DataBarRenderMode](../../com.aspose.cells/databarrendermode).

**Returns:**
int
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Specifica il nome del font predefinito per l'esportazione html; il font predefinito verrà usato quando il font dello stile non esiste. Se questa proprietà è null, Aspose.Cells utilizzerà un font universale che ha la stessa famiglia del font originale; il valore predefinito è null.

**Returns:**
java.lang.String
### getDisableCss() {#getDisableCss--}
```
public boolean getDisableCss()
```


Indica se vengono applicati solo stili inline, senza fare affidamento su CSS. Il valore predefinito è false.

**Returns:**
boolean
### getDisableDownlevelRevealedComments() {#getDisableDownlevelRevealedComments--}
```
public boolean getDisableDownlevelRevealedComments()
```


Indica se disabilitare i commenti condizionali Downlevel-revealed durante l'esportazione del file in html; il valore predefinito è false.

**Returns:**
boolean
### getEmbeddedFontType() {#getEmbeddedFontType--}
```
public int getEmbeddedFontType()
```


Ottiene il tipo di incorporamento del file font nel file HTML. Il valore predefinito è [HtmlEmbeddedFontType.NONE](../../com.aspose.cells/htmlembeddedfonttype\#NONE) che indica che nessun font sarà incorporato nell'HTML.

Vedi [HtmlEmbeddedFontType](../../com.aspose.cells/htmlembeddedfonttype).

**Returns:**
int
### getEnableCssCustomProperties() {#getEnableCssCustomProperties--}
```
public boolean getEnableCssCustomProperties()
```


Ottimizza l'output HTML utilizzando le proprietà personalizzate CSS. Ad esempio, nello scenario in cui ci sono più occorrenze della stessa immagine base64, con una proprietà personalizzata i dati dell'immagine devono essere salvati una sola volta, migliorando così le prestazioni dell'HTML risultante. Il valore predefinito è false.

**Returns:**
boolean
### getEncodeEntityAsCode() {#getEncodeEntityAsCode--}
```
public boolean getEncodeEntityAsCode()
```


Indica se le entità dei caratteri HTML vengono sostituite con il codice decimale. (ad esempio, "&nbsp;" viene sostituito con "&\#160;"). Il valore predefinito è false.

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Se non impostato, utilizza Encoding.UTF8 come tipo di codifica predefinito.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Indica se crittografare le proprietà del documento durante il salvataggio come file .xls. Il valore predefinito è true.

**Remarks**

Solo per i file .xls, .xlsx, .xlsb e .xlsm.

**Returns:**
boolean
### getExcludeUnusedStyles() {#getExcludeUnusedStyles--}
```
public boolean getExcludeUnusedStyles()
```


Indica se escludere gli stili non utilizzati. Per i file HTML generati, l'esclusione degli stili inutilizzati può ridurre la dimensione del file senza influire sugli effetti visivi. Pertanto il valore predefinito di questa proprietà è true. Se l'utente ha bisogno di mantenere tutti gli stili nella cartella di lavoro per l'HTML generato (ad esempio nello scenario in cui l'utente deve ripristinare la cartella di lavoro dall'HTML generato in seguito), impostare questa proprietà su false.

**Returns:**
boolean
### getExportActiveWorksheetOnly() {#getExportActiveWorksheetOnly--}
```
public boolean getExportActiveWorksheetOnly()
```


Indica se esportare solo il foglio di lavoro attivo in un file HTML. Se true, solo il foglio di lavoro attivo verrà esportato in un file HTML; se false, l'intera cartella di lavoro verrà esportata in un file HTML. Il valore predefinito è false.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


Ottiene l'area CellArea di esportazione del foglio di lavoro attivo corrente. Se imposti questo attributo, l'area di stampa del foglio di lavoro attivo corrente verrà omessa. Solo l'area specificata verrà esportata durante il salvataggio del file in HTML.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getExportBogusRowData() {#getExportBogusRowData--}
```
public boolean getExportBogusRowData()
```


Indica se esportare dati falsi nella riga inferiore. Il valore predefinito è true. Se desideri importare il file HTML o MHT in Excel, mantieni il valore predefinito.

**Returns:**
boolean
### getExportCellCoordinate() {#getExportCellCoordinate--}
```
public boolean getExportCellCoordinate()
```


Indica se esportare le coordinate Excel delle celle non vuote durante il salvataggio del file in HTML. Il valore predefinito è false. Se desideri importare l'HTML generato in Excel, mantieni il valore predefinito.

**Returns:**
boolean
### getExportCommentsType() {#getExportCommentsType--}
```
public int getExportCommentsType()
```


Rappresenta il tipo di esportazione dei commenti nei file html.

Vedi [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Returns:**
int
### getExportDataOptions() {#getExportDataOptions--}
```
public int getExportDataOptions()
```


Indica la regola di esportazione dei dati del file html. Il valore predefinito è All.

Vedi [HtmlExportDataOptions](../../com.aspose.cells/htmlexportdataoptions).

**Returns:**
int
### getExportDocumentProperties() {#getExportDocumentProperties--}
```
public boolean getExportDocumentProperties()
```


Indica se esportare le proprietà del documento. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito.

**Returns:**
boolean
### getExportExtraHeadings() {#getExportExtraHeadings--}
```
public boolean getExportExtraHeadings()
```


Indica se esportare intestazioni aggiuntive quando la lunghezza del testo supera la colonna di visualizzazione massima. Il valore predefinito è false. Se desideri importare il file HTML in Excel, mantieni il valore predefinito.

**Returns:**
boolean
### getExportFormula() {#getExportFormula--}
```
public boolean getExportFormula()
```


Indica se esportare le formule durante il salvataggio del file in HTML. Il valore predefinito è true. Se desideri importare l'HTML generato in Excel, mantieni il valore predefinito.

**Returns:**
boolean
### getExportFrameScriptsAndProperties() {#getExportFrameScriptsAndProperties--}
```
public boolean getExportFrameScriptsAndProperties()
```


Indica se esportare gli script dei frame e le proprietà del documento. Il valore predefinito è true. Se desideri importare il file HTML o MHT in Excel, mantieni il valore predefinito.

**Returns:**
boolean
### getExportGridLines() {#getExportGridLines--}
```
public boolean getExportGridLines()
```


Indicazione se esportare le linee della griglia. Il valore predefinito è false.

**Returns:**
boolean
### getExportHeadings() {#getExportHeadings--}
```
public boolean getExportHeadings()
```


Indica se esportare le intestazioni di righe e colonne del foglio durante il salvataggio in file HTML.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, utilizza la proprietà HtmlSaveOptions.ExportRowColumnHeadings. Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
boolean
### getExportHiddenWorksheet() {#getExportHiddenWorksheet--}
```
public boolean getExportHiddenWorksheet()
```


Indicazione se esportare il contenuto del foglio di lavoro nascosto. Il valore predefinito è true.

**Returns:**
boolean
### getExportImagesAsBase64() {#getExportImagesAsBase64--}
```
public boolean getExportImagesAsBase64()
```


Specifica se le immagini vengono salvate in formato Base64 in HTML, MHTML o EPUB.

**Remarks**

Quando questa proprietà è impostata su true, i dati dell'immagine vengono esportati direttamente negli elementi img e non vengono creati file separati.

**Returns:**
boolean
### getExportNamedRangeAnchors() {#getExportNamedRangeAnchors--}
```
public boolean getExportNamedRangeAnchors()
```


Indica se esportare gli elementi anchor per gli intervalli denominati durante il salvataggio come HTML. Il valore predefinito è true.

**Returns:**
boolean
### getExportObjectListener() {#getExportObjectListener--}
```
public IExportObjectListener getExportObjectListener()
```


Ottiene l'ExportObjectListener per l'esportazione degli oggetti.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, utilizza la proprietà HtmlSaveOptions.IStreamProvider. Questa proprietà sarà rimossa 12 mesi dopo, a partire da agosto 2015. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
[IExportObjectListener](../../com.aspose.cells/iexportobjectlistener)
### getExportPageFooters() {#getExportPageFooters--}
```
public boolean getExportPageFooters()
```


Indica se esportare le intestazioni di pagina.

**Remarks**

Funziona solo quando [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) è True.

**Returns:**
boolean
### getExportPageHeaders() {#getExportPageHeaders--}
```
public boolean getExportPageHeaders()
```


Indica se esportare le intestazioni di pagina.

**Remarks**

Funziona solo quando [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) è True.

**Returns:**
boolean
### getExportPrintAreaOnly() {#getExportPrintAreaOnly--}
```
public boolean getExportPrintAreaOnly()
```


Indica se esportare solo l'area di stampa nel file HTML. Il valore predefinito è false.

**Returns:**
boolean
### getExportRowColumnHeadings() {#getExportRowColumnHeadings--}
```
public boolean getExportRowColumnHeadings()
```


Indica se esportare le intestazioni di righe e colonne del foglio durante il salvataggio in file HTML.

**Remarks**

Il valore predefinito è false.

**Returns:**
boolean
### getExportSimilarBorderStyle() {#getExportSimilarBorderStyle--}
```
public boolean getExportSimilarBorderStyle()
```


Indica se esportare lo stile di bordo simile quando lo stile di bordo non è supportato dai browser. Se desideri importare il file HTML o MHT in Excel, mantieni il valore predefinito. Il valore predefinito è false.

**Returns:**
boolean
### getExportSingleTab() {#getExportSingleTab--}
```
public boolean getExportSingleTab()
```


Indica se esportare la singola scheda quando il file contiene solo un foglio di lavoro. Il valore predefinito è false.

**Returns:**
boolean
### getExportWorkbookProperties() {#getExportWorkbookProperties--}
```
public boolean getExportWorkbookProperties()
```


Indicazione se esportare le proprietà della cartella di lavoro. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito.

**Returns:**
boolean
### getExportWorksheetCSSSeparately() {#getExportWorksheetCSSSeparately--}
```
public boolean getExportWorksheetCSSSeparately()
```


Indicazione se esportare il CSS del foglio di lavoro separatamente. Il valore predefinito è false.

**Returns:**
boolean
### getExportWorksheetProperties() {#getExportWorksheetProperties--}
```
public boolean getExportWorksheetProperties()
```


Indicazione se esportare le proprietà del foglio di lavoro. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito.

**Returns:**
boolean
### getFilePathProvider() {#getFilePathProvider--}
```
public IFilePathProvider getFilePathProvider()
```


Ottiene l'IFilePathProvider per esportare il Worksheet in HTML separatamente.

**Returns:**
[IFilePathProvider](../../com.aspose.cells/ifilepathprovider)
### getFormatDataIgnoreColumnWidth() {#getFormatDataIgnoreColumnWidth--}
```
public boolean getFormatDataIgnoreColumnWidth()
```


Indica se mostrare tutti i dati formattati della cella quando il contenuto supera la colonna. Se true, la larghezza della colonna viene ignorata e tutti i dati della cella vengono esportati. Se false, i dati vengono esportati come in Excel. Il valore predefinito è false.

**Returns:**
boolean
### getHiddenColDisplayType() {#getHiddenColDisplayType--}
```
public int getHiddenColDisplayType()
```


Colonna nascosta (la larghezza di questa colonna è 0) in Excel, prima di salvarla in formato HTML, se HtmlHiddenColDisplayType è "Remove", la colonna nascosta non verrà emessa; se il valore è "Hidden", la colonna verrà emessa ma sarà nascosta; il valore predefinito è "Hidden".

Vedi [HtmlHiddenColDisplayType](../../com.aspose.cells/htmlhiddencoldisplaytype).

**Returns:**
int
### getHiddenRowDisplayType() {#getHiddenRowDisplayType--}
```
public int getHiddenRowDisplayType()
```


Riga nascosta (l'altezza di questa riga è 0) in Excel, prima di salvarla in formato HTML, se HtmlHiddenRowDisplayType è "Remove", la riga nascosta non verrà emessa; se il valore è "Hidden", la riga verrà emessa ma sarà nascosta; il valore predefinito è "Hidden".

Vedi [HtmlHiddenRowDisplayType](../../com.aspose.cells/htmlhiddenrowdisplaytype).

**Returns:**
int
### getHideOverflowWrappedText() {#getHideOverflowWrappedText--}
```
public boolean getHideOverflowWrappedText()
```


Indica se nascondere il testo in eccesso quando il formato della cella è impostato su a capo automatico. Il valore predefinito è false

**Returns:**
boolean
### getHtmlCrossStringType() {#getHtmlCrossStringType--}
```
public int getHtmlCrossStringType()
```


Indica se una stringa che attraversa più celle verrà visualizzata nello stesso modo di MS Excel quando si salva un file Excel in formato HTML. Per impostazione predefinita il valore è Default, quindi per le stringhe che attraversano più celle c'è poca differenza tra i file HTML creati da Aspose.Cells e MS Excel. Tuttavia le prestazioni nella creazione di file HTML di grandi dimensioni, impostando il valore su Cross, sarebbero diverse volte più rapide rispetto a impostarlo su Default o Fit2Cell.

Vedi [HtmlCrossType](../../com.aspose.cells/htmlcrosstype).

**Returns:**
int
### getHtmlVersion() {#getHtmlVersion--}
```
public int getHtmlVersion()
```


Specifica la versione dello standard HTML da utilizzare durante il salvataggio nel formato HTML. Il valore predefinito è HtmlVersion.Default.

Vedi [HtmlVersion](../../com.aspose.cells/htmlversion).

**Returns:**
int
### getIgnoreInvisibleShapes() {#getIgnoreInvisibleShapes--}
```
public boolean getIgnoreInvisibleShapes()
```


Indica se esportare le forme non visibili

**Remarks**

Il valore predefinito è false.

**Returns:**
boolean
### getImageOptions() {#getImageOptions--}
```
public ImageOrPrintOptions getImageOptions()
```


Ottieni l'oggetto ImageOrPrintOptions prima dell'esportazione

**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
### getImageScalable() {#getImageScalable--}
```
public boolean getImageScalable()
```


Indica se utilizzare unità scalabili per descrivere la larghezza dell'immagine quando si utilizzano unità scalabili per descrivere la larghezza della colonna. Il valore predefinito è true.

**Returns:**
boolean
### getLayoutMode() {#getLayoutMode--}
```
public int getLayoutMode()
```


Ottiene la modalità di layout durante il salvataggio in HTML. Il valore predefinito è [HtmlLayoutMode.NORMAL](../../com.aspose.cells/htmllayoutmode\#NORMAL)

Vedi [HtmlLayoutMode](../../com.aspose.cells/htmllayoutmode).

**Returns:**
int
### getLinkTargetType() {#getLinkTargetType--}
```
public int getLinkTargetType()
```


Indica il tipo dell'attributo target nel collegamento `<a>`. Il valore predefinito è HtmlLinkTargetType.Parent.

Vedi [HtmlLinkTargetType](../../com.aspose.cells/htmllinktargettype).

**Returns:**
int
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file.

**Remarks**

Il valore predefinito è false.

**Returns:**
boolean
### getMergeEmptyTdForcely() {#getMergeEmptyTdForcely--}
```
public boolean getMergeEmptyTdForcely()
```


Indica se unire forzatamente gli elementi TD vuoti durante l'esportazione del file in html. La dimensione del file html sarà ridotta in modo significativo impostando il valore su true. Il valore predefinito è false. Se desideri importare il file html in Excel o esportare linee di griglia perfette quando salvi il file in html, mantieni il valore predefinito.

**Returns:**
boolean
### getMergeEmptyTdType() {#getMergeEmptyTdType--}
```
public int getMergeEmptyTdType()
```


L'opzione per unire celle vuote contigue (elementi td vuoti). Il valore predefinito è MergeEmptyTdType.Default.

Vedi [MergeEmptyTdType](../../com.aspose.cells/mergeemptytdtype).

**Returns:**
int
### getOfficeMathOutputMode() {#getOfficeMathOutputMode--}
```
public int getOfficeMathOutputMode()
```


Indica come gli oggetti OfficeMath vengono esportati in HTML. Il valore predefinito è Image.

Vedi [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype).

**Returns:**
int
### getPageTitle() {#getPageTitle--}
```
public String getPageTitle()
```


Il titolo della pagina html. Solo per il salvataggio su stream html.

**Returns:**
java.lang.String
### getParseHtmlTagInCell() {#getParseHtmlTagInCell--}
```
public boolean getParseHtmlTagInCell()
```


Indica se il tag html (come `<div></div>`) nella cella deve essere analizzato come valore della cella o conservato così com'è. Il valore predefinito è true.

**Returns:**
boolean
### getPresentationPreference() {#getPresentationPreference--}
```
public boolean getPresentationPreference()
```


Indica se il file html o mht è la preferenza di presentazione. Il valore predefinito è false. Se desideri una presentazione più bella, imposta il valore su true.

**Returns:**
boolean
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Indica se memorizzare nella cache i dati più recenti del grafico.

**Returns:**
boolean
### getSaveAsSingleFile() {#getSaveAsSingleFile--}
```
public boolean getSaveAsSingleFile()
```


Indica se salvare l'html come file unico. Il valore predefinito è false.

**Remarks**

Se nel workbook sono presenti più fogli di lavoro o altre risorse necessarie, come immagini, solitamente questi fogli e risorse devono essere salvati in file separati. In alcuni scenari, l'utente potrebbe aver bisogno di ottenere un unico file risultante per comodità di trasferimento. In tal caso, l'utente può impostare questa proprietà su true.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Ottiene il formato di salvataggio del file.

Vedi [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


Ottiene i fogli da renderizzare. Il valore predefinito è tutti i fogli visibili nel workbook: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getShowAllSheets() {#getShowAllSheets--}
```
public boolean getShowAllSheets()
```


Indica se mostrare tutti i fogli quando si salva come file HTML unico.

**Remarks**

Funziona solo quando [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) è True.

**Returns:**
boolean
### getSortExternalNames() {#getSortExternalNames--}
```
public boolean getSortExternalNames()
```


Indica se ordinare i nomi definiti esterni prima di salvare il file.

**Returns:**
boolean
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


Indica se ordinare i nomi definiti prima di salvare il file.

**Returns:**
boolean
### getSpaceMode() {#getSpaceMode--}
```
public int getSpaceMode()
```


Indica come gli spazi vengono renderizzati nell'output HTML. Questa opzione è attualmente applicata solo ai formati numerici (ad es. formato contabile). Il valore predefinito è [HtmlSpaceMode.CSS](../../com.aspose.cells/htmlspacemode\#CSS).

Vedi [HtmlSpaceMode](../../com.aspose.cells/htmlspacemode).

**Returns:**
int
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


Ottiene l'IStreamProvider per l'esportazione degli oggetti.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getTableCssId() {#getTableCssId--}
```
public String getTableCssId()
```


Ottiene il prefisso del nome css di tipo come tr, col, td e così via, contenuti nell'elemento table che ha l'attributo specifico TableCssId. Il valore predefinito è "".

**Returns:**
java.lang.String
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


Indica se aggiornare l'impostazione Smart Art. Il valore predefinito è false.

**Remarks**

Ha effetto solo dopo aver chiamato il metodo Shape.GetResultOfSmartArt() e quando le forme memorizzate nella cache esistono nel file modello.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


Indica se convalidare le celle unite prima di salvare il file.

**Remarks**

Il valore predefinito è false.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Ottiene il callback di avviso.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### getWidthScalable() {#getWidthScalable--}
```
public boolean getWidthScalable()
```


Indica se esportare la larghezza della colonna in unità di scala in html. Il valore predefinito è false.

**Returns:**
boolean
### getWorksheetScalable() {#getWorksheetScalable--}
```
public boolean getWorksheetScalable()
```


Indica se ingrandire o ridurre l'HTML tramite il livello di zoom del foglio di lavoro durante il salvataggio del file in HTML; il valore predefinito è false.

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


Indica se i bordi della tabella sono collassati. Il valore predefinito è true.

**Returns:**
boolean
### isExpImageToTempDir() {#isExpImageToTempDir--}
```
public boolean isExpImageToTempDir()
```


Indica se esportare i file immagine in una directory temporanea. Solo per il salvataggio su stream html.

**Returns:**
boolean
### isExportComments() {#isExportComments--}
```
public boolean isExportComments()
```


Indica se esportare i commenti durante il salvataggio del file in HTML; il valore predefinito è false.

**Returns:**
boolean
### isFullPathLink() {#isFullPathLink--}
```
public boolean isFullPathLink()
```


Indica se utilizzare link con percorso completo in sheet00x.htm, filelist.xml e tabstrip.htm. Il valore predefinito è false.

**Returns:**
boolean
### isIECompatible() {#isIECompatible--}
```
public boolean isIECompatible()
```


Indica se l'HTML di output è compatibile con il browser IE. Il valore predefinito è false.

**Returns:**
boolean
### isJsBrowserCompatible() {#isJsBrowserCompatible--}
```
public boolean isJsBrowserCompatible()
```


Indica se JavaScript è compatibile con i browser che non supportano JavaScript. Il valore predefinito è true.

**Returns:**
boolean
### isMobileCompatible() {#isMobileCompatible--}
```
public boolean isMobileCompatible()
```


Indica se l'HTML di output è compatibile con i dispositivi mobili. Il valore predefinito è false.

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


Indica se aggiungere un font generico al CSS font-family. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAddTooltipText(boolean value) {#setAddTooltipText-boolean-}
```
public void setAddTooltipText(boolean value)
```


Indica se aggiungere il testo del tooltip quando i dati non possono essere visualizzati completamente. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAttachedFilesDirectory(String value) {#setAttachedFilesDirectory-java.lang.String-}
```
public void setAttachedFilesDirectory(String value)
```


La directory in cui verranno salvati i file allegati. Solo per il salvataggio in stream HTML.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setAttachedFilesUrlPrefix(String value) {#setAttachedFilesUrlPrefix-java.lang.String-}
```
public void setAttachedFilesUrlPrefix(String value)
```


Specifica il prefisso Url dei file allegati, come le immagini nel file HTML. Solo per il salvataggio in stream HTML.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setBorderCollapsed(boolean value) {#setBorderCollapsed-boolean-}
```
public void setBorderCollapsed(boolean value)
```


Indica se i bordi della tabella sono collassati. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


La cartella per i file temporanei che possono essere usati come cache dei dati.

**Remarks**

Se la cartella non è stata specificata, il valore predefinito è [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Se il suo valore predefinito è null o vuoto, o è stato specificato come null o vuoto, allora non verrà utilizzato alcun file di cache durante il salvataggio del workbook.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


Indica se calcolare le formule prima di salvare il file html.

**Remarks**

Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCellCssPrefix(String value) {#setCellCssPrefix-java.lang.String-}
```
public void setCellCssPrefix(String value)
```


Imposta il prefisso del nome CSS; il valore predefinito è "".

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCellNameAttribute(String value) {#setCellNameAttribute-java.lang.String-}
```
public void setCellNameAttribute(String value)
```


Specifica l'attributo che indica il CellName da scrivere. (ad esempio, se il valore è "id", allora per la cella "A1" l'output sarà: <td id='A1'>). Il valore predefinito è null.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Ad esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando si inserisce un valore più lungo di 32K, verrà troncato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


Rendi il workbook vuoto dopo aver salvato il file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file.

**Remarks**

Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCssStyles(String value) {#setCssStyles-java.lang.String-}
```
public void setCssStyles(String value)
```


Imposta gli stili css aggiuntivi per il formattatore. Funziona solo quando [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) è True.  CssStyles="body \{ padding: 5px \}";

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setDataBarRenderMode(int value) {#setDataBarRenderMode-int-}
```
public void setDataBarRenderMode(int value)
```


Rappresenta la modalità di rendering di DataBar durante la conversione di file Excel in file HTML. Il valore predefinito è [DataBarRenderMode.BACKGROUND\_COLOR](../../com.aspose.cells/databarrendermode\#BACKGROUND-COLOR).

Vedi [DataBarRenderMode](../../com.aspose.cells/databarrendermode).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Specifica il nome del font predefinito per l'esportazione html; il font predefinito verrà usato quando il font dello stile non esiste. Se questa proprietà è null, Aspose.Cells utilizzerà un font universale che ha la stessa famiglia del font originale; il valore predefinito è null.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setDisableCss(boolean value) {#setDisableCss-boolean-}
```
public void setDisableCss(boolean value)
```


Indica se vengono applicati solo stili inline, senza fare affidamento su CSS. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDisableDownlevelRevealedComments(boolean value) {#setDisableDownlevelRevealedComments-boolean-}
```
public void setDisableDownlevelRevealedComments(boolean value)
```


Indica se disabilitare i commenti condizionali Downlevel-revealed durante l'esportazione del file in html; il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEmbeddedFontType(int value) {#setEmbeddedFontType-int-}
```
public void setEmbeddedFontType(int value)
```


Imposta il tipo di incorporamento del file di font nel file html. Il valore predefinito è [HtmlEmbeddedFontType.NONE](../../com.aspose.cells/htmlembeddedfonttype\#NONE) che indica che nessun font sarà incorporato nell'html.

Vedi [HtmlEmbeddedFontType](../../com.aspose.cells/htmlembeddedfonttype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setEnableCssCustomProperties(boolean value) {#setEnableCssCustomProperties-boolean-}
```
public void setEnableCssCustomProperties(boolean value)
```


Ottimizza l'output HTML utilizzando le proprietà personalizzate CSS. Ad esempio, nello scenario in cui ci sono più occorrenze della stessa immagine base64, con una proprietà personalizzata i dati dell'immagine devono essere salvati una sola volta, migliorando così le prestazioni dell'HTML risultante. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEncodeEntityAsCode(boolean value) {#setEncodeEntityAsCode-boolean-}
```
public void setEncodeEntityAsCode(boolean value)
```


Indica se le entità dei caratteri HTML vengono sostituite con il codice decimale. (ad esempio, "&nbsp;" viene sostituito con "&\#160;"). Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Se non impostato, utilizza Encoding.UTF8 come tipo di codifica predefinito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setEncryptDocumentProperties(boolean value) {#setEncryptDocumentProperties-boolean-}
```
public void setEncryptDocumentProperties(boolean value)
```


Indica se crittografare le proprietà del documento durante il salvataggio come file .xls. Il valore predefinito è true.

**Remarks**

Solo per i file .xls, .xlsx, .xlsb e .xlsm.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExcludeUnusedStyles(boolean value) {#setExcludeUnusedStyles-boolean-}
```
public void setExcludeUnusedStyles(boolean value)
```


Indica se escludere gli stili non utilizzati. Per i file HTML generati, l'esclusione degli stili inutilizzati può ridurre la dimensione del file senza influire sugli effetti visivi. Pertanto il valore predefinito di questa proprietà è true. Se l'utente ha bisogno di mantenere tutti gli stili nella cartella di lavoro per l'HTML generato (ad esempio nello scenario in cui l'utente deve ripristinare la cartella di lavoro dall'HTML generato in seguito), impostare questa proprietà su false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExpImageToTempDir(boolean value) {#setExpImageToTempDir-boolean-}
```
public void setExpImageToTempDir(boolean value)
```


Indica se esportare i file immagine in una directory temporanea. Solo per il salvataggio su stream html.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportActiveWorksheetOnly(boolean value) {#setExportActiveWorksheetOnly-boolean-}
```
public void setExportActiveWorksheetOnly(boolean value)
```


Indica se esportare solo il foglio di lavoro attivo in un file HTML. Se true, solo il foglio di lavoro attivo verrà esportato in un file HTML; se false, l'intera cartella di lavoro verrà esportata in un file HTML. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


Imposta l'area di celle da esportare del foglio di lavoro attivo corrente. Se imposti questo attributo, l'area di stampa del foglio di lavoro attivo corrente verrà omessa. Solo l'area specificata sarà esportata quando si salva il file in html.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportBogusRowData(boolean value) {#setExportBogusRowData-boolean-}
```
public void setExportBogusRowData(boolean value)
```


Indica se esportare dati falsi nella riga inferiore. Il valore predefinito è true. Se desideri importare il file HTML o MHT in Excel, mantieni il valore predefinito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportCellCoordinate(boolean value) {#setExportCellCoordinate-boolean-}
```
public void setExportCellCoordinate(boolean value)
```


Indica se esportare le coordinate Excel delle celle non vuote durante il salvataggio del file in HTML. Il valore predefinito è false. Se desideri importare l'HTML generato in Excel, mantieni il valore predefinito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportComments(boolean value) {#setExportComments-boolean-}
```
public void setExportComments(boolean value)
```


Indica se esportare i commenti durante il salvataggio del file in HTML; il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportCommentsType(int value) {#setExportCommentsType-int-}
```
public void setExportCommentsType(int value)
```


Rappresenta il tipo di esportazione dei commenti nei file html.

Vedi [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setExportDataOptions(int value) {#setExportDataOptions-int-}
```
public void setExportDataOptions(int value)
```


Indica la regola di esportazione dei dati del file html. Il valore predefinito è All.

Vedi [HtmlExportDataOptions](../../com.aspose.cells/htmlexportdataoptions).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setExportDocumentProperties(boolean value) {#setExportDocumentProperties-boolean-}
```
public void setExportDocumentProperties(boolean value)
```


Indica se esportare le proprietà del documento. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportExtraHeadings(boolean value) {#setExportExtraHeadings-boolean-}
```
public void setExportExtraHeadings(boolean value)
```


Indica se esportare intestazioni aggiuntive quando la lunghezza del testo supera la colonna di visualizzazione massima. Il valore predefinito è false. Se desideri importare il file HTML in Excel, mantieni il valore predefinito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportFormula(boolean value) {#setExportFormula-boolean-}
```
public void setExportFormula(boolean value)
```


Indica se esportare le formule durante il salvataggio del file in HTML. Il valore predefinito è true. Se desideri importare l'HTML generato in Excel, mantieni il valore predefinito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportFrameScriptsAndProperties(boolean value) {#setExportFrameScriptsAndProperties-boolean-}
```
public void setExportFrameScriptsAndProperties(boolean value)
```


Indica se esportare gli script dei frame e le proprietà del documento. Il valore predefinito è true. Se desideri importare il file HTML o MHT in Excel, mantieni il valore predefinito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportGridLines(boolean value) {#setExportGridLines-boolean-}
```
public void setExportGridLines(boolean value)
```


Indicazione se esportare le linee della griglia. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportHeadings(boolean value) {#setExportHeadings-boolean-}
```
public void setExportHeadings(boolean value)
```


Indica se esportare le intestazioni di righe e colonne del foglio durante il salvataggio in file HTML.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, utilizza la proprietà HtmlSaveOptions.ExportRowColumnHeadings. Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportHiddenWorksheet(boolean value) {#setExportHiddenWorksheet-boolean-}
```
public void setExportHiddenWorksheet(boolean value)
```


Indicazione se esportare il contenuto del foglio di lavoro nascosto. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportImagesAsBase64(boolean value) {#setExportImagesAsBase64-boolean-}
```
public void setExportImagesAsBase64(boolean value)
```


Specifica se le immagini vengono salvate in formato Base64 in HTML, MHTML o EPUB.

**Remarks**

Quando questa proprietà è impostata su true, i dati dell'immagine vengono esportati direttamente negli elementi img e non vengono creati file separati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportNamedRangeAnchors(boolean value) {#setExportNamedRangeAnchors-boolean-}
```
public void setExportNamedRangeAnchors(boolean value)
```


Indica se esportare gli elementi anchor per gli intervalli denominati durante il salvataggio come HTML. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportObjectListener(IExportObjectListener value) {#setExportObjectListener-com.aspose.cells.IExportObjectListener-}
```
public void setExportObjectListener(IExportObjectListener value)
```


Imposta l'ExportObjectListener per l'esportazione degli oggetti.

**Remarks**

NOTA: Questa proprietà è ora obsoleta. Invece, utilizza la proprietà HtmlSaveOptions.IStreamProvider. Questa proprietà sarà rimossa 12 mesi dopo, a partire da agosto 2015. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [IExportObjectListener](../../com.aspose.cells/iexportobjectlistener) |  |

### setExportPageFooters(boolean value) {#setExportPageFooters-boolean-}
```
public void setExportPageFooters(boolean value)
```


Indica se esportare le intestazioni di pagina.

**Remarks**

Funziona solo quando [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) è True.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportPageHeaders(boolean value) {#setExportPageHeaders-boolean-}
```
public void setExportPageHeaders(boolean value)
```


Indica se esportare le intestazioni di pagina.

**Remarks**

Funziona solo quando [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) è True.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportPrintAreaOnly(boolean value) {#setExportPrintAreaOnly-boolean-}
```
public void setExportPrintAreaOnly(boolean value)
```


Indica se esportare solo l'area di stampa nel file HTML. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportRowColumnHeadings(boolean value) {#setExportRowColumnHeadings-boolean-}
```
public void setExportRowColumnHeadings(boolean value)
```


Indica se esportare le intestazioni di righe e colonne del foglio durante il salvataggio in file HTML.

**Remarks**

Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportSimilarBorderStyle(boolean value) {#setExportSimilarBorderStyle-boolean-}
```
public void setExportSimilarBorderStyle(boolean value)
```


Indica se esportare lo stile di bordo simile quando lo stile di bordo non è supportato dai browser. Se desideri importare il file HTML o MHT in Excel, mantieni il valore predefinito. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportSingleTab(boolean value) {#setExportSingleTab-boolean-}
```
public void setExportSingleTab(boolean value)
```


Indica se esportare la singola scheda quando il file contiene solo un foglio di lavoro. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportWorkbookProperties(boolean value) {#setExportWorkbookProperties-boolean-}
```
public void setExportWorkbookProperties(boolean value)
```


Indicazione se esportare le proprietà della cartella di lavoro. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportWorksheetCSSSeparately(boolean value) {#setExportWorksheetCSSSeparately-boolean-}
```
public void setExportWorksheetCSSSeparately(boolean value)
```


Indicazione se esportare il CSS del foglio di lavoro separatamente. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExportWorksheetProperties(boolean value) {#setExportWorksheetProperties-boolean-}
```
public void setExportWorksheetProperties(boolean value)
```


Indicazione se esportare le proprietà del foglio di lavoro. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFilePathProvider(IFilePathProvider value) {#setFilePathProvider-com.aspose.cells.IFilePathProvider-}
```
public void setFilePathProvider(IFilePathProvider value)
```


Imposta l'IFilePathProvider per l'esportazione del foglio di lavoro in HTML separatamente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [IFilePathProvider](../../com.aspose.cells/ifilepathprovider) |  |

### setFormatDataIgnoreColumnWidth(boolean value) {#setFormatDataIgnoreColumnWidth-boolean-}
```
public void setFormatDataIgnoreColumnWidth(boolean value)
```


Indica se mostrare tutti i dati formattati della cella quando il contenuto supera la colonna. Se true, la larghezza della colonna viene ignorata e tutti i dati della cella vengono esportati. Se false, i dati vengono esportati come in Excel. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFullPathLink(boolean value) {#setFullPathLink-boolean-}
```
public void setFullPathLink(boolean value)
```


Indica se utilizzare link con percorso completo in sheet00x.htm, filelist.xml e tabstrip.htm. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHiddenColDisplayType(int value) {#setHiddenColDisplayType-int-}
```
public void setHiddenColDisplayType(int value)
```


Colonna nascosta (la larghezza di questa colonna è 0) in Excel, prima di salvarla in formato HTML, se HtmlHiddenColDisplayType è "Remove", la colonna nascosta non verrà emessa; se il valore è "Hidden", la colonna verrà emessa ma sarà nascosta; il valore predefinito è "Hidden".

Vedi [HtmlHiddenColDisplayType](../../com.aspose.cells/htmlhiddencoldisplaytype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setHiddenRowDisplayType(int value) {#setHiddenRowDisplayType-int-}
```
public void setHiddenRowDisplayType(int value)
```


Riga nascosta (l'altezza di questa riga è 0) in Excel, prima di salvarla in formato HTML, se HtmlHiddenRowDisplayType è "Remove", la riga nascosta non verrà emessa; se il valore è "Hidden", la riga verrà emessa ma sarà nascosta; il valore predefinito è "Hidden".

Vedi [HtmlHiddenRowDisplayType](../../com.aspose.cells/htmlhiddenrowdisplaytype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setHideOverflowWrappedText(boolean value) {#setHideOverflowWrappedText-boolean-}
```
public void setHideOverflowWrappedText(boolean value)
```


Indica se nascondere il testo in eccesso quando il formato della cella è impostato su a capo automatico. Il valore predefinito è false

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHtmlCrossStringType(int value) {#setHtmlCrossStringType-int-}
```
public void setHtmlCrossStringType(int value)
```


Indica se una stringa che attraversa più celle verrà visualizzata nello stesso modo di MS Excel quando si salva un file Excel in formato HTML. Per impostazione predefinita il valore è Default, quindi per le stringhe che attraversano più celle c'è poca differenza tra i file HTML creati da Aspose.Cells e MS Excel. Tuttavia le prestazioni nella creazione di file HTML di grandi dimensioni, impostando il valore su Cross, sarebbero diverse volte più rapide rispetto a impostarlo su Default o Fit2Cell.

Vedi [HtmlCrossType](../../com.aspose.cells/htmlcrosstype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setHtmlVersion(int value) {#setHtmlVersion-int-}
```
public void setHtmlVersion(int value)
```


Specifica la versione dello standard HTML da utilizzare durante il salvataggio nel formato HTML. Il valore predefinito è HtmlVersion.Default.

Vedi [HtmlVersion](../../com.aspose.cells/htmlversion).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setIECompatible(boolean value) {#setIECompatible-boolean-}
```
public void setIECompatible(boolean value)
```


Indica se l'HTML di output è compatibile con il browser IE. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setIgnoreInvisibleShapes(boolean value) {#setIgnoreInvisibleShapes-boolean-}
```
public void setIgnoreInvisibleShapes(boolean value)
```


Indica se esportare le forme non visibili

**Remarks**

Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setImageScalable(boolean value) {#setImageScalable-boolean-}
```
public void setImageScalable(boolean value)
```


Indica se utilizzare unità scalabili per descrivere la larghezza dell'immagine quando si utilizzano unità scalabili per descrivere la larghezza della colonna. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setJsBrowserCompatible(boolean value) {#setJsBrowserCompatible-boolean-}
```
public void setJsBrowserCompatible(boolean value)
```


Indica se JavaScript è compatibile con i browser che non supportano JavaScript. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setLayoutMode(int value) {#setLayoutMode-int-}
```
public void setLayoutMode(int value)
```


Imposta la modalità di layout durante il salvataggio in HTML. Il valore predefinito è [HtmlLayoutMode.NORMAL](../../com.aspose.cells/htmllayoutmode\#NORMAL)

Vedi [HtmlLayoutMode](../../com.aspose.cells/htmllayoutmode).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setLinkTargetType(int value) {#setLinkTargetType-int-}
```
public void setLinkTargetType(int value)
```


Indica il tipo dell'attributo target nel collegamento `<a>`. Il valore predefinito è HtmlLinkTargetType.Parent.

Vedi [HtmlLinkTargetType](../../com.aspose.cells/htmllinktargettype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file.

**Remarks**

Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setMergeEmptyTdForcely(boolean value) {#setMergeEmptyTdForcely-boolean-}
```
public void setMergeEmptyTdForcely(boolean value)
```


Indica se unire forzatamente gli elementi TD vuoti durante l'esportazione del file in html. La dimensione del file html sarà ridotta in modo significativo impostando il valore su true. Il valore predefinito è false. Se desideri importare il file html in Excel o esportare linee di griglia perfette quando salvi il file in html, mantieni il valore predefinito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setMergeEmptyTdType(int value) {#setMergeEmptyTdType-int-}
```
public void setMergeEmptyTdType(int value)
```


L'opzione per unire celle vuote contigue (elementi td vuoti). Il valore predefinito è MergeEmptyTdType.Default.

Vedi [MergeEmptyTdType](../../com.aspose.cells/mergeemptytdtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMobileCompatible(boolean value) {#setMobileCompatible-boolean-}
```
public void setMobileCompatible(boolean value)
```


Indica se l'HTML di output è compatibile con i dispositivi mobili. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setOfficeMathOutputMode(int value) {#setOfficeMathOutputMode-int-}
```
public void setOfficeMathOutputMode(int value)
```


Indica come gli oggetti OfficeMath vengono esportati in HTML. Il valore predefinito è Image.

Vedi [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPageTitle(String value) {#setPageTitle-java.lang.String-}
```
public void setPageTitle(String value)
```


Il titolo della pagina html. Solo per il salvataggio su stream html.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setParseHtmlTagInCell(boolean value) {#setParseHtmlTagInCell-boolean-}
```
public void setParseHtmlTagInCell(boolean value)
```


Indica se il tag html (come `<div></div>`) nella cella deve essere analizzato come valore della cella o conservato così com'è. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPresentationPreference(boolean value) {#setPresentationPreference-boolean-}
```
public void setPresentationPreference(boolean value)
```


Indica se il file html o mht è la preferenza di presentazione. Il valore predefinito è false. Se desideri una presentazione più bella, imposta il valore su true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Indica se memorizzare nella cache i dati più recenti del grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSaveAsSingleFile(boolean value) {#setSaveAsSingleFile-boolean-}
```
public void setSaveAsSingleFile(boolean value)
```


Indica se salvare l'html come file unico. Il valore predefinito è false.

**Remarks**

Se nel workbook sono presenti più fogli di lavoro o altre risorse necessarie, come immagini, solitamente questi fogli e risorse devono essere salvati in file separati. In alcuni scenari, l'utente potrebbe aver bisogno di ottenere un unico file risultante per comodità di trasferimento. In tal caso, l'utente può impostare questa proprietà su true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


Imposta i fogli da renderizzare. L'impostazione predefinita è tutti i fogli visibili nella cartella di lavoro: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

### setShowAllSheets(boolean value) {#setShowAllSheets-boolean-}
```
public void setShowAllSheets(boolean value)
```


Indica se mostrare tutti i fogli quando si salva come file HTML unico.

**Remarks**

Funziona solo quando [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) è True.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


Indica se ordinare i nomi definiti esterni prima di salvare il file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


Indica se ordinare i nomi definiti prima di salvare il file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSpaceMode(int value) {#setSpaceMode-int-}
```
public void setSpaceMode(int value)
```


Indica come gli spazi vengono renderizzati nell'output HTML. Questa opzione è attualmente applicata solo ai formati numerici (ad es. formato contabile). Il valore predefinito è [HtmlSpaceMode.CSS](../../com.aspose.cells/htmlspacemode\#CSS).

Vedi [HtmlSpaceMode](../../com.aspose.cells/htmlspacemode).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


Imposta l'IStreamProvider per l'esportazione degli oggetti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setTableCssId(String value) {#setTableCssId-java.lang.String-}
```
public void setTableCssId(String value)
```


Imposta il prefisso del nome CSS di tipo, come tr, col, td e così via; sono contenuti nell'elemento table che possiede l'attributo specifico TableCssId. Il valore predefinito è "".

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


Indica se aggiornare l'impostazione Smart Art. Il valore predefinito è false.

**Remarks**

Ha effetto solo dopo aver chiamato il metodo Shape.GetResultOfSmartArt() e quando le forme memorizzate nella cache esistono nel file modello.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


Indica se convalidare le celle unite prima di salvare il file.

**Remarks**

Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Imposta la callback di avviso.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

### setWidthScalable(boolean value) {#setWidthScalable-boolean-}
```
public void setWidthScalable(boolean value)
```


Indica se esportare la larghezza della colonna in unità di scala in html. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setWorksheetScalable(boolean value) {#setWorksheetScalable-boolean-}
```
public void setWorksheetScalable(boolean value)
```


Indica se ingrandire o ridurre l'HTML tramite il livello di zoom del foglio di lavoro durante il salvataggio del file in HTML; il valore predefinito è false.

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

