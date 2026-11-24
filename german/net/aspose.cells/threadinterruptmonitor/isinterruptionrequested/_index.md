---
title: "ThreadInterruptMonitor.IsInterruptionRequested"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreadInterruptMonitor-Eigenschaft. Diese Implementierung prüft lediglich, ob die seit dem Start dieses Monitors bis jetzt verstrichene Zeit den vom Benutzer angegebenen Grenzwert überschreitet."
type: docs
url: /de/net/aspose.cells/threadinterruptmonitor/isinterruptionrequested/
---
## ThreadInterruptMonitor.IsInterruptionRequested property

Diese Implementierung prüft lediglich, ob die Zeitkosten (von dem Zeitpunkt, an dem dieser Monitor gestartet wurde, bis jetzt) größer sind als das vom Benutzer angegebene Limit.

```csharp
public override bool IsInterruptionRequested { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Threading;

    public class ThreadInterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Instanz von ThreadInterruptMonitor erstellen
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(terminateWithoutException: false);

            // Überwachung starten mit einer 2‑Sekunden‑Grenze
            monitor.StartMonitor(2000);

            // Eine langlaufende Operation simulieren
            Console.WriteLine("Starting long operation...");
            for (int i = 0; i < 100; i++)
            {
                // Prüfe, ob eine Unterbrechung angefordert wurde
                if (monitor.IsInterruptionRequested)
                {
                    Console.WriteLine("Operation was interrupted!");
                    break;
                }

                // Arbeit simulieren
                Thread.Sleep(100);
                worksheet.Cells[i, 0].Value = $"Processed row {i}";
                Console.WriteLine($"Processed row {i}");
            }

            // Überwachung beenden
            monitor.FinishMonitor();

            // Ergebnis speichern
            workbook.Save("ThreadInterruptionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


