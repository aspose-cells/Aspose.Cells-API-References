---
title: "AbstractInterruptMonitor.IsInterruptionRequested"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractInterruptMonitor property. Anger om avbrott begärs för den aktuella operationen. Om true avbryts då den aktuella operationen. Implementeringen bör utföra en snabb och effektiv kontroll här, annars kan den bli en flaskhals för proceduren."
type: docs
url: /sv/net/aspose.cells/abstractinterruptmonitor/isinterruptionrequested/
---
## AbstractInterruptMonitor.IsInterruptionRequested property

Anger om avbrott begärs för den aktuella operationen. Om sant kommer den aktuella operationen att avbrytas. Implementeringen bör utföra en snabb och effektiv kontroll här, annars kan den bli en flaskhals för proceduren.

```csharp
public abstract bool IsInterruptionRequested { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa avbrottsövervakare och tilldela till arbetsbok
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;

            // Visa initialt värde
            Console.WriteLine("Initial IsInterruptionRequested: " + monitor.IsInterruptionRequested);

            // Starta avbrottsuppgift
            Task.Run(() =>
            {
                Thread.Sleep(1000); // Wait 1 seconds
                Console.WriteLine("\nTriggering interruption...");
                monitor.Interrupt();
            });

            // Simulering av långvarig operation
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
                    
                    // Simulera bearbetningstid
                    if (i % 1000 == 0) 
                        Console.Write(".");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine("\nError: " + ex.Message);
            }

            // Spara resultatet
            workbook.Save("InterruptionDemoOutput.xlsx");

            Console.WriteLine("\nWorkbook saved with partial data.");
        }
    }
}
```

### Se även

* class [AbstractInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


