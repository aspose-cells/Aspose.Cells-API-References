---
title: "SystemTimeInterruptMonitor Klasse"
linktitle: "SystemTimeInterruptMonitor"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "SystemTimeInterruptMonitor-Klasse. Kapselt das Objekt, das systemtimeinterruptmonitor in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/systemtimeinterruptmonitor/
---

## SystemTimeInterruptMonitor class

Einfache Implementierung von <see cref="AbstractInterruptMonitor"/> durch Überprüfen und Vergleichen der aktuellen Systemzeit mit dem vom Benutzer festgelegten Limit.

```go

type SystemTimeInterruptMonitor struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewSystemTimeInterruptMonitor](./newsystemtimeinterruptmonitor/) | Konstruiert einen Unterbrechungsmonitor. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [StartMonitor](./startmonitor/) | Startet den Monitor mit dem angegebenen Zeitlimit. Der Startzeitpunkt zur Berechnung der Zeitkosten ist genau dann, wenn diese Methode aufgerufen wird, sodass das zu überwachende Verfahren unmittelbar nach diesem Aufruf gestartet werden sollte. |
| [IsInterruptionRequested](./isinterruptionrequested/) | Diese Implementierung prüft lediglich, ob die Zeitkosten (vom Start dieses Monitors bis jetzt) größer sind als das vom Benutzer angegebene Limit. |
| [GetTerminateWithoutException](./getterminatewithoutexception/) | Siehe AbstractInterruptMonitor.TerminateWithoutException. Diese Eigenschaft wird vom Benutzer beim Erzeugen dieser Monitorinstanz angegeben. |
