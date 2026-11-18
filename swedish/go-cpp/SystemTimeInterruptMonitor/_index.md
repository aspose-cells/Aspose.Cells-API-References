---
title: "SystemTimeInterruptMonitor klass"
linktitle: "SystemTimeInterruptMonitor"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "SystemTimeInterruptMonitor class. Inkapslar objektet som representerar systemtimeinterruptmonitor i Go."
type: docs
weight: 200
url: /sv/go-cpp/systemtimeinterruptmonitor/
---

## SystemTimeInterruptMonitor class

Enkel implementering av <see cref=\"AbstractInterruptMonitor\"/> genom att kontrollera och jämföra aktuell systemtid med användarspecificerad gräns.

```go

type SystemTimeInterruptMonitor struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewSystemTimeInterruptMonitor](./newsystemtimeinterruptmonitor/) | Skapar en avbrottsmonitor. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [StartMonitor](./startmonitor/) | Startar monitorn med den angivna tidsgränsen. Starttiden för att beräkna tidskostnad är precis när den här metoden anropas, så proceduren som behöver övervakas bör startas omedelbart efter detta anrop. |
| [IsInterruptionRequested](./isinterruptionrequested/) | Denna implementation kontrollerar bara om tidskostnaden (från tiden då monitorn startas till nu) är större än den av användaren angivna gränsen. |
| [GetTerminateWithoutException](./getterminatewithoutexception/) | Se AbstractInterruptMonitor.TerminateWithoutException. Denna egenskap specificeras av användaren när denna monitorinstans konstrueras. |
