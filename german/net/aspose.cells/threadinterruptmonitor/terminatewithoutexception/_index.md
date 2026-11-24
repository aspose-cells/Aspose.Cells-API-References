---
title: "ThreadInterruptMonitor.TerminateWithoutException"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreadInterruptMonitor-Eigenschaft. Siehe TerminateWithoutException. Diese Eigenschaft wird vom Benutzer beim Erzeugen dieser Monitorinstanz angegeben."
type: docs
url: /de/net/aspose.cells/threadinterruptmonitor/terminatewithoutexception/
---
## ThreadInterruptMonitor.TerminateWithoutException property

Siehe [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/). Diese Eigenschaft wird vom Benutzer angegeben, wenn diese Überwachungsinstanz erstellt wird.

```csharp
public override bool TerminateWithoutException { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadInterruptMonitorPropertyTerminateWithoutExceptionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Instanz von ThreadInterruptMonitor mit dem anfänglichen TerminateWithoutException‑Wert
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
            
            // Den aktuellen Wert der Eigenschaft anzeigen
            Console.WriteLine("Current TerminateWithoutException value: " + monitor.TerminateWithoutException);

            // Überwachung starten mit einer 5‑Sekunden‑Grenze
            monitor.StartMonitor(5000);

            // Verarbeitung demonstrieren, die unterbrochen werden könnte
            try
            {
                for (int i = 0; i < 100000; i++)
                {
                    // Lange Verarbeitung simulieren
                    if (monitor.IsInterruptionRequested)
                    {
                        Console.WriteLine("Processing was interrupted");
                        break;
                    }
                    worksheet.Cells[i, 0].Value = "Value " + i;
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception occurred: " + ex.Message);
            }
            finally
            {
                monitor.FinishMonitor();
            }

            // Erstellen Sie einen weiteren Monitor mit TerminateWithoutException auf true gesetzt
            ThreadInterruptMonitor silentMonitor = new ThreadInterruptMonitor(true);
            Console.WriteLine("\nNew monitor TerminateWithoutException value: " + silentMonitor.TerminateWithoutException);

            // Ergebnis speichern
            workbook.Save("PropertyTerminateWithoutExceptionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


