---
title: "Classe TxtSaveOptions"
linktitle: "TxtSaveOptions"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe TxtSaveOptions. Incapsula l'oggetto che rappresenta txtsaveoptions in Go."
type: docs
weight: 200
url: /it/go-cpp/txtsaveoptions/
---

## TxtSaveOptions class

Rappresenta le opzioni di salvataggio per il formato csv/tab delimitato/altri formati di testo.

```go

type TxtSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewTxtSaveOptions](./newtxtsaveoptions/) | Crea le opzioni di salvataggio per file di testo. |
| [NewTxtSaveOptions_SaveFormat](./newtxtsaveoptions_saveformat/) | Crea le opzioni di salvataggio per file di testo. |
| [NewTxtSaveOptions_SaveOptions](./newtxtsaveoptions_saveoptions/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetSeparator](./getseparator/) | Recupera e imposta il delimitatore di caratteri del file di testo. |
| [SetSeparator](./setseparator/) | Recupera e imposta il delimitatore di caratteri del file di testo. |
| [GetSeparatorString](./getseparatorstring/) | Recupera e imposta un valore stringa come separatore. |
| [SetSeparatorString](./setseparatorstring/) | Recupera e imposta un valore stringa come separatore. |
| [GetEncoding](./getencoding/) | Recupera e imposta la codifica predefinita. |
| [SetEncoding](./setencoding/) | Recupera e imposta la codifica predefinita. |
| [GetQuoteType](./getquotetype/) | Recupera o imposta come citare i valori nel file di testo esportato. |
| [SetQuoteType](./setquotetype/) | Recupera o imposta come citare i valori nel file di testo esportato. |
| [GetFormatStrategy](./getformatstrategy/) | Recupera e imposta la strategia di formattazione quando si esporta il valore della cella come stringa. |
| [SetFormatStrategy](./setformatstrategy/) | Recupera e imposta la strategia di formattazione quando si esporta il valore della cella come stringa. |
| [GetTrimLeadingBlankRowAndColumn](./gettrimleadingblankrowandcolumn/) | Indica se le righe e le colonne vuote iniziali devono essere rimosse, come fa MS Excel. Il valore predefinito è true. |
| [SetTrimLeadingBlankRowAndColumn](./settrimleadingblankrowandcolumn/) | Indica se le righe e le colonne vuote iniziali devono essere rimosse, come fa MS Excel. Il valore predefinito è true. |
| [GetTrimTailingBlankCells](./gettrimtailingblankcells/) | Indica se le celle vuote finali in una riga devono essere rimosse. Il valore predefinito è false. |
| [SetTrimTailingBlankCells](./settrimtailingblankcells/) | Indica se le celle vuote finali in una riga devono essere rimosse. Il valore predefinito è false. |
| [GetKeepSeparatorsForBlankRow](./getkeepseparatorsforblankrow/) | Indica se i separatori devono essere emessi per una riga vuota. Il valore predefinito è false, quindi per impostazione predefinita il contenuto della riga vuota sarà vuoto. |
| [SetKeepSeparatorsForBlankRow](./setkeepseparatorsforblankrow/) | Indica se i separatori devono essere emessi per una riga vuota. Il valore predefinito è false, quindi per impostazione predefinita il contenuto della riga vuota sarà vuoto. |
| [GetExportArea](./getexportarea/) | L'intervallo di celle da esportare. |
| [SetExportArea](./setexportarea/) | L'intervallo di celle da esportare. |
| [GetExportQuotePrefix](./getexportquoteprefix/) | Indica se il segno di apice singolo deve essere esportato come parte del valore di una cella quando Style.QuotePrefix è true per essa. Il valore predefinito è false. |
| [SetExportQuotePrefix](./setexportquoteprefix/) | Indica se il segno di apice singolo deve essere esportato come parte del valore di una cella quando Style.QuotePrefix è true per essa. Il valore predefinito è false. |
| [GetExportAllSheets](./getexportallsheets/) | Indica se esportare tutti i fogli nel file di testo. Se è false, esporta solo il foglio attivo, proprio come MS Excel. |
| [SetExportAllSheets](./setexportallsheets/) | Indica se esportare tutti i fogli nel file di testo. Se è false, esporta solo il foglio attivo, proprio come MS Excel. |
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
