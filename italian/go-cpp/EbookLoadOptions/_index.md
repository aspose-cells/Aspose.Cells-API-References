---
title: "EbookLoadOptions Classe"
linktitle: "EbookLoadOptions"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "EbookLoadOptions classe. Incapsula l'oggetto che rappresenta ebookloadoptions in Go."
type: docs
weight: 200
url: /it/go-cpp/ebookloadoptions/
---

## EbookLoadOptions class

Rappresenta le opzioni durante l'importazione di un file ebook.

```go

type EbookLoadOptions struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewEbookLoadOptions](./newebookloadoptions/) | Crea un'opzione per caricare il file ebook. |
| [NewEbookLoadOptions_LoadFormat](./newebookloadoptions_loadformat/) | Crea un'opzione di caricamento del file ebook. |
| [NewEbookLoadOptions_HtmlLoadOptions](./newebookloadoptions_htmlloadoptions/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetEncoding](./getencoding/) | Ottiene e imposta la codifica predefinita. Si applica solo ai file csv. |
| [SetEncoding](./setencoding/) | Ottiene e imposta la codifica predefinita. Si applica solo ai file csv. |
| [GetLoadStyleStrategy](./getloadstylestrategy/) | Indica la strategia per applicare lo stile ai valori analizzati quando si converte una stringa in numero o data/ora. |
| [SetLoadStyleStrategy](./setloadstylestrategy/) | Indica la strategia per applicare lo stile ai valori analizzati quando si converte una stringa in numero o data/ora. |
| [GetConvertNumericData](./getconvertnumericdata/) | Ottiene o imposta un valore che indica se la stringa nel file di testo è convertita in dati numerici. Il valore predefinito è true. |
| [SetConvertNumericData](./setconvertnumericdata/) | Ottiene o imposta un valore che indica se la stringa nel file di testo è convertita in dati numerici. Il valore predefinito è true. |
| [GetConvertDateTimeData](./getconvertdatetimedata/) | Ottiene o imposta un valore che indica se la stringa nel file di testo è convertita in dati di data. Il valore predefinito è true. |
| [SetConvertDateTimeData](./setconvertdatetimedata/) | Ottiene o imposta un valore che indica se la stringa nel file di testo è convertita in dati di data. Il valore predefinito è true. |
| [GetKeepPrecision](./getkeepprecision/) | Indica se non analizzare un valore stringa se la lunghezza è 15. |
| [SetKeepPrecision](./setkeepprecision/) | Indica se non analizzare un valore stringa se la lunghezza è 15. |
| [GetLoadFormulas](./getloadformulas/) | Indica se importare le formule se il file HTML originale contiene formule |
| [SetLoadFormulas](./setloadformulas/) | Indica se importare le formule se il file HTML originale contiene formule |
| [GetSupportDivTag](./getsupportdivtag/) | Indica se supportare il layout del tag <c>&lt;div&gt;</c> quando il file HTML lo contiene. Il valore predefinito è false. |
| [SetSupportDivTag](./setsupportdivtag/) | Indica se supportare il layout del tag <c>&lt;div&gt;</c> quando il file HTML lo contiene. Il valore predefinito è false. |
| [GetDeleteRedundantSpaces](./getdeleteredundantspaces/) | Indica se eliminare gli spazi ridondanti quando il testo va a capo usando il tag <c>&lt;br&gt;</c>. Il valore predefinito è false. |
| [SetDeleteRedundantSpaces](./setdeleteredundantspaces/) | Indica se eliminare gli spazi ridondanti quando il testo va a capo usando il tag <c>&lt;br&gt;</c>. Il valore predefinito è false. |
| [GetAutoFitColsAndRows](./getautofitcolsandrows/) | Indica se adattare automaticamente colonne e righe. Il valore predefinito è false. |
| [SetAutoFitColsAndRows](./setautofitcolsandrows/) | Indica se adattare automaticamente colonne e righe. Il valore predefinito è false. |
| [GetHasFormula](./gethasformula/) | Indica se il testo è una formula se inizia con "=", |
| [SetHasFormula](./sethasformula/) | Indica se il testo è una formula se inizia con "=", |
| [GetProgId](./getprogid/) | Ottiene l'ID del programma che crea il file. Solo per file MHT. |
| [GetTableLoadOptions](./gettableloadoptions/) | Ottieni l'istanza di HtmlTableLoadOptionCollection |
| [GetDetectLaTeX](./getdetectlatex/) | Indica se rilevare formule LaTeX nel file HTML. Il valore predefinito è false. |
| [SetDetectLaTeX](./setdetectlatex/) | Indica se rilevare formule LaTeX nel file HTML. Il valore predefinito è false. |
| [GetParagraphLayoutMode](./getparagraphlayoutmode/) | Specifica come gli elementi HTML &lt;p&gt; vengono renderizzati durante il caricamento dell'HTML. Il valore predefinito è HtmlParagraphLayoutMode.Normal. |
| [SetParagraphLayoutMode](./setparagraphlayoutmode/) | Specifica come gli elementi HTML &lt;p&gt; vengono renderizzati durante il caricamento dell'HTML. Il valore predefinito è HtmlParagraphLayoutMode.Normal. |
| [GetHyperlinkLoadMode](./gethyperlinkloadmode/) | Specifica come i collegamenti ipertestuali vengono caricati durante il caricamento dell'HTML. |
| [SetHyperlinkLoadMode](./sethyperlinkloadmode/) | Specifica come i collegamenti ipertestuali vengono caricati durante il caricamento dell'HTML. |
| [GetLoadFormat](./getloadformat/) | Ottiene il formato di caricamento. |
| [GetPassword](./getpassword/) | Ottiene e imposta la password della cartella di lavoro. |
| [SetPassword](./setpassword/) | Ottiene e imposta la password della cartella di lavoro. |
| [GetParsingFormulaOnOpen](./getparsingformulaonopen/) | Indica se analizzare la formula durante la lettura del file. |
| [SetParsingFormulaOnOpen](./setparsingformulaonopen/) | Indica se analizzare la formula durante la lettura del file. |
| [GetParsingPivotCachedRecords](./getparsingpivotcachedrecords/) | Indica se analizzare i record cache della tabella pivot durante il caricamento del file. Il valore predefinito è false. |
| [SetParsingPivotCachedRecords](./setparsingpivotcachedrecords/) | Indica se analizzare i record cache della tabella pivot durante il caricamento del file. Il valore predefinito è false. |
| [SetPaperSize](./setpapersize/) | Imposta la dimensione della carta di stampa predefinita dalle impostazioni della stampante predefinita. |
| [GetLanguageCode](./getlanguagecode/) | Ottiene o imposta la lingua dell'interfaccia utente della versione della Cartella di lavoro basata sul CountryCode con cui è stato salvato il file. |
| [SetLanguageCode](./setlanguagecode/) | Ottiene o imposta la lingua dell'interfaccia utente della versione della Cartella di lavoro basata sul CountryCode con cui è stato salvato il file. |
| [GetRegion](./getregion/) | Ottiene o imposta le impostazioni regionali utilizzate per la Cartella di lavoro che verrà caricata. |
| [SetRegion](./setregion/) | Ottiene o imposta le impostazioni regionali utilizzate per la Cartella di lavoro che verrà caricata. |
| [GetDefaultStyleSettings](./getdefaultstylesettings/) | Ottiene le impostazioni di stile predefinite per l'inizializzazione degli stili della cartella di lavoro |
| [GetInterruptMonitor](./getinterruptmonitor/) | Ottiene e imposta il monitor di interruzione. |
| [SetInterruptMonitor](./setinterruptmonitor/) | Ottiene e imposta il monitor di interruzione. |
| [GetIgnoreNotPrinted](./getignorenotprinted/) | Ignora i dati che non vengono stampati se si stampa direttamente il file |
| [SetIgnoreNotPrinted](./setignorenotprinted/) | Ignora i dati che non vengono stampati se si stampa direttamente il file |
| [GetCheckDataValid](./getcheckdatavalid/) | Verifica se i dati sono validi nel file modello. |
| [SetCheckDataValid](./setcheckdatavalid/) | Verifica se i dati sono validi nel file modello. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | Indica se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Per esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando si inserisce un valore più lungo di 32K, ad esempio tramite Cell.PutValue(string), se questa proprietà è true, si otterrà un'Exception. Se questa proprietà è false, accetteremo la stringa inserita come valore della cella, così in seguito potrai esportare la stringa completa per altri formati di file come CSV. Tuttavia, se hai impostato un valore di questo tipo che è non valido per il formato file Excel, non dovresti salvare la cartella di lavoro come formato Excel in seguito. Altrimenti potrebbero verificarsi errori imprevisti nel file Excel generato. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | Indica se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Per esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando si inserisce un valore più lungo di 32K, ad esempio tramite Cell.PutValue(string), se questa proprietà è true, si otterrà un'Exception. Se questa proprietà è false, accetteremo la stringa inserita come valore della cella, così in seguito potrai esportare la stringa completa per altri formati di file come CSV. Tuttavia, se hai impostato un valore di questo tipo che è non valido per il formato file Excel, non dovresti salvare la cartella di lavoro come formato Excel in seguito. Altrimenti potrebbero verificarsi errori imprevisti nel file Excel generato. |
| [GetKeepUnparsedData](./getkeepunparseddata/) | Indica se mantenere i dati non analizzati in memoria per la Cartella di lavoro quando viene caricata dal file modello. Il valore predefinito è true. |
| [SetKeepUnparsedData](./setkeepunparseddata/) | Indica se mantenere i dati non analizzati in memoria per la Cartella di lavoro quando viene caricata dal file modello. Il valore predefinito è true. |
| [GetLoadFilter](./getloadfilter/) | Il filtro per indicare come caricare i dati. |
| [SetLoadFilter](./setloadfilter/) | Il filtro per indicare come caricare i dati. |
| [GetMemorySetting](./getmemorysetting/) | Ottiene o imposta la modalità di memoria per la cartella di lavoro caricata. |
| [SetMemorySetting](./setmemorysetting/) | Ottiene o imposta la modalità di memoria per la cartella di lavoro caricata. |
| [GetAutoFitterOptions](./getautofitteroptions/) | Ottiene e imposta le opzioni dell'auto fitter. |
| [SetAutoFitterOptions](./setautofitteroptions/) | Ottiene e imposta le opzioni dell'auto fitter. |
| [GetAutoFilter](./getautofilter/) | Indica se filtrare automaticamente i dati durante il caricamento dei file. |
| [SetAutoFilter](./setautofilter/) | Indica se filtrare automaticamente i dati durante il caricamento dei file. |
| [GetFontConfigs](./getfontconfigs/) | Ottiene e imposta le configurazioni dei font individuali. Funziona solo per la Cartella di lavoro che utilizza questo LoadOptions per il caricamento. |
| [SetFontConfigs](./setfontconfigs/) | Ottiene e imposta le configurazioni dei font individuali. Funziona solo per la Cartella di lavoro che utilizza questo LoadOptions per il caricamento. |
| [GetIgnoreUselessShapes](./getignoreuselessshapes/) | Indica se ignorare forme inutili. |
| [SetIgnoreUselessShapes](./setignoreuselessshapes/) | Indica se ignorare forme inutili. |
| [GetPreservePaddingSpacesInFormula](./getpreservepaddingspacesinformula/) | Indica se preservare quegli spazi e interruzioni di riga che sono inseriti tra i token della formula durante l'ottenimento e l'impostazione delle formule. Il valore predefinito è false. |
| [SetPreservePaddingSpacesInFormula](./setpreservepaddingspacesinformula/) | Indica se preservare quegli spazi e interruzioni di riga che sono inseriti tra i token della formula durante l'ottenimento e l'impostazione delle formule. Il valore predefinito è false. |
