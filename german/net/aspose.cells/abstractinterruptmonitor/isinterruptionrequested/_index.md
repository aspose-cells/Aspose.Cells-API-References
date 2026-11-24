---
title: "AbstractInterruptMonitor.IsInterruptionRequested"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AbstractInterruptMonitor-Eigenschaft. Gibt an, ob für den aktuellen Vorgang eine Unterbrechung angefordert wird. Wenn true, wird der aktuelle Vorgang unterbrochen. Die Implementierung sollte hier eine schnelle und effiziente Prüfung durchführen, da sie sonst zu einem weiteren Engpass im Verfahren werden kann."
type: docs
url: /de/net/aspose.cells/abstractinterruptmonitor/isinterruptionrequested/
---
## AbstractInterruptMonitor.IsInterruptionRequested property

Gibt an, ob für den aktuellen Vorgang eine Unterbrechung angefordert wird. Wenn true, wird der aktuelle Vorgang unterbrochen. Die Implementierung sollte hier eine schnelle und effiziente Prüfung durchführen, sonst könnte sie zum weiteren Engpass für den Vorgang werden.

```csharp
public abstract bool IsInterruptionRequested { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Threading;
    using System.Threading.Tasks;

    public class AbstractInterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle einen Unterbrechungsmonitor und weise ihn dem Arbeitsbuch zu
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;

            // Anfangswert anzeigen
            Console.WriteLine("Initial IsInterruptionRequested: " + monitor.IsInterruptionRequested);

            // Unterbrechungsaufgabe starten
            Task.Run(() =>
            {
                Thread.Sleep(1000); // Wait 1 seconds
                Console.WriteLine("\nTriggering interruption...");
                monitor.Interrupt();
            });

            // Simulation einer langlaufenden Operation
            Console.WriteLine("Starting data generation...");
            try
            {
                for (int i = 0; i < 500000000; i++)
                {
                    if (monitor.IsInterruptionRequested)
                    {
                        Console.WriteLine($"\nInterrupted at row {i}");
                        break;
                    }

                    worksheet.Cells[i, 0].Value = $"Data {i}";
                    
                    // Verarbeitungszeit simulieren
                    if (i % 1000 == 0) 
                        Console.Write(".");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine("\nError: " + ex.Message);
            }

            // Ergebnis speichern
            workbook.Save("InterruptionDemoOutput.xlsx");

            Console.WriteLine("\nWorkbook saved with partial data.");
        }
    }
}
```

### Siehe auch

* class [AbstractInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


