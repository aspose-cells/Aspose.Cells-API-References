---
title: "SystemTimeInterruptMonitor.TerminateWithoutException"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SystemTimeInterruptMonitor Eigenschaft. Siehe TerminateWithoutException. Diese Eigenschaft wird vom Benutzer angegeben, wenn diese Überwachungsinstanz erstellt wird."
type: docs
url: /de/net/aspose.cells/systemtimeinterruptmonitor/terminatewithoutexception/
---
## SystemTimeInterruptMonitor.TerminateWithoutException property

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

    public class SystemTimeInterruptMonitorPropertyTerminateWithoutExceptionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie eine Instanz von SystemTimeInterruptMonitor mit dem anfänglichen TerminateWithoutException-Wert
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // Zeigen Sie den aktuellen Wert der TerminateWithoutException-Eigenschaft an
            Console.WriteLine("Current TerminateWithoutException value: " + monitor.TerminateWithoutException);

            // Starten Sie die Überwachung mit einem Zeitlimit von 1000ms
            monitor.StartMonitor(1000);

            // Demonstrieren Sie die Wirkung von TerminateWithoutException, indem Sie einen langen Vorgang versuchen
            try
            {
                // Simulieren Sie einen langen Vorgang, der das Zeitlimit überschreiten könnte
                for (int i = 0; i < 100000; i++)
                {
                    worksheet.Cells[i, 0].Value = i;
                    if (monitor.IsInterruptionRequested)
                    {
                        Console.WriteLine("Operation interrupted by monitor");
                        break;
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception caught: " + ex.Message);
            }

            // Erstellen Sie einen weiteren Monitor mit TerminateWithoutException auf true gesetzt
            SystemTimeInterruptMonitor monitorNoException = new SystemTimeInterruptMonitor(true);
            Console.WriteLine("New monitor TerminateWithoutException value: " + monitorNoException.TerminateWithoutException);

            // Speichere die Arbeitsmappe
            workbook.Save("PropertyTerminateWithoutExceptionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


