---
title: "AbstractInterruptMonitor-Klasse"
linktitle: "AbstractInterruptMonitor"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "AbstractInterruptMonitor-Klasse. Kapselt das Objekt, das abstractinterruptmonitor in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/abstractinterruptmonitor/
---

## AbstractInterruptMonitor class

Überwacht Unterbrechungsanfragen bei allen zeitaufwändigen Vorgängen.

```go

type AbstractInterruptMonitor struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [GetTerminateWithoutException](./getterminatewithoutexception/) | Wenn das Verfahren unterbrochen wird, ob das Verfahren stillschweigend beendet oder eine Ausnahme ausgelöst wird. Standard ist false, das heißt, wenn IsInterruptionRequested true ist, wird eine CellsException mit dem Code ExceptionType.Interrupted ausgelöst. |
