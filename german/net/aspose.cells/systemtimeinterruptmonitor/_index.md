---
title: "Klasse SystemTimeInterruptMonitor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.SystemTimeInterruptMonitor Klasse. Einfache Implementierung von AbstractInterruptMonitor durch Überprüfen und Vergleichen der aktuellen Systemzeit mit dem vom Benutzer festgelegten Limit"
type: docs
url: /de/net/aspose.cells/systemtimeinterruptmonitor/
---
## SystemTimeInterruptMonitor class

Einfache Implementierung von [`AbstractInterruptMonitor`](../abstractinterruptmonitor/) durch Überprüfen und Vergleichen der aktuellen Systemzeit mit dem vom Benutzer festgelegten Limit.

```csharp
public class SystemTimeInterruptMonitor : AbstractInterruptMonitor
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [SystemTimeInterruptMonitor](systemtimeinterruptmonitor/)(bool) | Konstruiert einen Unterbrechungsmonitor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/systemtimeinterruptmonitor/isinterruptionrequested/) { get; } | Diese Implementierung prüft lediglich, ob die Zeitkosten (von dem Zeitpunkt, an dem dieser Monitor gestartet wurde, bis jetzt) größer sind als das vom Benutzer angegebene Limit. |
| override [TerminateWithoutException](../../aspose.cells/systemtimeinterruptmonitor/terminatewithoutexception/) { get; } | Siehe [`TerminateWithoutException`](../abstractinterruptmonitor/terminatewithoutexception/). Diese Eigenschaft wird vom Benutzer beim Erstellen dieser Monitorinstanz angegeben. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [StartMonitor](../../aspose.cells/systemtimeinterruptmonitor/startmonitor/)(int) | Startet den Monitor mit dem angegebenen Zeitlimit. Der Startzeitpunkt zur Berechnung der Zeitkosten ist genau der Moment, in dem diese Methode aufgerufen wird, sodass das zu überwachende Verfahren unmittelbar nach diesem Aufruf gestartet werden sollte. |

### Hinweise

Diese Implementierung ist lediglich eine einfache Lösung für einfache Szenarien. Sie muss häufig die Systemzeit abrufen und prüfen, sodass sie die Leistung in gewissem Maße negativ beeinflussen kann.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SystemTimeInterruptMonitorDemo
    {
        public static void SystemTimeInterruptMonitorExample()
        {
            // Erstellen Sie eine Instanz von SystemTimeInterruptMonitor mit terminateWithoutException auf false gesetzt.
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // Erstellen Sie LoadOptions und setzen Sie den InterruptMonitor auf den erstellten Monitor.
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // Starten Sie die Überwachung mit einem Zeitlimit von 1000 Millisekunden (1 Sekunde).
            monitor.StartMonitor(1000);

            try
            {
                // Laden Sie eine Arbeitsmappe mit den angegebenen LoadOptions.
                Workbook wb = new Workbook("Large.xlsx", lopts);

                // Wenn die Zeitkosten für das Laden der Vorlagendatei eine Sekunde überschreiten, ist eine Unterbrechung erforderlich und es wird hier eine Ausnahme ausgelöst.
                // Andernfalls starten Sie die Überwachung des Speicherverfahrens mit einem neuen Zeitlimit.
                monitor.StartMonitor(1500); // time limit is 1.5 seconds

                // Speichere die Arbeitsmappe
                wb.Save("SystemTimeInterruptMonitorExample.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Operation interrupted: " + ex.Message);
            }
        }
    }
}
```

### Siehe auch

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


