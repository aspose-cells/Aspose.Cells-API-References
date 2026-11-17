---
title: "XmlLoadOptions Classe"
linktitle: "XmlLoadOptions"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "XmlLoadOptions classe. Incapsula l'oggetto che rappresenta xmlloadoptions in Go."
type: docs
weight: 200
url: /it/go-cpp/xmlloadoptions/
---

## XmlLoadOptions class

Rappresenta le opzioni di caricamento XML.

```go

type XmlLoadOptions struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewXmlLoadOptions](./newxmlloadoptions/) | Rappresenta le opzioni di caricamento del file xml. |
| [NewXmlLoadOptions_LoadFormat](./newxmlloadoptions_loadformat/) | Rappresenta le opzioni di caricamento del file xml. |
| [NewXmlLoadOptions_LoadOptions](./newxmlloadoptions_loadoptions/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetStartCell](./getstartcell/) | Ottiene e imposta la cella di partenza. |
| [SetStartCell](./setstartcell/) | Ottiene e imposta la cella di partenza. |
| [IsXmlMap](./isxmlmap/) | Indica se mappare xml su Excel. Il valore predefinito è false. |
| [SetIsXmlMap](./setisxmlmap/) | Indica se mappare xml su Excel. Il valore predefinito è false. |
| [GetContainsMultipleWorksheets](./getcontainsmultipleworksheets/) | Indica se importare xml come più fogli di lavoro. |
| [SetContainsMultipleWorksheets](./setcontainsmultipleworksheets/) | Indica se importare xml come più fogli di lavoro. |
| [GetConvertNumericOrDate](./getconvertnumericordate/) | Indica se convertire il valore nel file xml in numerico o data. |
| [SetConvertNumericOrDate](./setconvertnumericordate/) | Indica se convertire il valore nel file xml in numerico o data. |
| [Get_NumberFormat](./get_numberformat/) | Ottiene e imposta il formato del valore numerico. |
| [SetNumberFormat](./setnumberformat/) | Ottiene e imposta il formato del valore numerico. |
| [Get_DateFormat](./get_dateformat/) | Ottiene e imposta il formato del valore di data. |
| [SetDateFormat](./setdateformat/) | Ottiene e imposta il formato del valore di data. |
| [GetIgnoreRootAttributes](./getignorerootattributes/) | Indica se ignorare gli attributi dell'elemento radice. |
| [SetIgnoreRootAttributes](./setignorerootattributes/) | Indica se ignorare gli attributi dell'elemento radice. |
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
