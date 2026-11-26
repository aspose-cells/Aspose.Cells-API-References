---
title: "SystemTimeInterruptMonitor.TerminateWithoutException"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SystemTimeInterruptMonitor. См. TerminateWithoutException. Это свойство задаётся пользователем при создании экземпляра монитора"
type: docs
url: /ru/net/aspose.cells/systemtimeinterruptmonitor/terminatewithoutexception/
---
## SystemTimeInterruptMonitor.TerminateWithoutException property

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

    public class SystemTimeInterruptMonitorPropertyTerminateWithoutExceptionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать экземпляр SystemTimeInterruptMonitor с начальным значением TerminateWithoutException
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // Отобразить текущее значение свойства TerminateWithoutException
            Console.WriteLine("Current TerminateWithoutException value: " + monitor.TerminateWithoutException);

            // Начать мониторинг с ограничением времени в 1000 мс
            monitor.StartMonitor(1000);

            // Продемонстрировать эффект TerminateWithoutException, попыткой выполнить длительную операцию
            try
            {
                // Смоделировать длительную операцию, которая может превысить ограничение времени
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

            // Создать ещё один монитор с TerminateWithoutException, установленным в true
            SystemTimeInterruptMonitor monitorNoException = new SystemTimeInterruptMonitor(true);
            Console.WriteLine("New monitor TerminateWithoutException value: " + monitorNoException.TerminateWithoutException);

            // Сохраните книгу
            workbook.Save("PropertyTerminateWithoutExceptionDemo.xlsx");
        }
    }
}
```

### См. также

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


