---
title: "AbstractInterruptMonitor.TerminateWithoutException"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractInterruptMonitor property. När proceduren avbryts, om den ska avslutas tyst eller kasta ett undantag. Standard är false, vilket betyder att när IsInterruptionRequested är true kommer ett CellsException med koden Interrupted att kastas."
type: docs
url: /sv/net/aspose.cells/abstractinterruptmonitor/terminatewithoutexception/
---
## AbstractInterruptMonitor.TerminateWithoutException property

När proceduren avbryts, om den ska avslutas tyst eller kasta ett undantag. Standard är false, det vill säga, när [`IsInterruptionRequested`](../isinterruptionrequested/) är true, kommer ett [`CellsException`](../../cellsexception/) med koden Interrupted att kastas.

```csharp
public virtual bool TerminateWithoutException { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractInterruptMonitorPropertyTerminateWithoutExceptionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll i kalkylblad för att skapa bearbetningsbelastning
            for (int row = 0; row < 5000; row++)
            {
                for (int col = 0; col < 50; col++)
                {
                    worksheet.Cells[row, col].Value = "SampleData";
                }
            }

            // Demonstrera SystemTimeInterruptMonitor med undantagsavslut
            var interruptMonitor1 = new SystemTimeInterruptMonitor(terminateWithoutException: false);
            Console.WriteLine($"Initial TerminateWithoutException: {interruptMonitor1.TerminateWithoutException}");

            workbook.InterruptMonitor = interruptMonitor1;
            interruptMonitor1.StartMonitor(1); // Set 1ms timeout

            try
            {
                workbook.Save("TerminateWithException.xlsx");
                Console.WriteLine("Saved successfully (unexpected with false setting)");
            }
            catch (CellsException ex)
            {
                Console.WriteLine($"Operation terminated with exception: {ex.Message}");
            }

            // Demonstrera SystemTimeInterruptMonitor med tyst avslut
            var interruptMonitor2 = new SystemTimeInterruptMonitor(terminateWithoutException: true);
            Console.WriteLine($"\nNew TerminateWithoutException: {interruptMonitor2.TerminateWithoutException}");

            workbook.InterruptMonitor = interruptMonitor2;
            interruptMonitor2.StartMonitor(1);

            try
            {
                workbook.Save("TerminateSilently.xlsx");
                Console.WriteLine("Saved without exception (expected with true setting)");
            }
            catch (CellsException)
            {
                Console.WriteLine("Exception caught (unexpected with true setting)");
            }

        }
    }

}
```

### Se även

* class [AbstractInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


