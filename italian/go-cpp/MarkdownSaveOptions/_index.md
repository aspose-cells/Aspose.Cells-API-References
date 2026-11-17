---
title: "Classe MarkdownSaveOptions"
linktitle: "MarkdownSaveOptions"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe MarkdownSaveOptions. Incapsula l'oggetto che rappresenta markdownsaveoptions in Go."
type: docs
weight: 200
url: /it/go-cpp/markdownsaveoptions/
---

## MarkdownSaveOptions class

Rappresenta le opzioni di salvataggio per markdown.

```go

type MarkdownSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewMarkdownSaveOptions](./newmarkdownsaveoptions/) | Crea opzioni per il salvataggio del documento markdown |
| [NewMarkdownSaveOptions_SaveOptions](./newmarkdownsaveoptions_saveoptions/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetEncoding](./getencoding/) | Recupera e imposta la codifica predefinita. |
| [SetEncoding](./setencoding/) | Recupera e imposta la codifica predefinita. |
| [GetFormatStrategy](./getformatstrategy/) | Recupera e imposta la strategia di formattazione quando si esporta il valore della cella come stringa. |
| [SetFormatStrategy](./setformatstrategy/) | Recupera e imposta la strategia di formattazione quando si esporta il valore della cella come stringa. |
| [GetLineSeparator](./getlineseparator/) | Ottiene e imposta il separatore di riga. |
| [SetLineSeparator](./setlineseparator/) | Ottiene e imposta il separatore di riga. |
| [GetTableHeaderType](./gettableheadertype/) | Ottiene e imposta come impostare l'intestazione della tabella. |
| [SetTableHeaderType](./settableheadertype/) | Ottiene e imposta come impostare l'intestazione della tabella. |
| [GetSheetSet](./getsheetset/) | Ottiene o imposta i fogli da renderizzare. L'impostazione predefinita è tutti i fogli visibili nella cartella di lavoro: Aspose.Cells.Rendering.SheetSet.Active. |
| [SetSheetSet](./setsheetset/) | Ottiene o imposta i fogli da renderizzare. L'impostazione predefinita è tutti i fogli visibili nella cartella di lavoro: Aspose.Cells.Rendering.SheetSet.Active. |
| [GetImageOptions](./getimageoptions/) | Ottieni l'oggetto ImageOrPrintOptions prima dell'esportazione. |
| [GetExportImagesAsBase64](./getexportimagesasbase64/) | Specifica se le immagini vengono salvate in formato Base64 in Markdown. Il valore predefinito è true. |
| [SetExportImagesAsBase64](./setexportimagesasbase64/) | Specifica se le immagini vengono salvate in formato Base64 in Markdown. Il valore predefinito è true. |
| [GetCalculateFormula](./getcalculateformula/) | Indica se calcolare le formule prima di salvare il file markdown. |
| [SetCalculateFormula](./setcalculateformula/) | Indica se calcolare le formule prima di salvare il file markdown. |
| [GetExportHyperlinkAsReference](./getexporthyperlinkasreference/) | Indica se esportare i collegamenti ipertestuali usando definizioni di riferimento invece del formato inline. Il valore predefinito è false. |
| [SetExportHyperlinkAsReference](./setexporthyperlinkasreference/) | Indica se esportare i collegamenti ipertestuali usando definizioni di riferimento invece del formato inline. Il valore predefinito è false. |
| [GetAlignColumnPadding](./getaligncolumnpadding/) | Indica se l'allineamento delle colonne è abilitato per le tabelle Markdown generate. Quando abilitato, le colonne sono allineate riempiendo il contenuto delle celle con il carattere specificato (tipicamente ' ' per gli spazi). Impostare a '\0' per disabilitare l'allineamento delle colonne (predefinito). |
| [SetAlignColumnPadding](./setaligncolumnpadding/) | Indica se l'allineamento delle colonne è abilitato per le tabelle Markdown generate. Quando abilitato, le colonne sono allineate riempiendo il contenuto delle celle con il carattere specificato (tipicamente ' ' per gli spazi). Impostare a '\0' per disabilitare l'allineamento delle colonne (predefinito). |
| [GetSplitTablesByBlankRow](./getsplittablesbyblankrow/) | Indica se le righe vuote nel foglio di lavoro devono essere trattate come separatori di tabella durante l'esportazione in Markdown. Il valore predefinito è false. |
| [SetSplitTablesByBlankRow](./setsplittablesbyblankrow/) | Indica se le righe vuote nel foglio di lavoro devono essere trattate come separatori di tabella durante l'esportazione in Markdown. Il valore predefinito è false. |
| [GetOfficeMathOutputType](./getofficemathoutputtype/) | Indica come gli oggetti OfficeMath vengono esportati in Markdown. Il valore predefinito è Image. |
| [SetOfficeMathOutputType](./setofficemathoutputtype/) | Indica come gli oggetti OfficeMath vengono esportati in Markdown. Il valore predefinito è Image. |
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
