---
title: "Класс ThreadInterruptMonitor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.ThreadInterruptMonitor класс. Простая реализация AbstractInterruptMonitor путем запуска другого потока, требующего прерывания после сна, заданного пользователем"
type: docs
url: /ru/net/aspose.cells/threadinterruptmonitor/
---
## ThreadInterruptMonitor class

Простая реализация [`AbstractInterruptMonitor`](../abstractinterruptmonitor/) путем запуска другого потока, требующего прерывания после сна, заданного пользователем.

```csharp
public class ThreadInterruptMonitor : AbstractInterruptMonitor
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ThreadInterruptMonitor](threadinterruptmonitor/)(bool) | Создаёт один монитор прерываний. |

## Свойства

| Имя | Описание |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/threadinterruptmonitor/isinterruptionrequested/) { get; } | Эта реализация просто проверяет, превышает ли затраченное время (от момента запуска этого монитора до текущего момента) заданное пользователем ограничение. |
| override [TerminateWithoutException](../../aspose.cells/threadinterruptmonitor/terminatewithoutexception/) { get; } | Смотрите [`TerminateWithoutException`](../abstractinterruptmonitor/terminatewithoutexception/). Это свойство задаётся пользователем при создании экземпляра этого монитора. |

## Методы

| Имя | Описание |
| --- | --- |
| [FinishMonitor](../../aspose.cells/threadinterruptmonitor/finishmonitor/)() | Завершает монитор для одной процедуры. |
| [StartMonitor](../../aspose.cells/threadinterruptmonitor/startmonitor/)(int) | Запускает монитор с указанным ограничением времени. Время начала для расчёта затраченного времени устанавливается в момент вызова этого метода, поэтому процедура, которую необходимо мониторить, должна быть запущена сразу после этого вызова. |

### Примечания

Один экземпляр монитора может использоваться многократно, при условии, что вы отслеживаете каждый процесс последовательно. Его не следует использовать для мониторинга нескольких процедур одновременно в многопоточной среде.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadInterruptMonitorDemo
    {
        public static void ThreadInterruptMonitorExample()
        {
            // Создайте экземпляр ThreadInterruptMonitor с параметром terminateWithoutException, установленным в false
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);

            // Создайте LoadOptions и установите InterruptMonitor в созданный монитор
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // Запустите монитор с ограничением времени в 1000 миллисекунд (1 секунда)
            monitor.StartMonitor(1000);

            try
            {
                // Загрузите книгу с указанными LoadOptions
                Workbook wb = new Workbook("Large.xlsx", lopts);

                // Завершите монитор для процедуры загрузки
                monitor.FinishMonitor();

                // Снова запустите монитор с новым ограничением времени в 1500 миллисекунд (1,5 секунды)
                monitor.StartMonitor(1500);

                // Сохраните книгу
                wb.Save("result.xlsx");

                // Завершите монитор для процедуры сохранения
                monitor.FinishMonitor();
            }
            catch (Exception ex)
            {
                Console.WriteLine("An exception occurred: " + ex.Message);
            }
        }
    }
}
```

### См. также

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


