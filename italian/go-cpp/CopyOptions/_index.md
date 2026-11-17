---
title: "Classe CopyOptions"
linktitle: "CopyOptions"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe CopyOptions. Incapsula l'oggetto che rappresenta copyoptions in Go."
type: docs
weight: 200
url: /it/go-cpp/copyoptions/
---

## CopyOptions class

Rappresenta le opzioni di copia.

```go

type CopyOptions struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewCopyOptions](./newcopyoptions/) | Costruttore CopyOptions. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetKeepMacros](./getkeepmacros/) | Indica se mantenere le macro; |
| [SetKeepMacros](./setkeepmacros/) | Indica se mantenere le macro; |
| [GetExtendToAdjacentRange](./getextendtoadjacentrange/) | Indica se estendere gli intervalli quando si copia l'intervallo a quello adiacente. |
| [SetExtendToAdjacentRange](./setextendtoadjacentrange/) | Indica se estendere gli intervalli quando si copia l'intervallo a quello adiacente. |
| [GetCopyNames](./getcopynames/) | Indica se copiare i nomi. |
| [SetCopyNames](./setcopynames/) | Indica se copiare i nomi. |
| [GetCopyInvalidFormulasAsValues](./getcopyinvalidformulasasvalues/) | Se la formula non è valida per la destinazione, copia solo i valori. |
| [SetCopyInvalidFormulasAsValues](./setcopyinvalidformulasasvalues/) | Se la formula non è valida per la destinazione, copia solo i valori. |
| [GetColumnCharacterWidth](./getcolumncharacterwidth/) | Indica se copiare la larghezza della colonna in unità di caratteri. |
| [SetColumnCharacterWidth](./setcolumncharacterwidth/) | Indica se copiare la larghezza della colonna in unità di caratteri. |
| [GetReferToSheetWithSameName](./getrefertosheetwithsamename/) | In MS Excel, quando si copiano formule che fanno riferimento ad altri fogli di lavoro durante la copia di un foglio in un altro, le formule copiate dovrebbero fare riferimento alla cartella di lavoro di origine. Tuttavia, in alcune situazioni l'utente potrebbe aver bisogno che le formule copiate facciano riferimento a fogli con lo stesso nome nella stessa cartella di lavoro, ad esempio quando quei fogli sono stati copiati prima di questa operazione di copia; in tal caso questa proprietà dovrebbe essere impostata su true. |
| [SetReferToSheetWithSameName](./setrefertosheetwithsamename/) | In MS Excel, quando si copiano formule che fanno riferimento ad altri fogli di lavoro durante la copia di un foglio in un altro, le formule copiate dovrebbero fare riferimento alla cartella di lavoro di origine. Tuttavia, in alcune situazioni l'utente potrebbe aver bisogno che le formule copiate facciano riferimento a fogli con lo stesso nome nella stessa cartella di lavoro, ad esempio quando quei fogli sono stati copiati prima di questa operazione di copia; in tal caso questa proprietà dovrebbe essere impostata su true. |
| [GetReferToDestinationSheet](./getrefertodestinationsheet/) | Quando si copia l'intervallo nello stesso file e il grafico fa riferimento al foglio di origine, False indica che la sorgente dati del grafico copiato non verrà modificata. True indica che la sorgente dati del grafico copiato fa riferimento al foglio di destinazione. |
| [SetReferToDestinationSheet](./setrefertodestinationsheet/) | Quando si copia l'intervallo nello stesso file e il grafico fa riferimento al foglio di origine, False indica che la sorgente dati del grafico copiato non verrà modificata. True indica che la sorgente dati del grafico copiato fa riferimento al foglio di destinazione. |
| [GetUpdateInvalidReferencesToTargetSheet](./getupdateinvalidreferencestotargetsheet/) | Indica se fare riferimento al foglio di lavoro di destinazione se il foglio di lavoro di riferimento non è stato copiato. |
| [SetUpdateInvalidReferencesToTargetSheet](./setupdateinvalidreferencestotargetsheet/) | Indica se fare riferimento al foglio di lavoro di destinazione se il foglio di lavoro di riferimento non è stato copiato. |
