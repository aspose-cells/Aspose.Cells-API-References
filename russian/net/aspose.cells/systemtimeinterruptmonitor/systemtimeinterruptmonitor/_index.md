---
title: "SystemTimeInterruptMonitor.SystemTimeInterruptMonitor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор SystemTimeInterruptMonitor. Создаёт один монитор прерываний"
type: docs
url: /ru/net/aspose.cells/systemtimeinterruptmonitor/systemtimeinterruptmonitor/
---
## SystemTimeInterruptMonitor constructor

Создаёт один монитор прерываний.

```csharp
public SystemTimeInterruptMonitor(bool terminateWithoutException)
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
    public class SystemTimeInterruptMonitorMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Создайте экземпляр с параметром terminateWithoutException, установленным в false
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // Настройте параметры загрузки с монитором
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // Начните мониторинг с ограничением времени в 1 секунду
            monitor.StartMonitor(1000);

            try
            {
                // Попытка загрузить рабочую книгу
                Workbook wb = new Workbook("sample.xlsx", lopts);

                // Сбросить монитор для операции сохранения с ограничением в 1,5 секунды
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

### См. также

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


