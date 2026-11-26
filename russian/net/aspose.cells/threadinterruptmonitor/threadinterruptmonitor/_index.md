---
title: "ThreadInterruptMonitor.ThreadInterruptMonitor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор ThreadInterruptMonitor. Создаёт один монитор прерываний"
type: docs
url: /ru/net/aspose.cells/threadinterruptmonitor/threadinterruptmonitor/
---
## ThreadInterruptMonitor constructor

Создаёт один монитор прерываний.

```csharp
public ThreadInterruptMonitor(bool terminateWithoutException)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| terminateWithoutException | Boolean | [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/) |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadInterruptMonitorMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Создайте ThreadInterruptMonitor с параметром throwOnInterrupted, установленным в false
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
            workbook.InterruptMonitor = monitor;
            
            // Установите короткий временной предел (100 мс) для демонстрации
            int timeLimit = 100;
            monitor.StartMonitor(timeLimit);

            try
            {
                // Выполните длительную операцию (будет прервана)
                for (int i = 0; i < 100000; i++)
                {
                    workbook.Worksheets[0].Cells[i % 100, i / 100].PutValue(i);
                }
                
                Console.WriteLine("Operation completed without interruption");
            }
            catch (CellsException e)
            {
                if (e.Code == ExceptionType.Interrupted)
                {
                    Console.WriteLine("Operation was successfully interrupted");
                }
                else
                {
                    Console.WriteLine("Error occurred: " + e.Message);
                }
            }
        }
    }
}
```

### См. также

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


