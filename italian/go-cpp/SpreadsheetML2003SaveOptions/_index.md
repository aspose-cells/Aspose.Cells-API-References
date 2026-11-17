---
title: "Classe SpreadsheetML2003SaveOptions"
linktitle: "SpreadsheetML2003SaveOptions"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe SpreadsheetML2003SaveOptions. Incapsula l'oggetto che rappresenta spreadsheetml2003saveoptions in Go."
type: docs
weight: 200
url: /it/go-cpp/spreadsheetml2003saveoptions/
---

## SpreadsheetML2003SaveOptions class

Rappresenta le opzioni per salvare il file Excel 2003 spreadml.

```go

type SpreadsheetML2003SaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewSpreadsheetML2003SaveOptions](./newspreadsheetml2003saveoptions/) | Crea le opzioni per salvare il file Excel 2003 spreadml. |
| [NewSpreadsheetML2003SaveOptions_SaveOptions](./newspreadsheetml2003saveoptions_saveoptions/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [IsIndentedFormatting](./isindentedformatting/) | Fa sì che gli elementi figli siano indentati. |
| [SetIsIndentedFormatting](./setisindentedformatting/) | Fa sì che gli elementi figli siano indentati. |
| [GetLimitAsXls](./getlimitasxls/) | Limite per xls, l'indice massimo di riga è 65535 e l'indice massimo di colonna è 255. |
| [SetLimitAsXls](./setlimitasxls/) | Limite per xls, l'indice massimo di riga è 65535 e l'indice massimo di colonna è 255. |
| [GetExportColumnIndexOfCell](./getexportcolumnindexofcell/) | Il valore predefinito è false, significa che l'indice di colonna sarà ignorato se la cella è contigua alla cella precedente. |
| [SetExportColumnIndexOfCell](./setexportcolumnindexofcell/) | Il valore predefinito è false, significa che l'indice di colonna sarà ignorato se la cella è contigua alla cella precedente. |
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
