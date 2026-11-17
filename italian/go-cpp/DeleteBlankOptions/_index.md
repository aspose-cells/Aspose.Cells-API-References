---
title: "DeleteBlankOptions Class"
linktitle: "DeleteBlankOptions"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "DeleteBlankOptions class. Incapsula l'oggetto che rappresenta deleteblankoptions in Go."
type: docs
weight: 200
url: /it/go-cpp/deleteblankoptions/
---

## DeleteBlankOptions class

Rappresenta l'impostazione per l'eliminazione di celle/righe/colonne vuote.

```go

type DeleteBlankOptions struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewDeleteBlankOptions](./newdeleteblankoptions/) | Costruttore predefinito. |
| [NewDeleteBlankOptions_DeleteOptions](./newdeleteblankoptions_deleteoptions/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetEmptyStringAsBlank](./getemptystringasblank/) | Indica se una cella verrà considerata vuota quando il suo valore è una stringa vuota. Il valore predefinito è true. |
| [SetEmptyStringAsBlank](./setemptystringasblank/) | Indica se una cella verrà considerata vuota quando il suo valore è una stringa vuota. Il valore predefinito è true. |
| [GetEmptyFormulaValueAsBlank](./getemptyformulavalueasblank/) | Indica se una cella verrà considerata vuota quando è una formula e il risultato calcolato è null o una stringa vuota. Il valore predefinito è false. |
| [SetEmptyFormulaValueAsBlank](./setemptyformulavalueasblank/) | Indica se una cella verrà considerata vuota quando è una formula e il risultato calcolato è null o una stringa vuota. Il valore predefinito è false. |
| [GetDrawingsAsBlank](./getdrawingsasblank/) | Indica se gli oggetti correlati al disegno, come immagine, forma, grafico... verranno considerati vuoti. Il valore predefinito è true. |
| [SetDrawingsAsBlank](./setdrawingsasblank/) | Indica se gli oggetti correlati al disegno, come immagine, forma, grafico... verranno considerati vuoti. Il valore predefinito è true. |
| [GetMergedCellsShrinkType](./getmergedcellsshrinktype/) | Indica come elaborare le celle unite quando si eliminano righe/colonne vuote. |
| [SetMergedCellsShrinkType](./setmergedcellsshrinktype/) | Indica come elaborare le celle unite quando si eliminano righe/colonne vuote. |
| [GetStartIndex](./getstartindex/) | Specifica l'indice di riga/colonna iniziale dell'intervallo da verificare e cancellare righe/colonne vuote. |
| [SetStartIndex](./setstartindex/) | Specifica l'indice di riga/colonna iniziale dell'intervallo da verificare e cancellare righe/colonne vuote. |
| [GetEndIndex](./getendindex/) | Specifica l'indice di riga/colonna finale (inclusivo) dell'intervallo da verificare e cancellare righe/colonne vuote. Il valore predefinito è -1 e -1 indica l'intervallo massimo di tutti gli oggetti (celle, disegni, ...) che devono essere controllati. |
| [SetEndIndex](./setendindex/) | Specifica l'indice di riga/colonna finale (inclusivo) dell'intervallo da verificare e cancellare righe/colonne vuote. Il valore predefinito è -1 e -1 indica l'intervallo massimo di tutti gli oggetti (celle, disegni, ...) che devono essere controllati. |
| [GetUpdateReference](./getupdatereference/) | Indica se aggiornare i riferimenti in altri fogli di lavoro. |
| [SetUpdateReference](./setupdatereference/) | Indica se aggiornare i riferimenti in altri fogli di lavoro. |
| [GetFormulaChangeMonitor](./getformulachangemonitor/) | Ottiene/Imposta il monitor per tracciare le modifiche causate dall'eliminazione. |
| [SetFormulaChangeMonitor](./setformulachangemonitor/) | Ottiene/Imposta il monitor per tracciare le modifiche causate dall'eliminazione. |
