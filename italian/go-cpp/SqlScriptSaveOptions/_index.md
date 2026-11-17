---
title: "Classe SqlScriptSaveOptions"
linktitle: "SqlScriptSaveOptions"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe SqlScriptSaveOptions. Incapsula l'oggetto che rappresenta sqlscriptsaveoptions in Go."
type: docs
weight: 200
url: /it/go-cpp/sqlscriptsaveoptions/
---

## SqlScriptSaveOptions class

Rappresenta le opzioni di salvataggio di sql.

```go

type SqlScriptSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewSqlScriptSaveOptions](./newsqlscriptsaveoptions/) | Crea le opzioni per salvare il file sql. |
| [NewSqlScriptSaveOptions_SaveOptions](./newsqlscriptsaveoptions_saveoptions/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetCheckIfTableExists](./getcheckiftableexists/) | Verifica se il nome della tabella esiste prima di creare |
| [SetCheckIfTableExists](./setcheckiftableexists/) | Verifica se il nome della tabella esiste prima di creare |
| [GetColumnTypeMap](./getcolumntypemap/) | Ottiene e imposta la mappa dei tipi di colonna per diversi database. |
| [SetColumnTypeMap](./setcolumntypemap/) | Ottiene e imposta la mappa dei tipi di colonna per diversi database. |
| [GetCheckAllDataForColumnType](./getcheckalldataforcolumntype/) | Controlla tutti i dati per trovare il tipo di dati delle colonne. |
| [SetCheckAllDataForColumnType](./setcheckalldataforcolumntype/) | Controlla tutti i dati per trovare il tipo di dati delle colonne. |
| [GetAddBlankLineBetweenRows](./getaddblanklinebetweenrows/) | Inserisci una riga vuota tra ogni dato. |
| [SetAddBlankLineBetweenRows](./setaddblanklinebetweenrows/) | Inserisci una riga vuota tra ogni dato. |
| [GetSeparator](./getseparator/) | Ottiene e imposta il separatore di caratteri dello script sql. |
| [SetSeparator](./setseparator/) | Ottiene e imposta il separatore di caratteri dello script sql. |
| [GetOperatorType](./getoperatortype/) | Ottiene e imposta il tipo di operatore di sql. |
| [SetOperatorType](./setoperatortype/) | Ottiene e imposta il tipo di operatore di sql. |
| [GetPrimaryKey](./getprimarykey/) | Rappresenta quale colonna è la chiave primaria della tabella dati. |
| [SetPrimaryKey](./setprimarykey/) | Rappresenta quale colonna è la chiave primaria della tabella dati. |
| [GetCreateTable](./getcreatetable/) | Indica se esportare sql per la creazione della tabella. |
| [SetCreateTable](./setcreatetable/) | Indica se esportare sql per la creazione della tabella. |
| [GetIdName](./getidname/) | Ottiene e imposta il nome della colonna ID. |
| [SetIdName](./setidname/) | Ottiene e imposta il nome della colonna ID. |
| [GetStartId](./getstartid/) | Ottiene e imposta l'ID di partenza. |
| [SetStartId](./setstartid/) | Ottiene e imposta l'ID di partenza. |
| [GetTableName](./gettablename/) | Ottiene e imposta il nome della tabella. |
| [SetTableName](./settablename/) | Ottiene e imposta il nome della tabella. |
| [GetExportAsString](./getexportasstring/) | Indica se esportare tutti i dati come valore stringa. |
| [SetExportAsString](./setexportasstring/) | Indica se esportare tutti i dati come valore stringa. |
| [GetSheetIndexes](./getsheetindexes/) | Rappresenta gli indici dei fogli esportati. |
| [SetSheetIndexes](./setsheetindexes/) | Rappresenta gli indici dei fogli esportati. |
| [GetExportArea](./getexportarea/) | Ottiene o imposta l'intervallo di esportazione. |
| [SetExportArea](./setexportarea/) | Ottiene o imposta l'intervallo di esportazione. |
| [GetHasHeaderRow](./gethasheaderrow/) | Indica se l'intervallo contiene la riga di intestazione. |
| [SetHasHeaderRow](./sethasheaderrow/) | Indica se l'intervallo contiene la riga di intestazione. |
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
