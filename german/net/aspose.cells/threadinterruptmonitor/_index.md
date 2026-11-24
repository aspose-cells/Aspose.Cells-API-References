---
title: "Klasse ThreadInterruptMonitor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ThreadInterruptMonitor‑Klasse. Einfache Implementierung von AbstractInterruptMonitor, indem ein weiterer Thread gestartet wird, der nach einer vom Benutzer angegebenen Wartezeit die Unterbrechung verlangt."
type: docs
url: /de/net/aspose.cells/threadinterruptmonitor/
---
## ThreadInterruptMonitor class

Einfache Implementierung von [`AbstractInterruptMonitor`](../abstractinterruptmonitor/), indem ein weiterer Thread gestartet wird, der nach einer vom Benutzer angegebenen Wartezeit die Unterbrechung verlangt.

```csharp
public class ThreadInterruptMonitor : AbstractInterruptMonitor
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [ThreadInterruptMonitor](threadinterruptmonitor/)(bool) | Konstruiert einen Unterbrechungsmonitor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/threadinterruptmonitor/isinterruptionrequested/) { get; } | Diese Implementierung prüft lediglich, ob die Zeitkosten (von dem Zeitpunkt, an dem dieser Monitor gestartet wurde, bis jetzt) größer sind als das vom Benutzer angegebene Limit. |
| override [TerminateWithoutException](../../aspose.cells/threadinterruptmonitor/terminatewithoutexception/) { get; } | Siehe [`TerminateWithoutException`](../abstractinterruptmonitor/terminatewithoutexception/). Diese Eigenschaft wird vom Benutzer beim Erstellen dieser Monitorinstanz angegeben. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [FinishMonitor](../../aspose.cells/threadinterruptmonitor/finishmonitor/)() | Beendet den Monitor für einen Vorgang. |
| [StartMonitor](../../aspose.cells/threadinterruptmonitor/startmonitor/)(int) | Startet den Monitor mit dem angegebenen Zeitlimit. Der Startzeitpunkt zur Berechnung der Zeitkosten ist genau der Moment, in dem diese Methode aufgerufen wird, sodass das zu überwachende Verfahren unmittelbar nach diesem Aufruf gestartet werden sollte. |

### Hinweise

Eine Monitor‑Instanz kann wiederholt verwendet werden, solange Sie jeden Prozess nacheinander überwachen. Sie sollte nicht verwendet werden, um mehrere Vorgänge gleichzeitig in mehreren Threads zu überwachen.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadInterruptMonitorDemo
    {
        public static void ThreadInterruptMonitorExample()
        {
            // Erstellen Sie eine Instanz von ThreadInterruptMonitor mit terminateWithoutException auf false gesetzt
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);

            // Erstellen Sie LoadOptions und setzen Sie den InterruptMonitor auf den erstellten Monitor.
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // Starten Sie den Monitor mit einem Zeitlimit von 1000 Millisekunden (1 Sekunde)
            monitor.StartMonitor(1000);

            try
            {
                // Laden Sie eine Arbeitsmappe mit den angegebenen LoadOptions.
                Workbook wb = new Workbook("Large.xlsx", lopts);

                // Beenden Sie den Monitor für den Ladevorgang
                monitor.FinishMonitor();

                // Starten Sie den Monitor erneut mit einer neuen Zeitbegrenzung von 1500 Millisekunden (1,5 Sekunden)
                monitor.StartMonitor(1500);

                // Speichere die Arbeitsmappe
                wb.Save("result.xlsx");

                // Beenden Sie den Monitor für den Speicherungsprozess
                monitor.FinishMonitor();
            }
            catch (Exception ex)
            {
                Console.WriteLine("An exception occurred: " + ex.Message);
            }
        }
    }
}
```

### Siehe auch

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


