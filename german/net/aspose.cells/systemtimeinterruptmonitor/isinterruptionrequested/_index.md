---
title: "SystemTimeInterruptMonitor.IsInterruptionRequested"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SystemTimeInterruptMonitor-Eigenschaft. Diese Implementierung prüft lediglich, ob die Zeitdauer seit dem Start dieses Monitors bis jetzt größer ist als das vom Benutzer angegebene Limit."
type: docs
url: /de/net/aspose.cells/systemtimeinterruptmonitor/isinterruptionrequested/
---
## SystemTimeInterruptMonitor.IsInterruptionRequested property

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

    public class SystemTimeInterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Instanz von SystemTimeInterruptMonitor
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);
            
            // Starte die Überwachung mit einem Zeitlimit von 5 Sekunden
            monitor.StartMonitor(5000);

            // Zeige den anfänglichen IsInterruptionRequested-Wert an
            Console.WriteLine("Initial IsInterruptionRequested: " + monitor.IsInterruptionRequested);

            // Simuliere einen langlaufenden Vorgang
            Console.WriteLine("Starting long operation...");
            for (int i = 0; i < 100000; i++)
            {
                worksheet.Cells[i, 0].Value = i;
                
                // Prüfe, ob eine Unterbrechung angefordert wurde
                if (monitor.IsInterruptionRequested)
                {
                    Console.WriteLine("Operation interrupted after time limit!");
                    break;
                }
            }

            // Zeige den finalen IsInterruptionRequested-Wert an
            Console.WriteLine("Final IsInterruptionRequested: " + monitor.IsInterruptionRequested);

            // Ergebnis speichern
            workbook.Save("PropertyIsInterruptionRequestedDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


