---
title: "Classe XmlSaveOptions"
linktitle: "XmlSaveOptions"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe XmlSaveOptions. Incapsula l'oggetto che rappresenta xmlsaveoptions in Go."
type: docs
weight: 200
url: /it/go-cpp/xmlsaveoptions/
---

## XmlSaveOptions class

Rappresenta le opzioni per salvare la cartella di lavoro come file XML.

```go

type XmlSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewXmlSaveOptions](./newxmlsaveoptions/) | Crea opzioni per il salvataggio di file XML. |
| [NewXmlSaveOptions_SaveOptions](./newxmlsaveoptions_saveoptions/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetSheetIndexes](./getsheetindexes/) | Rappresenta gli indici dei fogli esportati. |
| [SetSheetIndexes](./setsheetindexes/) | Rappresenta gli indici dei fogli esportati. |
| [GetExportArea](./getexportarea/) | Ottiene o imposta l'intervallo di esportazione. |
| [SetExportArea](./setexportarea/) | Ottiene o imposta l'intervallo di esportazione. |
| [GetHasHeaderRow](./gethasheaderrow/) | Indica se l'intervallo contiene la riga di intestazione. |
| [SetHasHeaderRow](./sethasheaderrow/) | Indica se l'intervallo contiene la riga di intestazione. |
| [GetXmlMapName](./getxmlmapname/) | Indica se esportare la mappa XML nel file. |
| [SetXmlMapName](./setxmlmapname/) | Indica se esportare la mappa XML nel file. |
| [GetSheetNameAsElementName](./getsheetnameaselementname/) | Indica se esportare il nome del foglio come nome dell'elemento. |
| [SetSheetNameAsElementName](./setsheetnameaselementname/) | Indica se esportare il nome del foglio come nome dell'elemento. |
| [GetDataAsAttribute](./getdataasattribute/) | Indica se esportare i dati come attributi dell'elemento. |
| [SetDataAsAttribute](./setdataasattribute/) | Indica se esportare i dati come attributi dell'elemento. |
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
