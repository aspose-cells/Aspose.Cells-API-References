---
title: "DocxSaveOptions Classe"
linktitle: "DocxSaveOptions"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "DocxSaveOptions classe. Incapsula l'oggetto che rappresenta docxsaveoptions in Go."
type: docs
weight: 200
url: /it/go-cpp/docxsaveoptions/
---

## DocxSaveOptions class

Rappresenta le opzioni per il salvataggio del file .docx.

```go

type DocxSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewDocxSaveOptions](./newdocxsaveoptions/) | Rappresenta le opzioni per il salvataggio del file .docx. |
| [NewDocxSaveOptions_Bool](./newdocxsaveoptions_bool/) | Rappresenta le opzioni per il salvataggio del file .docx. |
| [NewDocxSaveOptions_PaginatedSaveOptions](./newdocxsaveoptions_paginatedsaveoptions/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetSaveAsEditableShapes](./getsaveaseditableshapes/) | Salva tutti gli oggetti di disegno come forme modificabili nel file Word, così puoi modificarli in Word. |
| [SetSaveAsEditableShapes](./setsaveaseditableshapes/) | Salva tutti gli oggetti di disegno come forme modificabili nel file Word, così puoi modificarli in Word. |
| [GetEmbedXlsxAsChartDataSource](./getembedxlsxaschartdatasource/) | Indica se incorporare un file xlsx come origine dati del grafico. |
| [SetEmbedXlsxAsChartDataSource](./setembedxlsxaschartdatasource/) | Indica se incorporare un file xlsx come origine dati del grafico. |
| [GetAsFlatOpc](./getasflatopc/) | Indica se salvare come file OPC piatto che può essere generato da Open XML SDK |
| [SetAsFlatOpc](./setasflatopc/) | Indica se salvare come file OPC piatto che può essere generato da Open XML SDK |
| [GetSaveElementType](./getsaveelementtype/) | Indica quali elementi devono essere salvati. |
| [SetSaveElementType](./setsaveelementtype/) | Indica quali elementi devono essere salvati. |
| [GetAsNormalView](./getasnormalview/) | Esportazione del file Excel in file docx in visualizzazione normale. Se questa proprietà è true, verrà generata un'Area e nessuna scala avrà effetto. Il valore predefinito è false. |
| [SetAsNormalView](./setasnormalview/) | Esportazione del file Excel in file docx in visualizzazione normale. Se questa proprietà è true, verrà generata un'Area e nessuna scala avrà effetto. Il valore predefinito è false. |
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
