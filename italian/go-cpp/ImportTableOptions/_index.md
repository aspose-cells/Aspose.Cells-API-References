---
title: "ImportTableOptions Classe"
linktitle: "ImportTableOptions"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "ImportTableOptions classe. Incapsula l'oggetto che rappresenta importtableoptions in Go."
type: docs
weight: 200
url: /it/go-cpp/importtableoptions/
---

## ImportTableOptions class

Rappresenta le opzioni di importazione dei dati nelle celle.

```go

type ImportTableOptions struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewImportTableOptions](./newimporttableoptions/) | Crea le opzioni di importazione predefinite. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetConvertGridStyle](./getconvertgridstyle/) | Indica se applicare lo stile della vista griglia alle celle. |
| [SetConvertGridStyle](./setconvertgridstyle/) | Indica se applicare lo stile della vista griglia alle celle. |
| [GetConvertNumericData](./getconvertnumericdata/) | Ottiene o imposta un valore che indica se il valore stringa deve essere convertito in valore numerico o data. |
| [SetConvertNumericData](./setconvertnumericdata/) | Ottiene o imposta un valore che indica se il valore stringa deve essere convertito in valore numerico o data. |
| [GetInsertRows](./getinsertrows/) | Indica se devono essere aggiunte nuove righe per l'importazione dei record di dati. |
| [SetInsertRows](./setinsertrows/) | Indica se devono essere aggiunte nuove righe per l'importazione dei record di dati. |
| [GetShiftFirstRowDown](./getshiftfirstrowdown/) | Indica se spostare la prima riga verso il basso durante l'inserimento delle righe. |
| [SetShiftFirstRowDown](./setshiftfirstrowdown/) | Indica se spostare la prima riga verso il basso durante l'inserimento delle righe. |
| [IsFieldNameShown](./isfieldnameshown/) | Indica se il nome del campo deve essere importato. |
| [SetIsFieldNameShown](./setisfieldnameshown/) | Indica se il nome del campo deve essere importato. |
| [GetExportCaptionAsFieldName](./getexportcaptionasfieldname/) | Indica se esportare la didascalia come nome del campo |
| [SetExportCaptionAsFieldName](./setexportcaptionasfieldname/) | Indica se esportare la didascalia come nome del campo |
| [GetDateFormat](./getdateformat/) | Ottiene o imposta la stringa di formato data per le celle con valori datetime importati. |
| [SetDateFormat](./setdateformat/) | Ottiene o imposta la stringa di formato data per le celle con valori datetime importati. |
| [GetNumberFormats](./getnumberformats/) | Ottiene o imposta i formati numerici |
| [SetNumberFormats](./setnumberformats/) | Ottiene o imposta i formati numerici |
| [GetStyles](./getstyles/) | Ottiene e imposta gli stili per ogni colonna della tabella. |
| [SetStyles](./setstyles/) | Ottiene e imposta gli stili per ogni colonna della tabella. |
| [GetIsFormulas](./getisformulas/) | Indica se i dati sono formule. |
| [SetIsFormulas](./setisformulas/) | Indica se i dati sono formule. |
| [GetTotalRows](./gettotalrows/) | Ottiene o imposta il conteggio totale delle righe da importare dalla fonte dati. -1 significa tutte le righe della fonte dati specificata. |
| [SetTotalRows](./settotalrows/) | Ottiene o imposta il conteggio totale delle righe da importare dalla fonte dati. -1 significa tutte le righe della fonte dati specificata. |
| [GetTotalColumns](./gettotalcolumns/) | Ottiene o imposta il conteggio totale delle colonne da importare dalla fonte dati. -1 significa tutte le righe della fonte dati specificata. |
| [SetTotalColumns](./settotalcolumns/) | Ottiene o imposta il conteggio totale delle colonne da importare dalla fonte dati. -1 significa tutte le righe della fonte dati specificata. |
| [GetColumnIndexes](./getcolumnindexes/) | Ottiene o imposta le colonne (indice 0) da importare dalla fonte dati. null significa che tutte le colonne devono essere importate. |
| [SetColumnIndexes](./setcolumnindexes/) | Ottiene o imposta le colonne (indice 0) da importare dalla fonte dati. null significa che tutte le colonne devono essere importate. |
| [GetDefaultValues](./getdefaultvalues/) | Il valore predefinito per il valore nella tabella è null. |
| [SetDefaultValues](./setdefaultvalues/) | Il valore predefinito per il valore nella tabella è null. |
| [IsHtmlString](./ishtmlstring/) | Indica se il valore contiene tag html. |
| [SetIsHtmlString](./setishtmlstring/) | Indica se il valore contiene tag html. |
| [GetCheckMergedCells](./getcheckmergedcells/) | Indica se controllare le celle unite. |
| [SetCheckMergedCells](./setcheckmergedcells/) | Indica se controllare le celle unite. |
