---
title: "Classe OoxmlSaveOptions"
linktitle: "OoxmlSaveOptions"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe OoxmlSaveOptions. Incapsula l'oggetto che rappresenta ooxmlsaveoptions in Go."
type: docs
weight: 200
url: /it/go-cpp/ooxmlsaveoptions/
---

## OoxmlSaveOptions class

Rappresenta le opzioni di salvataggio del file Office Open XML.

```go

type OoxmlSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewOoxmlSaveOptions](./newooxmlsaveoptions/) | Crea le opzioni per salvare il file Office Open XML. |
| [NewOoxmlSaveOptions_SaveFormat](./newooxmlsaveoptions_saveformat/) | Crea le opzioni per salvare il file Office Open XML. |
| [NewOoxmlSaveOptions_SaveOptions](./newooxmlsaveoptions_saveoptions/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetAsFlatOpc](./getasflatopc/) | Indica se salvare come file OPC flat che può essere generato da Open XML SDK. |
| [SetAsFlatOpc](./setasflatopc/) | Indica se salvare come file OPC flat che può essere generato da Open XML SDK. |
| [GetExportCellName](./getexportcellname/) | Indica se esportare il nome della cella in un file Excel2007 .xlsx (.xlsm, .xltx, .xltm). Se il file di output può essere accessibile da SQL Server DTS, questo valore deve essere true. Impostare il valore a false aumenterà notevolmente le prestazioni e ridurrà la dimensione del file quando si creano file di grandi dimensioni. Il valore predefinito è true. |
| [SetExportCellName](./setexportcellname/) | Indica se esportare il nome della cella in un file Excel2007 .xlsx (.xlsm, .xltx, .xltm). Se il file di output può essere accessibile da SQL Server DTS, questo valore deve essere true. Impostare il valore a false aumenterà notevolmente le prestazioni e ridurrà la dimensione del file quando si creano file di grandi dimensioni. Il valore predefinito è true. |
| [GetUpdateZoom](./getupdatezoom/) | Indica se aggiornare il fattore di scala prima di salvare il file se le proprietà PageSetup.FitToPagesWide e PageSetup.FitToPagesTall controllano come il foglio di lavoro viene scalato. |
| [SetUpdateZoom](./setupdatezoom/) | Indica se aggiornare il fattore di scala prima di salvare il file se le proprietà PageSetup.FitToPagesWide e PageSetup.FitToPagesTall controllano come il foglio di lavoro viene scalato. |
| [GetEnableZip64](./getenablezip64/) | Utilizza le estensioni ZIP64 durante la scrittura di archivi zip, se necessario. |
| [SetEnableZip64](./setenablezip64/) | Utilizza le estensioni ZIP64 durante la scrittura di archivi zip, se necessario. |
| [GetEmbedOoxmlAsOleObject](./getembedooxmlasoleobject/) | Indica se incorporare file Ooxml di OleObject come oggetto ole. |
| [SetEmbedOoxmlAsOleObject](./setembedooxmlasoleobject/) | Indica se incorporare file Ooxml di OleObject come oggetto ole. |
| [GetCompressionType](./getcompressiontype/) | Ottiene e imposta il tipo di compressione per il file ooxml. |
| [SetCompressionType](./setcompressiontype/) | Ottiene e imposta il tipo di compressione per il file ooxml. |
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
