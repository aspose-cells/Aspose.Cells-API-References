---
title: "Classe SystemTimeInterruptMonitor"
linktitle: "SystemTimeInterruptMonitor"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe SystemTimeInterruptMonitor. Incapsula l'oggetto che rappresenta systemtimeinterruptmonitor in Go."
type: docs
weight: 200
url: /it/go-cpp/systemtimeinterruptmonitor/
---

## SystemTimeInterruptMonitor class

Implementazione semplice di <see cref="AbstractInterruptMonitor"/> controllando e confrontando l'ora di sistema corrente con il limite specificato dall'utente.

```go

type SystemTimeInterruptMonitor struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewSystemTimeInterruptMonitor](./newsystemtimeinterruptmonitor/) | Costruisce un monitor di interruzione. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [StartMonitor](./startmonitor/) | Avvia il monitor con il limite di tempo specificato. Il tempo di avvio per calcolare il tempo impiegato è proprio quando questo metodo viene chiamato, quindi la procedura che deve essere monitorata dovrebbe essere avviata subito dopo questa chiamata. |
| [IsInterruptionRequested](./isinterruptionrequested/) | Questa implementazione verifica semplicemente se il tempo impiegato (dal momento in cui si avvia questo monitor fino a ora) è superiore al limite specificato dall'utente. |
| [GetTerminateWithoutException](./getterminatewithoutexception/) | Vedi AbstractInterruptMonitor.TerminateWithoutException. Questa proprietà è specificata dall'utente durante la costruzione di questa istanza di monitor. |
