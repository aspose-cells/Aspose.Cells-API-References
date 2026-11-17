---
title: "Classe JsonSaveOptions"
linktitle: "JsonSaveOptions"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe JsonSaveOptions. Incapsula l'oggetto che rappresenta jsonsaveoptions in Go."
type: docs
weight: 200
url: /it/go-cpp/jsonsaveoptions/
---

## JsonSaveOptions class

Rappresenta le opzioni di salvataggio della cartella di lavoro come file JSON.

```go

type JsonSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewJsonSaveOptions](./newjsonsaveoptions/) | Crea opzioni per il salvataggio di file json. |
| [NewJsonSaveOptions_SaveOptions](./newjsonsaveoptions_saveoptions/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetExportStylePool](./getexportstylepool/) | Indica se esportare gli stili collettivamente o individualmente per ogni cella. |
| [SetExportStylePool](./setexportstylepool/) | Indica se esportare gli stili collettivamente o individualmente per ogni cella. |
| [GetExportHyperlinkType](./getexporthyperlinktype/) | Rappresenta il tipo di esportazione dei collegamenti ipertestuali in json. |
| [SetExportHyperlinkType](./setexporthyperlinktype/) | Rappresenta il tipo di esportazione dei collegamenti ipertestuali in json. |
| [GetSkipEmptyRows](./getskipemptyrows/) | Indica se saltare le righe vuote. |
| [SetSkipEmptyRows](./setskipemptyrows/) | Indica se saltare le righe vuote. |
| [GetSheetIndexes](./getsheetindexes/) | Rappresenta gli indici dei fogli esportati. |
| [SetSheetIndexes](./setsheetindexes/) | Rappresenta gli indici dei fogli esportati. |
| [GetSchemas](./getschemas/) | Lo schema json originale di ogni foglio di lavoro. |
| [SetSchemas](./setschemas/) | Lo schema json originale di ogni foglio di lavoro. |
| [GetExportArea](./getexportarea/) | Ottiene o imposta l'intervallo di esportazione. |
| [SetExportArea](./setexportarea/) | Ottiene o imposta l'intervallo di esportazione. |
| [GetHasHeaderRow](./gethasheaderrow/) | Indica se l'intervallo contiene la riga di intestazione. |
| [SetHasHeaderRow](./sethasheaderrow/) | Indica se l'intervallo contiene la riga di intestazione. |
| [GetExportAsString](./getexportasstring/) | Esporta il valore stringa delle celle in json. |
| [SetExportAsString](./setexportasstring/) | Esporta il valore stringa delle celle in json. |
| [GetIndent](./getindent/) | Indica l'indentazione. |
| [SetIndent](./setindent/) | Indica l'indentazione. |
| [GetExportNestedStructure](./getexportnestedstructure/) | Esportato come struttura Json gerarchica padre-figlio. |
| [SetExportNestedStructure](./setexportnestedstructure/) | Esportato come struttura Json gerarchica padre-figlio. |
| [GetExportEmptyCells](./getexportemptycells/) | Indica se esportare le celle vuote come null. |
| [SetExportEmptyCells](./setexportemptycells/) | Indica se esportare le celle vuote come null. |
| [GetAlwaysExportAsJsonObject](./getalwaysexportasjsonobject/) | Indica se esportare sempre Excel in json come oggetto, anche se nel file è presente un solo foglio di lavoro. |
| [SetAlwaysExportAsJsonObject](./setalwaysexportasjsonobject/) | Indica se esportare sempre Excel in json come oggetto, anche se nel file è presente un solo foglio di lavoro. |
| [GetToExcelStruct](./gettoexcelstruct/) | Indica se convertire in una struttura json del file Excel. |
| [SetToExcelStruct](./settoexcelstruct/) | Indica se convertire in una struttura json del file Excel. |
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
