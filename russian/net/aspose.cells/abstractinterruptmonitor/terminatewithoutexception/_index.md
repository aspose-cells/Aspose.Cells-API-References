---
title: "AbstractInterruptMonitor.TerminateWithoutException"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AbstractInterruptMonitor. Когда процедура прерывается, следует ли завершать её тихо или бросать исключение. По умолчанию false, то есть когда IsInterruptionRequested истинно, будет выброшено CellsException с кодом Interrupted."
type: docs
url: /ru/net/aspose.cells/abstractinterruptmonitor/terminatewithoutexception/
---
## AbstractInterruptMonitor.TerminateWithoutException property

Когда процедура прерывается, следует ли завершать её тихо или бросать исключение. По умолчанию false, то есть когда [`IsInterruptionRequested`](../isinterruptionrequested/) истинно, будет выброшено [`CellsException`](../../cellsexception/) с кодом Interrupted.

```csharp
public virtual bool TerminateWithoutException { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractInterruptMonitorPropertyTerminateWithoutExceptionDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполните лист для создания нагрузки обработки
            for (int row = 0; row < 5000; row++)
            {
                for (int col = 0; col < 50; col++)
                {
                    worksheet.Cells[row, col].Value = "SampleData";
                }
            }

            // Продемонстрировать SystemTimeInterruptMonitor с завершением через исключение
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

            // Продемонстрировать SystemTimeInterruptMonitor с тихим завершением
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

### См. также

* class [AbstractInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


