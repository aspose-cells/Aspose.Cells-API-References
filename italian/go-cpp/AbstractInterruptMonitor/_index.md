---
title: "AbstractInterruptMonitor Classe"
linktitle: "AbstractInterruptMonitor"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe AbstractInterruptMonitor. Incapsula l'oggetto che rappresenta abstractinterruptmonitor in Go."
type: docs
weight: 200
url: /it/go-cpp/abstractinterruptmonitor/
---

## AbstractInterruptMonitor class

Monitor per le richieste di interruzione in tutte le operazioni che richiedono tempo.

```go

type AbstractInterruptMonitor struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [GetTerminateWithoutException](./getterminatewithoutexception/) | Quando la procedura viene interrotta, se terminare la procedura silenziosamente o lanciare un'eccezione. Il valore predefinito è false, cioè, quando IsInterruptionRequested è true, verrà lanciata una CellsException con codice ExceptionType.Interrupted. |
