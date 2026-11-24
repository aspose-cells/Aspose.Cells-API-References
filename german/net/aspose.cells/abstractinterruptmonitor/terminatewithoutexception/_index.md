---
title: "AbstractInterruptMonitor.TerminateWithoutException"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AbstractInterruptMonitor-Eigenschaft. Gibt an, ob das Verfahren bei einer Unterbrechung stillschweigend beendet oder eine Ausnahme ausgelöst werden soll. Standardwert ist false, das heißt, wenn IsInterruptionRequested true ist, wird eine CellsException mit dem Code Interrupted ausgelöst."
type: docs
url: /de/net/aspose.cells/abstractinterruptmonitor/terminatewithoutexception/
---
## AbstractInterruptMonitor.TerminateWithoutException property

Wenn das Verfahren unterbrochen wird, ob es stillschweigend beendet oder eine Ausnahme ausgelöst werden soll. Standardwert ist false, das heißt, wenn [`IsInterruptionRequested`](../isinterruptionrequested/) true ist, wird eine [`CellsException`](../../cellsexception/) mit dem Code Interrupted ausgelöst.

```csharp
public virtual bool TerminateWithoutException { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractInterruptMonitorPropertyTerminateWithoutExceptionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Arbeitsblatt befüllen, um Arbeitslast zu erzeugen
            for (int row = 0; row < 5000; row++)
            {
                for (int col = 0; col < 50; col++)
                {
                    worksheet.Cells[row, col].Value = "SampleData";
                }
            }

            // Demonstriere SystemTimeInterruptMonitor mit Ausnahmebeendigung
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

            // Demonstriere SystemTimeInterruptMonitor mit stiller Beendigung
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

### Siehe auch

* class [AbstractInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


