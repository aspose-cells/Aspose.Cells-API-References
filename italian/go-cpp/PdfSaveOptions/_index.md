---
title: "Classe PdfSaveOptions"
linktitle: "PdfSaveOptions"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe PdfSaveOptions. Incapsula l'oggetto che rappresenta pdfsaveoptions in Go."
type: docs
weight: 200
url: /it/go-cpp/pdfsaveoptions/
---

## PdfSaveOptions class

Rappresenta le opzioni per il salvataggio del file pdf.

```go

type PdfSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewPdfSaveOptions](./newpdfsaveoptions/) | Crea le opzioni per il salvataggio del file PDF. |
| [NewPdfSaveOptions_PaginatedSaveOptions](./newpdfsaveoptions_paginatedsaveoptions/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetEmbedStandardWindowsFonts](./getembedstandardwindowsfonts/) | Vero per incorporare i font TrueType.Affetta solo i caratteri ASCII 32-127.I font per i codici carattere superiori a 127 sono sempre incorporati.I font sono sempre incorporati per lo standard PDF/A-1a, PDF/A-1b.Il valore predefinito è vero. |
| [SetEmbedStandardWindowsFonts](./setembedstandardwindowsfonts/) | Vero per incorporare i font TrueType.Affetta solo i caratteri ASCII 32-127.I font per i codici carattere superiori a 127 sono sempre incorporati.I font sono sempre incorporati per lo standard PDF/A-1a, PDF/A-1b.Il valore predefinito è vero. |
| [GetBookmark](./getbookmark/) | Ottiene e imposta l'oggetto PdfBookmarkEntry</see>. |
| [SetBookmark](./setbookmark/) | Ottiene e imposta l'oggetto PdfBookmarkEntry</see>. |
| [GetCompliance](./getcompliance/) | Ottiene o imposta il livello di conformità agli standard PDF per i documenti di output. |
| [SetCompliance](./setcompliance/) | Ottiene o imposta il livello di conformità agli standard PDF per i documenti di output. |
| [GetSecurityOptions](./getsecurityoptions/) | Imposta queste opzioni, quando è necessaria la sicurezza nel risultato xls2pdf. |
| [SetSecurityOptions](./setsecurityoptions/) | Imposta queste opzioni, quando è necessaria la sicurezza nel risultato xls2pdf. |
| [GetCalculateFormula](./getcalculateformula/) | Indica se calcolare le formule prima di salvare il file PDF. |
| [SetCalculateFormula](./setcalculateformula/) | Indica se calcolare le formule prima di salvare il file PDF. |
| [GetPdfCompression](./getpdfcompression/) | Indica l'algoritmo di compressione |
| [SetPdfCompression](./setpdfcompression/) | Indica l'algoritmo di compressione |
| [SetImageResample](./setimageresample/) | Imposta i PPI (pixel per pollice) desiderati per le immagini di ricampionamento e la qualità JPEG.Tutte le immagini saranno convertite in JPEG con l'impostazione di qualità specificata,e le immagini con PPI superiore a quello specificato (pixel per pollice) saranno ricampionate. |
| [GetCreatedTime](./getcreatedtime/) | Ottiene e imposta l'ora di generazione del documento PDF. |
| [SetCreatedTime](./setcreatedtime/) | Ottiene e imposta l'ora di generazione del documento PDF. |
| [GetProducer](./getproducer/) | Ottiene e imposta il produttore del documento PDF generato. |
| [SetProducer](./setproducer/) | Ottiene e imposta il produttore del documento PDF generato. |
| [GetOptimizationType](./getoptimizationtype/) | Ottiene e imposta il tipo di ottimizzazione PDF. |
| [SetOptimizationType](./setoptimizationtype/) | Ottiene e imposta il tipo di ottimizzazione PDF. |
| [GetCustomPropertiesExport](./getcustompropertiesexport/) | Ottiene o imposta un valore che determina il modo in cui CustomDocumentPropertyCollection vengono esportati nel file PDF. Il valore predefinito è Nessuno. |
| [SetCustomPropertiesExport](./setcustompropertiesexport/) | Ottiene o imposta un valore che determina il modo in cui CustomDocumentPropertyCollection vengono esportati nel file PDF. Il valore predefinito è Nessuno. |
| [GetExportDocumentStructure](./getexportdocumentstructure/) | Indica se esportare la struttura del documento. |
| [SetExportDocumentStructure](./setexportdocumentstructure/) | Indica se esportare la struttura del documento. |
| [GetDisplayDocTitle](./getdisplaydoctitle/) | Indica se la barra del titolo della finestra deve visualizzare il titolo del documento. |
| [SetDisplayDocTitle](./setdisplaydoctitle/) | Indica se la barra del titolo della finestra deve visualizzare il titolo del documento. |
| [GetFontEncoding](./getfontencoding/) | Ottiene o imposta la codifica dei font incorporati nel PDF. |
| [SetFontEncoding](./setfontencoding/) | Ottiene o imposta la codifica dei font incorporati nel PDF. |
| [GetWatermark](./getwatermark/) | Ottiene o imposta la filigrana per l'output. |
| [SetWatermark](./setwatermark/) | Ottiene o imposta la filigrana per l'output. |
| [GetEmbedAttachments](./getembedattachments/) | Indica se incorporare l'allegato per gli oggetti Ole in Excel. |
| [SetEmbedAttachments](./setembedattachments/) | Indica se incorporare l'allegato per gli oggetti Ole in Excel. |
| [GetZoomBehavior](./getzoombehavior/) | Ottiene o imposta la modalità di visualizzazione iniziale quando il documento PDF generato viene aperto. Il valore predefinito è PdfZoomBehavior.None. |
| [SetZoomBehavior](./setzoombehavior/) | Ottiene o imposta la modalità di visualizzazione iniziale quando il documento PDF generato viene aperto. Il valore predefinito è PdfZoomBehavior.None. |
| [GetZoomFactor](./getzoomfactor/) | Ottiene o imposta la percentuale di zoom utilizzata quandoZoomBehavior è PdfZoomBehavior.ZoomFactor. |
| [SetZoomFactor](./setzoomfactor/) | Ottiene o imposta la percentuale di zoom utilizzata quandoZoomBehavior è PdfZoomBehavior.ZoomFactor. |
| [GetDefaultFont](./getdefaultfont/) | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in PDF o immagine. Imposta il DefaultFont, ad esempio MingLiu o MS Gothic, per visualizzare questi caratteri. Se questa proprietà non è impostata, Aspose.Cells utilizzerà il font predefinito del sistema per mostrare questi caratteri Unicode. |
| [SetDefaultFont](./setdefaultfont/) | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in PDF o immagine. Imposta il DefaultFont, ad esempio MingLiu o MS Gothic, per visualizzare questi caratteri. Se questa proprietà non è impostata, Aspose.Cells utilizzerà il font predefinito del sistema per mostrare questi caratteri Unicode. |
| [GetCheckWorkbookDefaultFont](./getcheckworkbookdefaultfont/) | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in PDF o immagine. Imposta questo su true per provare a utilizzare prima il font predefinito della cartella di lavoro per visualizzare questi caratteri. |
| [SetCheckWorkbookDefaultFont](./setcheckworkbookdefaultfont/) | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in PDF o immagine. Imposta questo su true per provare a utilizzare prima il font predefinito della cartella di lavoro per visualizzare questi caratteri. |
| [SetCheckFontCompatibility](./setcheckfontcompatibility/) | Indica se verificare la compatibilità del font per ogni carattere nel testo. |
| [GetCheckFontCompatibility](./getcheckfontcompatibility/) | Indica se verificare la compatibilità del font per ogni carattere nel testo. |
| [SetIsFontSubstitutionCharGranularity](./setisfontsubstitutionchargranularity/) | Indica se sostituire il font del carattere solo quando il font della cella non è compatibile. |
| [IsFontSubstitutionCharGranularity](./isfontsubstitutionchargranularity/) | Indica se sostituire il font del carattere solo quando il font della cella non è compatibile. |
| [GetOnePagePerSheet](./getonepagepersheet/) | Se OnePagePerSheet è true, tutto il contenuto di un foglio verrà esportato in una sola pagina nel risultato. La dimensione della carta del pagesetup sarà invalida, ma le altre impostazioni del pagesetup continueranno ad avere effetto. |
| [SetOnePagePerSheet](./setonepagepersheet/) | Se OnePagePerSheet è true, tutto il contenuto di un foglio verrà esportato in una sola pagina nel risultato. La dimensione della carta del pagesetup sarà invalida, ma le altre impostazioni del pagesetup continueranno ad avere effetto. |
| [GetAllColumnsInOnePagePerSheet](./getallcolumnsinonepagepersheet/) | Se AllColumnsInOnePagePerSheet è true, tutto il contenuto delle colonne di un foglio verrà esportato in una sola pagina nel risultato. La larghezza della carta del pagesetup sarà ignorata, ma le altre impostazioni del pagesetup continueranno ad avere effetto. |
| [SetAllColumnsInOnePagePerSheet](./setallcolumnsinonepagepersheet/) | Se AllColumnsInOnePagePerSheet è true, tutto il contenuto delle colonne di un foglio verrà esportato in una sola pagina nel risultato. La larghezza della carta del pagesetup sarà ignorata, ma le altre impostazioni del pagesetup continueranno ad avere effetto. |
| [GetIgnoreError](./getignoreerror/) | Indica se è necessario nascondere l'errore durante il rendering. L'errore può riguardare forme, immagini, rendering di grafici, ecc. |
| [SetIgnoreError](./setignoreerror/) | Indica se è necessario nascondere l'errore durante il rendering. L'errore può riguardare forme, immagini, rendering di grafici, ecc. |
| [GetOutputBlankPageWhenNothingToPrint](./getoutputblankpagewhennothingtoprint/) | Indica se generare una pagina vuota quando non c'è nulla da stampare. |
| [SetOutputBlankPageWhenNothingToPrint](./setoutputblankpagewhennothingtoprint/) | Indica se generare una pagina vuota quando non c'è nulla da stampare. |
| [SetPageIndex](./setpageindex/) | Ottiene o imposta l'indice basato su zero della prima pagina da salvare. |
| [GetPageIndex](./getpageindex/) | Ottiene o imposta l'indice basato su zero della prima pagina da salvare. |
| [SetPageCount](./setpagecount/) | Ottiene o imposta il numero di pagine da salvare. |
| [GetPageCount](./getpagecount/) | Ottiene o imposta il numero di pagine da salvare. |
| [GetPrintingPageType](./getprintingpagetype/) | Indica quali pagine non verranno stampate. |
| [SetPrintingPageType](./setprintingpagetype/) | Indica quali pagine non verranno stampate. |
| [GetGridlineType](./getgridlinetype/) | Ottiene o imposta il tipo di linea della griglia. |
| [SetGridlineType](./setgridlinetype/) | Ottiene o imposta il tipo di linea della griglia. |
| [GetGridlineColor](./getgridlinecolor/) | Ottiene o imposta il colore della linea della griglia. |
| [SetGridlineColor](./setgridlinecolor/) | Ottiene o imposta il colore della linea della griglia. |
| [GetTextCrossType](./gettextcrosstype/) | Ottiene o imposta il tipo di visualizzazione del testo quando la larghezza del testo supera quella della cella. |
| [SetTextCrossType](./settextcrosstype/) | Ottiene o imposta il tipo di visualizzazione del testo quando la larghezza del testo supera quella della cella. |
| [GetDefaultEditLanguage](./getdefaulteditlanguage/) | Ottiene o imposta la lingua di modifica predefinita. |
| [SetDefaultEditLanguage](./setdefaulteditlanguage/) | Ottiene o imposta la lingua di modifica predefinita. |
| [GetSheetSet](./getsheetset/) | Ottiene o imposta i fogli da renderizzare. L'impostazione predefinita è tutti i fogli visibili nella cartella di lavoro: Aspose.Cells.Rendering.SheetSet.Visible. |
| [SetSheetSet](./setsheetset/) | Ottiene o imposta i fogli da renderizzare. L'impostazione predefinita è tutti i fogli visibili nella cartella di lavoro: Aspose.Cells.Rendering.SheetSet.Visible. |
| [GetDrawObjectEventHandler](./getdrawobjecteventhandler/) | Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering. |
| [SetDrawObjectEventHandler](./setdrawobjecteventhandler/) | Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering. |
| [GetEmfRenderSetting](./getemfrendersetting/) | Impostazione per il rendering del metafile Emf. |
| [SetEmfRenderSetting](./setemfrendersetting/) | Impostazione per il rendering del metafile Emf. |
| [GetCustomRenderSettings](./getcustomrendersettings/) | Ottiene o imposta le impostazioni personalizzate durante il rendering. |
| [SetCustomRenderSettings](./setcustomrendersettings/) | Ottiene o imposta le impostazioni personalizzate durante il rendering. |
| [GetRenderingBehavior](./getrenderingbehavior/) | Ottiene o imposta i comportamenti di rendering specifici per Excel da applicare. |
| [SetRenderingBehavior](./setrenderingbehavior/) | Ottiene o imposta i comportamenti di rendering specifici per Excel da applicare. |
| [GetSaveFormat](./getsaveformat/) | Ottiene il formato di salvataggio del file. |
| [GetClearData](./getcleardata/) | Rende la cartella di lavoro vuota dopo aver salvato il file. |
| [SetClearData](./setcleardata/) | Rende la cartella di lavoro vuota dopo aver salvato il file. |
| [GetCachedFileFolder](./getcachedfilefolder/) | La cartella per i file temporanei che possono essere usati come cache dei dati. |
| [SetCachedFileFolder](./setcachedfilefolder/) | La cartella per i file temporanei che possono essere usati come cache dei dati. |
| [GetValidateMergedAreas](./getvalidatemergedareas/) | Indica se convalidare le celle unite prima di salvare il file. |
| [SetValidateMergedAreas](./setvalidatemergedareas/) | Indica se convalidare le celle unite prima di salvare il file. |
| [GetMergeAreas](./getmergeareas/) | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. |
| [SetMergeAreas](./setmergeareas/) | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. |
| [GetCreateDirectory](./getcreatedirectory/) | Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. |
| [SetCreateDirectory](./setcreatedirectory/) | Se vero e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. |
| [GetSortNames](./getsortnames/) | Indica se ordinare i nomi definiti prima di salvare il file. |
| [SetSortNames](./setsortnames/) | Indica se ordinare i nomi definiti prima di salvare il file. |
| [GetSortExternalNames](./getsortexternalnames/) | Indica se ordinare i nomi definiti esterni prima di salvare il file. |
| [SetSortExternalNames](./setsortexternalnames/) | Indica se ordinare i nomi definiti esterni prima di salvare il file. |
| [GetRefreshChartCache](./getrefreshchartcache/) | Indica se memorizzare nella cache gli ultimi dati del grafico. |
| [SetRefreshChartCache](./setrefreshchartcache/) | Indica se memorizzare nella cache gli ultimi dati del grafico. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | Se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Per esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, verrà troncato. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | Se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Per esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, verrà troncato. |
| [GetUpdateSmartArt](./getupdatesmartart/) | Indica se aggiornare le impostazioni di SmartArt. Il valore predefinito è false. |
| [SetUpdateSmartArt](./setupdatesmartart/) | Indica se aggiornare le impostazioni di SmartArt. Il valore predefinito è false. |
| [GetEncryptDocumentProperties](./getencryptdocumentproperties/) | Indica se crittografare le proprietà del documento quando si salva come file .xls. Il valore predefinito è true. |
| [SetEncryptDocumentProperties](./setencryptdocumentproperties/) | Indica se crittografare le proprietà del documento quando si salva come file .xls. Il valore predefinito è true. |
