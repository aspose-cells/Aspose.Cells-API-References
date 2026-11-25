---
title: "AbstractInterruptMonitor.TerminateWithoutException"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AbstractInterruptMonitor. Quando la procedura è interrotta, se terminare la procedura silenziosamente o lanciare un Exception. Il valore predefinito è false, cioè quando IsInterruptionRequested è true verrà lanciata una CellsException con codice Interrupted."
type: docs
url: /it/net/aspose.cells/abstractinterruptmonitor/terminatewithoutexception/
---
## AbstractInterruptMonitor.TerminateWithoutException property

Quando la procedura è interrotta, se terminare la procedura silenziosamente o lanciare un Exception. Il valore predefinito è false, cioè, quando [`IsInterruptionRequested`](../isinterruptionrequested/) è true, verrà lanciata una [`CellsException`](../../cellsexception/) con codice Interrupted.

```csharp
public virtual bool TerminateWithoutException { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractInterruptMonitorPropertyTerminateWithoutExceptionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola il foglio di lavoro per creare carico di elaborazione
            for (int row = 0; row < 5000; row++)
            {
                for (int col = 0; col < 50; col++)
                {
                    worksheet.Cells[row, col].Value = "SampleData";
                }
            }

            // Dimostra SystemTimeInterruptMonitor con terminazione tramite eccezione
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

            // Dimostra SystemTimeInterruptMonitor con terminazione silenziosa
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

### Vedi anche

* class [AbstractInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


