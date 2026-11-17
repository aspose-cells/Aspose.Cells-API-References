---
title: "TxtLoadOptions Classe"
linktitle: "TxtLoadOptions"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "TxtLoadOptions classe. Incapsula l'oggetto che rappresenta txtloadoptions in Go."
type: docs
weight: 200
url: /it/go-cpp/txtloadoptions/
---

## TxtLoadOptions class

Rappresenta le opzioni per caricare un file di testo.

```go

type TxtLoadOptions struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewTxtLoadOptions](./newtxtloadoptions/) | Crea le opzioni per il caricamento del file di testo. |
| [NewTxtLoadOptions_LoadFormat](./newtxtloadoptions_loadformat/) | Crea le opzioni per il caricamento del file di testo. |
| [NewTxtLoadOptions_AbstractTextLoadOptions](./newtxtloadoptions_abstracttextloadoptions/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetSeparator](./getseparator/) | Ottiene e imposta il separatore di caratteri del file di testo. |
| [SetSeparator](./setseparator/) | Ottiene e imposta il separatore di caratteri del file di testo. |
| [GetSeparatorString](./getseparatorstring/) | Recupera e imposta un valore stringa come separatore. |
| [SetSeparatorString](./setseparatorstring/) | Recupera e imposta un valore stringa come separatore. |
| [IsMultiEncoded](./ismultiencoded/) | True indica che il file contiene diverse codifiche. |
| [SetIsMultiEncoded](./setismultiencoded/) | True indica che il file contiene diverse codifiche. |
| [GetHasFormula](./gethasformula/) | Indica se il testo è una formula se inizia con "=", |
| [SetHasFormula](./sethasformula/) | Indica se il testo è una formula se inizia con "=", |
| [GetHasTextQualifier](./gethastextqualifier/) | Indica se esiste un qualificatore di testo per il valore della cella. Il valore predefinito è true. |
| [SetHasTextQualifier](./sethastextqualifier/) | Indica se esiste un qualificatore di testo per il valore della cella. Il valore predefinito è true. |
| [GetTextQualifier](./gettextqualifier/) | Specifica il qualificatore di testo per i valori delle celle. Il qualificatore predefinito è '\"'. |
| [SetTextQualifier](./settextqualifier/) | Specifica il qualificatore di testo per i valori delle celle. Il qualificatore predefinito è '\"'. |
| [GetTreatConsecutiveDelimitersAsOne](./gettreatconsecutivedelimitersasone/) | Indica se i delimitatori consecutivi devono essere trattati come uno. |
| [SetTreatConsecutiveDelimitersAsOne](./settreatconsecutivedelimitersasone/) | Indica se i delimitatori consecutivi devono essere trattati come uno. |
| [GetTreatQuotePrefixAsValue](./gettreatquoteprefixasvalue/) | Indica se il segno di apice singolo iniziale deve essere considerato parte del valore di una cella. Il valore predefinito è true. Se è false, l'apice singolo iniziale verrà rimosso dal valore della cella corrispondente e Style.QuotePrefix sarà impostato a true per la cella. |
| [SetTreatQuotePrefixAsValue](./settreatquoteprefixasvalue/) | Indica se il segno di apice singolo iniziale deve essere considerato parte del valore di una cella. Il valore predefinito è true. Se è false, l'apice singolo iniziale verrà rimosso dal valore della cella corrispondente e Style.QuotePrefix sarà impostato a true per la cella. |
| [GetExtendToNextSheet](./getextendtonextsheet/) | Indica se estendere i dati al foglio successivo quando le righe o le colonne dei dati superano il limite. Il valore predefinito è false. |
| [SetExtendToNextSheet](./setextendtonextsheet/) | Indica se estendere i dati al foglio successivo quando le righe o le colonne dei dati superano il limite. Il valore predefinito è false. |
| [GetHeaderRowsCount](./getheaderrowscount/) | Il conteggio delle righe di intestazione da ripetere per i fogli estesi. |
| [SetHeaderRowsCount](./setheaderrowscount/) | Il conteggio delle righe di intestazione da ripetere per i fogli estesi. |
| [GetHeaderColumnsCount](./getheadercolumnscount/) | Il conteggio delle colonne di intestazione da ripetere per i fogli estesi. |
| [SetHeaderColumnsCount](./setheadercolumnscount/) | Il conteggio delle colonne di intestazione da ripetere per i fogli estesi. |
| [GetMaxRowCount](./getmaxrowcount/) | Il conteggio massimo di righe da importare per un foglio. |
| [SetMaxRowCount](./setmaxrowcount/) | Il conteggio massimo di righe da importare per un foglio. |
| [GetMaxColumnCount](./getmaxcolumncount/) | Il conteggio massimo di colonne da importare per un foglio. |
| [SetMaxColumnCount](./setmaxcolumncount/) | Il conteggio massimo di colonne da importare per un foglio. |
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
