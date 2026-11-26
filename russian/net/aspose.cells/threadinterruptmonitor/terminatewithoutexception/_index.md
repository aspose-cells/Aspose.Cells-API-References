---
title: "ThreadInterruptMonitor.TerminateWithoutException"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreadInterruptMonitor. См. TerminateWithoutException. Это свойство задаётся пользователем при создании экземпляра монитора."
type: docs
url: /ru/net/aspose.cells/threadinterruptmonitor/terminatewithoutexception/
---
## ThreadInterruptMonitor.TerminateWithoutException property

См. [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/). Это свойство задаётся пользователем при создании экземпляра монитора.

```csharp
public override bool TerminateWithoutException { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadInterruptMonitorPropertyTerminateWithoutExceptionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте экземпляр ThreadInterruptMonitor с начальным значением TerminateWithoutException
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
            
            // Отобразите текущее значение свойства
            Console.WriteLine("Current TerminateWithoutException value: " + monitor.TerminateWithoutException);

            // Начните мониторинг с ограничением в 5 секунд
            monitor.StartMonitor(5000);

            // Продемонстрировать обработку, которая может быть прервана
            try
            {
                for (int i = 0; i < 100000; i++)
                {
                    // Смоделировать длительную обработку
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

            // Создать ещё один монитор с TerminateWithoutException, установленным в true
            ThreadInterruptMonitor silentMonitor = new ThreadInterruptMonitor(true);
            Console.WriteLine("\nNew monitor TerminateWithoutException value: " + silentMonitor.TerminateWithoutException);

            // Сохранить результат
            workbook.Save("PropertyTerminateWithoutExceptionDemo.xlsx");
        }
    }
}
```

### См. также

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


