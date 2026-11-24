---
title: "SystemTimeInterruptMonitor.SystemTimeInterruptMonitor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SystemTimeInterruptMonitor-Konstruktor. Erstellt einen Unterbrechungsmonitor"
type: docs
url: /de/net/aspose.cells/systemtimeinterruptmonitor/systemtimeinterruptmonitor/
---
## SystemTimeInterruptMonitor constructor

Konstruiert einen Unterbrechungsmonitor.

```csharp
public SystemTimeInterruptMonitor(bool terminateWithoutException)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| terminateWithoutException | Boolean | [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/) |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SystemTimeInterruptMonitorMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Erstelle eine Instanz mit terminateWithoutException auf false gesetzt
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // Richte Ladeoptionen mit dem Monitor ein
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // Starte die Überwachung mit einem Zeitlimit von 1 Sekunde
            monitor.StartMonitor(1000);

            try
            {
                // Versuche, eine Arbeitsmappe zu laden
                Workbook wb = new Workbook("sample.xlsx", lopts);

                // Setze den Monitor für den Speichervorgang mit einem Zeitlimit von 1,5 Sekunden zurück
                monitor.StartMonitor(1500);
                wb.Save("output.xlsx");
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

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


