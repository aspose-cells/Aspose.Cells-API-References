---
title: "HtmlSaveOptions Classe"
linktitle: "HtmlSaveOptions"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "HtmlSaveOptions classe. Incapsula l'oggetto che rappresenta htmlsaveoptions in Go."
type: docs
weight: 200
url: /it/go-cpp/htmlsaveoptions/
---

## HtmlSaveOptions class

Rappresenta le opzioni per salvare il file HTML.

```go

type HtmlSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewHtmlSaveOptions](./newhtmlsaveoptions/) | Crea opzioni per salvare il file html. |
| [NewHtmlSaveOptions_SaveFormat](./newhtmlsaveoptions_saveformat/) | Crea opzioni per salvare il file htm. |
| [NewHtmlSaveOptions_SaveOptions](./newhtmlsaveoptions_saveoptions/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetIgnoreInvisibleShapes](./getignoreinvisibleshapes/) | Indica se esportare le forme non visibili |
| [SetIgnoreInvisibleShapes](./setignoreinvisibleshapes/) | Indica se esportare le forme non visibili |
| [GetPageTitle](./getpagetitle/) | Il titolo della pagina html. Solo per il salvataggio in un flusso html. |
| [SetPageTitle](./setpagetitle/) | Il titolo della pagina html. Solo per il salvataggio in un flusso html. |
| [GetAttachedFilesDirectory](./getattachedfilesdirectory/) | La directory in cui verranno salvati i file allegati. Solo per il salvataggio in un flusso html. |
| [SetAttachedFilesDirectory](./setattachedfilesdirectory/) | La directory in cui verranno salvati i file allegati. Solo per il salvataggio in un flusso html. |
| [GetAttachedFilesUrlPrefix](./getattachedfilesurlprefix/) | Specifica il prefisso Url dei file allegati, come le immagini, nel file html. Solo per il salvataggio in un flusso html. |
| [SetAttachedFilesUrlPrefix](./setattachedfilesurlprefix/) | Specifica il prefisso Url dei file allegati, come le immagini, nel file html. Solo per il salvataggio in un flusso html. |
| [GetDefaultFontName](./getdefaultfontname/) | Specifica il nome del font predefinito per l'esportazione html; il font predefinito verrà usato quando il font dello stile non esiste. Se questa proprietà è null, Aspose.Cells utilizzerà un font universale che ha la stessa famiglia del font originale; il valore predefinito è null. |
| [SetDefaultFontName](./setdefaultfontname/) | Specifica il nome del font predefinito per l'esportazione html; il font predefinito verrà usato quando il font dello stile non esiste. Se questa proprietà è null, Aspose.Cells utilizzerà un font universale che ha la stessa famiglia del font originale; il valore predefinito è null. |
| [GetAddGenericFont](./getaddgenericfont/) | Indica se aggiungere un font generico alla proprietà CSS font-family. Il valore predefinito è true |
| [SetAddGenericFont](./setaddgenericfont/) | Indica se aggiungere un font generico alla proprietà CSS font-family. Il valore predefinito è true |
| [GetWorksheetScalable](./getworksheetscalable/) | Indica se ingrandire o ridurre l'html tramite il livello di zoom del foglio di lavoro durante il salvataggio del file in html, il valore predefinito è false. |
| [SetWorksheetScalable](./setworksheetscalable/) | Indica se ingrandire o ridurre l'html tramite il livello di zoom del foglio di lavoro durante il salvataggio del file in html, il valore predefinito è false. |
| [IsExportComments](./isexportcomments/) | Indica se esportare i commenti durante il salvataggio del file in html, il valore predefinito è false. |
| [SetIsExportComments](./setisexportcomments/) | Indica se esportare i commenti durante il salvataggio del file in html, il valore predefinito è false. |
| [GetExportCommentsType](./getexportcommentstype/) | Rappresenta il tipo di esportazione dei commenti nei file html. |
| [SetExportCommentsType](./setexportcommentstype/) | Rappresenta il tipo di esportazione dei commenti nei file html. |
| [GetDisableDownlevelRevealedComments](./getdisabledownlevelrevealedcomments/) | Indica se disabilitare i commenti condizionali Downlevel-revealed durante l'esportazione del file in html, il valore predefinito è false. |
| [SetDisableDownlevelRevealedComments](./setdisabledownlevelrevealedcomments/) | Indica se disabilitare i commenti condizionali Downlevel-revealed durante l'esportazione del file in html, il valore predefinito è false. |
| [IsExpImageToTempDir](./isexpimagetotempdir/) | Indica se esportare i file immagine in una directory temporanea. Solo per il salvataggio in uno stream html. |
| [SetIsExpImageToTempDir](./setisexpimagetotempdir/) | Indica se esportare i file immagine in una directory temporanea. Solo per il salvataggio in uno stream html. |
| [GetImageScalable](./getimagescalable/) | Indica se utilizzare unità scalabili per descrivere la larghezza dell'immagine quando si utilizza un'unità scalabile per descrivere la larghezza della colonna. Il valore predefinito è true. |
| [SetImageScalable](./setimagescalable/) | Indica se utilizzare unità scalabili per descrivere la larghezza dell'immagine quando si utilizza un'unità scalabile per descrivere la larghezza della colonna. Il valore predefinito è true. |
| [GetWidthScalable](./getwidthscalable/) | Indica se esportare la larghezza della colonna in unità di scala in html. Il valore predefinito è false. |
| [SetWidthScalable](./setwidthscalable/) | Indica se esportare la larghezza della colonna in unità di scala in html. Il valore predefinito è false. |
| [GetExportSingleTab](./getexportsingletab/) | Indica se esportare la singola scheda quando il file contiene un solo foglio di lavoro. Il valore predefinito è false. |
| [SetExportSingleTab](./setexportsingletab/) | Indica se esportare la singola scheda quando il file contiene un solo foglio di lavoro. Il valore predefinito è false. |
| [GetExportImagesAsBase64](./getexportimagesasbase64/) | Specifica se le immagini vengono salvate in formato Base64 in HTML, MHTML o EPUB. |
| [SetExportImagesAsBase64](./setexportimagesasbase64/) | Specifica se le immagini vengono salvate in formato Base64 in HTML, MHTML o EPUB. |
| [GetExportActiveWorksheetOnly](./getexportactiveworksheetonly/) | Indica se esportare solo il foglio di lavoro attivo in un file html. Se true, verrà esportato solo il foglio di lavoro attivo; se false, verrà esportata l'intera cartella di lavoro. Il valore predefinito è false. |
| [SetExportActiveWorksheetOnly](./setexportactiveworksheetonly/) | Indica se esportare solo il foglio di lavoro attivo in un file html. Se true, verrà esportato solo il foglio di lavoro attivo; se false, verrà esportata l'intera cartella di lavoro. Il valore predefinito è false. |
| [GetExportPrintAreaOnly](./getexportprintareaonly/) | Indica se esportare solo l'area di stampa in un file html. Il valore predefinito è false. |
| [SetExportPrintAreaOnly](./setexportprintareaonly/) | Indica se esportare solo l'area di stampa in un file html. Il valore predefinito è false. |
| [GetExportArea](./getexportarea/) | Ottiene o imposta l'area di cella da esportare del foglio di lavoro attivo corrente. Se imposti questo attributo, l'area di stampa del foglio di lavoro attivo corrente verrà omessa. Solo l'area specificata verrà esportata durante il salvataggio del file in html. |
| [SetExportArea](./setexportarea/) | Ottiene o imposta l'area di cella da esportare del foglio di lavoro attivo corrente. Se imposti questo attributo, l'area di stampa del foglio di lavoro attivo corrente verrà omessa. Solo l'area specificata verrà esportata durante il salvataggio del file in html. |
| [GetParseHtmlTagInCell](./getparsehtmltagincell/) | Indica se i tag html (come <c>&lt;div&gt;&lt;/div&gt;</c>) nella cella devono essere analizzati come valore della cella o preservati così come sono. Il valore predefinito è true. |
| [SetParseHtmlTagInCell](./setparsehtmltagincell/) | Indica se i tag html (come <c>&lt;div&gt;&lt;/div&gt;</c>) nella cella devono essere analizzati come valore della cella o preservati così come sono. Il valore predefinito è true. |
| [GetHtmlCrossStringType](./gethtmlcrossstringtype/) | Indica se una stringa che attraversa più celle verrà visualizzata nello stesso modo di MS Excel quando si salva un file Excel in formato html. Per impostazione predefinita il valore è Default, quindi per le stringhe che attraversano più celle c'è poca differenza tra i file html creati da Aspose.Cells e MS Excel. Tuttavia, per le prestazioni nella creazione di file html di grandi dimensioni, impostare il valore su Cross sarebbe diverse volte più veloce rispetto a impostarlo su Default o Fit2Cell. |
| [SetHtmlCrossStringType](./sethtmlcrossstringtype/) | Indica se una stringa che attraversa più celle verrà visualizzata nello stesso modo di MS Excel quando si salva un file Excel in formato html. Per impostazione predefinita il valore è Default, quindi per le stringhe che attraversano più celle c'è poca differenza tra i file html creati da Aspose.Cells e MS Excel. Tuttavia, per le prestazioni nella creazione di file html di grandi dimensioni, impostare il valore su Cross sarebbe diverse volte più veloce rispetto a impostarlo su Default o Fit2Cell. |
| [GetHiddenColDisplayType](./gethiddencoldisplaytype/) | Colonna nascosta (la larghezza di questa colonna è 0) in Excel, prima di salvarla in formato html, se HtmlHiddenColDisplayType è "Remove", la colonna nascosta non verrà emessa; se il valore è "Hidden", la colonna verrà emessa ma rimarrà nascosta. Il valore predefinito è "Hidden". |
| [SetHiddenColDisplayType](./sethiddencoldisplaytype/) | Colonna nascosta (la larghezza di questa colonna è 0) in Excel, prima di salvarla in formato html, se HtmlHiddenColDisplayType è "Remove", la colonna nascosta non verrà emessa; se il valore è "Hidden", la colonna verrà emessa ma rimarrà nascosta. Il valore predefinito è "Hidden". |
| [GetHiddenRowDisplayType](./gethiddenrowdisplaytype/) | Riga nascosta (l'altezza di questa riga è 0) in Excel, prima di salvarla in formato html, se HtmlHiddenRowDisplayType è "Remove", la riga nascosta non verrà emessa; se il valore è "Hidden", la riga verrà emessa ma rimarrà nascosta. Il valore predefinito è "Hidden". |
| [SetHiddenRowDisplayType](./sethiddenrowdisplaytype/) | Riga nascosta (l'altezza di questa riga è 0) in Excel, prima di salvarla in formato html, se HtmlHiddenRowDisplayType è "Remove", la riga nascosta non verrà emessa; se il valore è "Hidden", la riga verrà emessa ma rimarrà nascosta. Il valore predefinito è "Hidden". |
| [GetEncoding](./getencoding/) | Se non impostato, utilizza Encoding.UTF8 come tipo di codifica predefinito. |
| [SetEncoding](./setencoding/) | Se non impostato, utilizza Encoding.UTF8 come tipo di codifica predefinito. |
| [GetImageOptions](./getimageoptions/) | Ottieni l'oggetto ImageOrPrintOptions prima dell'esportazione. |
| [GetSaveAsSingleFile](./getsaveassinglefile/) | Indica se salvare l'html come file unico. Il valore predefinito è false. |
| [SetSaveAsSingleFile](./setsaveassinglefile/) | Indica se salvare l'html come file unico. Il valore predefinito è false. |
| [GetShowAllSheets](./getshowallsheets/) | Indica se mostrare tutti i fogli durante il salvataggio come file html unico. |
| [SetShowAllSheets](./setshowallsheets/) | Indica se mostrare tutti i fogli durante il salvataggio come file html unico. |
| [GetExportPageHeaders](./getexportpageheaders/) | Indica se esportare le intestazioni di pagina. |
| [SetExportPageHeaders](./setexportpageheaders/) | Indica se esportare le intestazioni di pagina. |
| [GetExportPageFooters](./getexportpagefooters/) | Indica se esportare le intestazioni di pagina. |
| [SetExportPageFooters](./setexportpagefooters/) | Indica se esportare le intestazioni di pagina. |
| [GetExportHiddenWorksheet](./getexporthiddenworksheet/) | Indica se esportare il contenuto dei fogli di lavoro nascosti. Il valore predefinito è true. |
| [SetExportHiddenWorksheet](./setexporthiddenworksheet/) | Indica se esportare il contenuto dei fogli di lavoro nascosti. Il valore predefinito è true. |
| [GetPresentationPreference](./getpresentationpreference/) | Indica se il file html o mht è la preferenza di presentazione. Il valore predefinito è false. Se desideri una presentazione più bella, imposta il valore su true. |
| [SetPresentationPreference](./setpresentationpreference/) | Indica se il file html o mht è la preferenza di presentazione. Il valore predefinito è false. Se desideri una presentazione più bella, imposta il valore su true. |
| [GetCellCssPrefix](./getcellcssprefix/) | Ottiene e imposta il prefisso del nome css, il valore predefinito è "". |
| [SetCellCssPrefix](./setcellcssprefix/) | Ottiene e imposta il prefisso del nome css, il valore predefinito è "". |
| [GetTableCssId](./gettablecssid/) | Ottiene e imposta il prefisso del nome css di tipo, come tr, col, td e così via, contenuti nell'elemento table che ha l'attributo specifico TableCssId. Il valore predefinito è "". |
| [SetTableCssId](./settablecssid/) | Ottiene e imposta il prefisso del nome css di tipo, come tr, col, td e così via, contenuti nell'elemento table che ha l'attributo specifico TableCssId. Il valore predefinito è "". |
| [IsFullPathLink](./isfullpathlink/) | Indica se utilizzare il collegamento con percorso completo in sheet00x.htm, filelist.xml e tabstrip.htm. Il valore predefinito è false. |
| [SetIsFullPathLink](./setisfullpathlink/) | Indica se utilizzare il collegamento con percorso completo in sheet00x.htm, filelist.xml e tabstrip.htm. Il valore predefinito è false. |
| [GetExportWorksheetCSSSeparately](./getexportworksheetcssseparately/) | Indica se esportare il CSS del foglio di lavoro separatamente. Il valore predefinito è false. |
| [SetExportWorksheetCSSSeparately](./setexportworksheetcssseparately/) | Indica se esportare il CSS del foglio di lavoro separatamente. Il valore predefinito è false. |
| [GetExportSimilarBorderStyle](./getexportsimilarborderstyle/) | Indica se esportare lo stile di bordo simile quando lo stile di bordo non è supportato dai browser. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito. Il valore predefinito è false. |
| [SetExportSimilarBorderStyle](./setexportsimilarborderstyle/) | Indica se esportare lo stile di bordo simile quando lo stile di bordo non è supportato dai browser. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito. Il valore predefinito è false. |
| [GetMergeEmptyTdType](./getmergeemptytdtype/) | L'opzione per unire celle vuote contigue (elementi td vuoti). Il valore predefinito è MergeEmptyTdType.Default. |
| [SetMergeEmptyTdType](./setmergeemptytdtype/) | L'opzione per unire celle vuote contigue (elementi td vuoti). Il valore predefinito è MergeEmptyTdType.Default. |
| [GetExportCellCoordinate](./getexportcellcoordinate/) | Indica se esportare le coordinate Excel delle celle non vuote durante il salvataggio del file in html. Il valore predefinito è false. Se desideri importare l'html generato in Excel, mantieni il valore predefinito. |
| [SetExportCellCoordinate](./setexportcellcoordinate/) | Indica se esportare le coordinate Excel delle celle non vuote durante il salvataggio del file in html. Il valore predefinito è false. Se desideri importare l'html generato in Excel, mantieni il valore predefinito. |
| [GetExportExtraHeadings](./getexportextraheadings/) | Indica se esportare intestazioni extra quando la lunghezza del testo supera la colonna di visualizzazione massima. Il valore predefinito è false. Se desideri importare il file html in Excel, mantieni il valore predefinito. |
| [SetExportExtraHeadings](./setexportextraheadings/) | Indica se esportare intestazioni extra quando la lunghezza del testo supera la colonna di visualizzazione massima. Il valore predefinito è false. Se desideri importare il file html in Excel, mantieni il valore predefinito. |
| [GetExportRowColumnHeadings](./getexportrowcolumnheadings/) | Indica se esportare le intestazioni di righe e colonne del foglio durante il salvataggio in file HTML. |
| [SetExportRowColumnHeadings](./setexportrowcolumnheadings/) | Indica se esportare le intestazioni di righe e colonne del foglio durante il salvataggio in file HTML. |
| [GetExportFormula](./getexportformula/) | Indica se esportare le formule durante il salvataggio del file in html. Il valore predefinito è true. Se desideri importare l'html generato in Excel, mantieni il valore predefinito. |
| [SetExportFormula](./setexportformula/) | Indica se esportare le formule durante il salvataggio del file in html. Il valore predefinito è true. Se desideri importare l'html generato in Excel, mantieni il valore predefinito. |
| [GetAddTooltipText](./getaddtooltiptext/) | Indica se aggiungere il testo del tooltip quando i dati non possono essere visualizzati completamente. Il valore predefinito è false. |
| [SetAddTooltipText](./setaddtooltiptext/) | Indica se aggiungere il testo del tooltip quando i dati non possono essere visualizzati completamente. Il valore predefinito è false. |
| [GetExportGridLines](./getexportgridlines/) | Indica se esportare le linee della griglia. Il valore predefinito è false. |
| [SetExportGridLines](./setexportgridlines/) | Indica se esportare le linee della griglia. Il valore predefinito è false. |
| [GetExportBogusRowData](./getexportbogusrowdata/) | Indica se esportare dati falsi dell'ultima riga. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito. |
| [SetExportBogusRowData](./setexportbogusrowdata/) | Indica se esportare dati falsi dell'ultima riga. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito. |
| [GetExcludeUnusedStyles](./getexcludeunusedstyles/) | Indica se escludere gli stili non utilizzati. Per i file html generati, l'esclusione degli stili inutilizzati può ridurre la dimensione del file senza influire sugli effetti visivi. Pertanto il valore predefinito di questa proprietà è true. Se l'utente deve mantenere tutti gli stili nella cartella di lavoro per l'html generato (ad esempio nello scenario in cui l'utente deve ripristinare la cartella di lavoro dall'html generato in seguito), impostare questa proprietà su false. |
| [SetExcludeUnusedStyles](./setexcludeunusedstyles/) | Indica se escludere gli stili non utilizzati. Per i file html generati, l'esclusione degli stili inutilizzati può ridurre la dimensione del file senza influire sugli effetti visivi. Pertanto il valore predefinito di questa proprietà è true. Se l'utente deve mantenere tutti gli stili nella cartella di lavoro per l'html generato (ad esempio nello scenario in cui l'utente deve ripristinare la cartella di lavoro dall'html generato in seguito), impostare questa proprietà su false. |
| [GetExportDocumentProperties](./getexportdocumentproperties/) | Indica se esportare le proprietà del documento. Il valore predefinito è true. Se desideri importare l'html o il file mht in Excel, mantieni il valore predefinito. |
| [SetExportDocumentProperties](./setexportdocumentproperties/) | Indica se esportare le proprietà del documento. Il valore predefinito è true. Se desideri importare l'html o il file mht in Excel, mantieni il valore predefinito. |
| [GetExportWorksheetProperties](./getexportworksheetproperties/) | Indica se esportare le proprietà del foglio di lavoro. Il valore predefinito è true. Se desideri importare l'html o il file mht in Excel, mantieni il valore predefinito. |
| [SetExportWorksheetProperties](./setexportworksheetproperties/) | Indica se esportare le proprietà del foglio di lavoro. Il valore predefinito è true. Se desideri importare l'html o il file mht in Excel, mantieni il valore predefinito. |
| [GetExportWorkbookProperties](./getexportworkbookproperties/) | Indica se esportare le proprietà della cartella di lavoro. Il valore predefinito è true. Se desideri importare l'html o il file mht in Excel, mantieni il valore predefinito. |
| [SetExportWorkbookProperties](./setexportworkbookproperties/) | Indica se esportare le proprietà della cartella di lavoro. Il valore predefinito è true. Se desideri importare l'html o il file mht in Excel, mantieni il valore predefinito. |
| [GetExportFrameScriptsAndProperties](./getexportframescriptsandproperties/) | Indica se esportare gli script del frame e le proprietà del documento. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito. |
| [SetExportFrameScriptsAndProperties](./setexportframescriptsandproperties/) | Indica se esportare gli script del frame e le proprietà del documento. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito. |
| [GetExportDataOptions](./getexportdataoptions/) | Indica la regola per l'esportazione dei dati del file html. Il valore predefinito è All. |
| [SetExportDataOptions](./setexportdataoptions/) | Indica la regola per l'esportazione dei dati del file html. Il valore predefinito è All. |
| [GetLinkTargetType](./getlinktargettype/) | Indica il tipo di attributo target nel collegamento <c>&lt;a&gt;</c>. Il valore predefinito è HtmlLinkTargetType.Parent. |
| [SetLinkTargetType](./setlinktargettype/) | Indica il tipo di attributo target nel collegamento <c>&lt;a&gt;</c>. Il valore predefinito è HtmlLinkTargetType.Parent. |
| [IsIECompatible](./isiecompatible/) | Indica se l'HTML di output è compatibile con il browser IE. Il valore predefinito è false |
| [SetIsIECompatible](./setisiecompatible/) | Indica se l'HTML di output è compatibile con il browser IE. Il valore predefinito è false |
| [GetFormatDataIgnoreColumnWidth](./getformatdataignorecolumnwidth/) | Indica se mostrare tutti i dati formattati della cella quando supera la larghezza della colonna. Se true, la larghezza della colonna viene ignorata e tutti i dati della cella verranno esportati. Se false, i dati verranno esportati come in Excel. Il valore predefinito è false. |
| [SetFormatDataIgnoreColumnWidth](./setformatdataignorecolumnwidth/) | Indica se mostrare tutti i dati formattati della cella quando supera la larghezza della colonna. Se true, la larghezza della colonna viene ignorata e tutti i dati della cella verranno esportati. Se false, i dati verranno esportati come in Excel. Il valore predefinito è false. |
| [GetCalculateFormula](./getcalculateformula/) | Indica se calcolare le formule prima di salvare il file html. |
| [SetCalculateFormula](./setcalculateformula/) | Indica se calcolare le formule prima di salvare il file html. |
| [IsJsBrowserCompatible](./isjsbrowsercompatible/) | Indica se JavaScript è compatibile con i browser che non supportano JavaScript. Il valore predefinito è true. |
| [SetIsJsBrowserCompatible](./setisjsbrowsercompatible/) | Indica se JavaScript è compatibile con i browser che non supportano JavaScript. Il valore predefinito è true. |
| [IsMobileCompatible](./ismobilecompatible/) | Indica se l'HTML di output è compatibile con i dispositivi mobili. Il valore predefinito è false. |
| [SetIsMobileCompatible](./setismobilecompatible/) | Indica se l'HTML di output è compatibile con i dispositivi mobili. Il valore predefinito è false. |
| [GetCssStyles](./getcssstyles/) | Ottiene o imposta gli stili CSS aggiuntivi per il formattatore. Funziona solo quando SaveAsSingleFile è True. |
| [SetCssStyles](./setcssstyles/) | Ottiene o imposta gli stili CSS aggiuntivi per il formattatore. Funziona solo quando SaveAsSingleFile è True. |
| [GetHideOverflowWrappedText](./gethideoverflowwrappedtext/) | Indica se nascondere il testo in overflow quando il formato della cella è impostato su a capo automatico. Il valore predefinito è false |
| [SetHideOverflowWrappedText](./sethideoverflowwrappedtext/) | Indica se nascondere il testo in overflow quando il formato della cella è impostato su a capo automatico. Il valore predefinito è false |
| [IsBorderCollapsed](./isbordercollapsed/) | Indica se i bordi della tabella sono compressi. Il valore predefinito è true. |
| [SetIsBorderCollapsed](./setisbordercollapsed/) | Indica se i bordi della tabella sono compressi. Il valore predefinito è true. |
| [GetEncodeEntityAsCode](./getencodeentityascode/) | Indica se le entità dei caratteri HTML vengono sostituite con il codice decimale. (ad es. "&amp;nbsp;" viene sostituita con "&amp;#160;"). Il valore predefinito è false. |
| [SetEncodeEntityAsCode](./setencodeentityascode/) | Indica se le entità dei caratteri HTML vengono sostituite con il codice decimale. (ad es. "&amp;nbsp;" viene sostituita con "&amp;#160;"). Il valore predefinito è false. |
| [GetOfficeMathOutputMode](./getofficemathoutputmode/) | Indica come gli oggetti OfficeMath vengono esportati in HTML. Il valore predefinito è Image. |
| [SetOfficeMathOutputMode](./setofficemathoutputmode/) | Indica come gli oggetti OfficeMath vengono esportati in HTML. Il valore predefinito è Image. |
| [GetCellNameAttribute](./getcellnameattribute/) | Specifica l'attributo che indica il CellName da scrivere. (ad es. Se il valore è "id", allora per la cella "A1", l'output sarà:&lt;td id='A1'&gt;). Il valore predefinito è null. |
| [SetCellNameAttribute](./setcellnameattribute/) | Specifica l'attributo che indica il CellName da scrivere. (ad es. Se il valore è "id", allora per la cella "A1", l'output sarà:&lt;td id='A1'&gt;). Il valore predefinito è null. |
| [GetDisableCss](./getdisablecss/) | Indica se vengono applicati solo gli stili inline, senza fare affidamento su CSS. Il valore predefinito è false. |
| [SetDisableCss](./setdisablecss/) | Indica se vengono applicati solo gli stili inline, senza fare affidamento su CSS. Il valore predefinito è false. |
| [GetEnableCssCustomProperties](./getenablecsscustomproperties/) | Ottimizza l'output di html utilizzando le proprietà personalizzate CSS. Ad esempio, nello scenario in cui ci sono più occorrenze della stessa immagine base64, con la proprietà personalizzata i dati dell'immagine devono essere salvati una sola volta, così le prestazioni dell'html risultante possono essere migliorate. Il valore predefinito è false. |
| [SetEnableCssCustomProperties](./setenablecsscustomproperties/) | Ottimizza l'output di html utilizzando le proprietà personalizzate CSS. Ad esempio, nello scenario in cui ci sono più occorrenze della stessa immagine base64, con la proprietà personalizzata i dati dell'immagine devono essere salvati una sola volta, così le prestazioni dell'html risultante possono essere migliorate. Il valore predefinito è false. |
| [GetHtmlVersion](./gethtmlversion/) | Specifica la versione dello standard HTML da utilizzare durante il salvataggio del formato HTML. Il valore predefinito è HtmlVersion.Default. |
| [SetHtmlVersion](./sethtmlversion/) | Specifica la versione dello standard HTML da utilizzare durante il salvataggio del formato HTML. Il valore predefinito è HtmlVersion.Default. |
| [GetSheetSet](./getsheetset/) | Ottiene o imposta i fogli da renderizzare. L'impostazione predefinita è tutti i fogli visibili nella cartella di lavoro: Aspose.Cells.Rendering.SheetSet.Visible. |
| [SetSheetSet](./setsheetset/) | Ottiene o imposta i fogli da renderizzare. L'impostazione predefinita è tutti i fogli visibili nella cartella di lavoro: Aspose.Cells.Rendering.SheetSet.Visible. |
| [GetLayoutMode](./getlayoutmode/) | Ottiene o imposta la modalità di layout durante il salvataggio in HTML. Il valore predefinito è HtmlLayoutMode.Normal |
| [SetLayoutMode](./setlayoutmode/) | Ottiene o imposta la modalità di layout durante il salvataggio in HTML. Il valore predefinito è HtmlLayoutMode.Normal |
| [GetEmbeddedFontType](./getembeddedfonttype/) | Ottiene o imposta il tipo di incorporamento del file di carattere nel file html. Il valore predefinito è HtmlEmbeddedFontType.None, che indica che nessun carattere sarà incorporato in html. |
| [SetEmbeddedFontType](./setembeddedfonttype/) | Ottiene o imposta il tipo di incorporamento del file di carattere nel file html. Il valore predefinito è HtmlEmbeddedFontType.None, che indica che nessun carattere sarà incorporato in html. |
| [GetExportNamedRangeAnchors](./getexportnamedrangeanchors/) | Indica se esportare gli elementi anchor per gli intervalli denominati durante il salvataggio come HTML. Il valore predefinito è true. |
| [SetExportNamedRangeAnchors](./setexportnamedrangeanchors/) | Indica se esportare gli elementi anchor per gli intervalli denominati durante il salvataggio come HTML. Il valore predefinito è true. |
| [GetDataBarRenderMode](./getdatabarrendermode/) | Rappresenta la modalità di rendering di DataBar durante la conversione di file Excel in file html. Il valore predefinito è DataBarRenderMode.BackgroundColor. |
| [SetDataBarRenderMode](./setdatabarrendermode/) | Rappresenta la modalità di rendering di DataBar durante la conversione di file Excel in file html. Il valore predefinito è DataBarRenderMode.BackgroundColor. |
| [GetSpaceMode](./getspacemode/) | Indica come gli spazi vengono renderizzati nell'output HTML. Questa opzione è attualmente applicata solo ai formati numerici (ad es. formato contabile). Il valore predefinito è HtmlSpaceMode.Css. |
| [SetSpaceMode](./setspacemode/) | Indica come gli spazi vengono renderizzati nell'output HTML. Questa opzione è attualmente applicata solo ai formati numerici (ad es. formato contabile). Il valore predefinito è HtmlSpaceMode.Css. |
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
