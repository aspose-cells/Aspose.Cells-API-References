---
title: "Classe AbstractLowCodeSaveOptionsProvider"
linktitle: "AbstractLowCodeSaveOptionsProvider"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "AbstractLowCodeSaveOptionsProvider classe. Incapsula l'oggetto che rappresenta abstractlowcodesaveoptionsprovider in Go."
type: docs
weight: 200
url: /it/go-cpp/abstractlowcodesaveoptionsprovider/
---

## AbstractLowCodeSaveOptionsProvider class

Implementazione per fornire opzioni di salvataggio multiple per processi che richiedono output multipli. Ad esempio, la funzionalità <see cref="SpreadsheetSplitter"/> richiede destinazioni multiple per salvare i file divisi.

```go

type AbstractLowCodeSaveOptionsProvider struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetSaveOptions](./getsaveoptions/) | Ottiene le opzioni di salvataggio da cui ottenere le impostazioni di output per la parte attualmente divisa.Restituire null indica di saltare la parte specificata. |
| [Finish](./finish/) | Rilascia le risorse dopo l'elaborazione della parte attualmente divisa. |
