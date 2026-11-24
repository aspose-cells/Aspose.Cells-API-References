---
title: "InterruptMonitor.IsInterruptionRequested"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "InterruptMonitor-Eigenschaft. Markieren Sie den Monitor als Anforderung einer Unterbrechung"
type: docs
url: /de/net/aspose.cells/interruptmonitor/isinterruptionrequested/
---
## InterruptMonitor.IsInterruptionRequested property

Den Monitor als Unterbrechungsanforderung markieren

```csharp
public override bool IsInterruptionRequested { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class InterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und greifen Sie auf ihr erstes Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie einen Interrupt-Monitor und weisen Sie ihn der Arbeitsmappe zu
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;

            // Zeigen Sie den Anfangszustand von IsInterruptionRequested an
            Console.WriteLine("Initial IsInterruptionRequested value: " + monitor.IsInterruptionRequested);

            // Simulieren Sie einen langlaufenden Datenverarbeitungsvorgang
            Console.WriteLine("Starting data processing...");
            for (int rowIdx = 0; rowIdx < 10000; rowIdx++)
            {
                // Fordern Sie eine Unterbrechung nach der Verarbeitung von 500 Zeilen an
                if (rowIdx == 500)
                {
                    monitor.Interrupt();
                    Console.WriteLine("Interrupt requested. IsInterruptionRequested: " + monitor.IsInterruptionRequested);
                }

                // Prüfen Sie, ob eine Unterbrechungsanforderung vorliegt
                if (monitor.IsInterruptionRequested)
                {
                    Console.WriteLine($"Processing interrupted at row {rowIdx}");
                    break;
                }

                // Simulieren Sie die Datenverarbeitung
                worksheet.Cells[rowIdx, 0].Value = $"Row {rowIdx} data";
            }

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("InterruptionDemoOutput.xlsx");
            Console.WriteLine("File saved with partial data due to interruption.");
        }
    }
}
```

### Siehe auch

* class [InterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


