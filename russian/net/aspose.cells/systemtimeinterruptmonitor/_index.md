---
title: "Класс SystemTimeInterruptMonitor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.SystemTimeInterruptMonitor. Простая реализация AbstractInterruptMonitor путем проверки и сравнения текущего системного времени с заданным пользователем ограничением"
type: docs
url: /ru/net/aspose.cells/systemtimeinterruptmonitor/
---
## SystemTimeInterruptMonitor class

Простая реализация [`AbstractInterruptMonitor`](../abstractinterruptmonitor/) путем проверки и сравнения текущего системного времени с заданным пользователем ограничением.

```csharp
public class SystemTimeInterruptMonitor : AbstractInterruptMonitor
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [SystemTimeInterruptMonitor](systemtimeinterruptmonitor/)(bool) | Создаёт один монитор прерываний. |

## Свойства

| Имя | Описание |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/systemtimeinterruptmonitor/isinterruptionrequested/) { get; } | Эта реализация просто проверяет, превышает ли затраченное время (от момента запуска этого монитора до текущего момента) заданное пользователем ограничение. |
| override [TerminateWithoutException](../../aspose.cells/systemtimeinterruptmonitor/terminatewithoutexception/) { get; } | Смотрите [`TerminateWithoutException`](../abstractinterruptmonitor/terminatewithoutexception/). Это свойство задаётся пользователем при создании экземпляра этого монитора. |

## Методы

| Имя | Описание |
| --- | --- |
| [StartMonitor](../../aspose.cells/systemtimeinterruptmonitor/startmonitor/)(int) | Запускает монитор с указанным ограничением времени. Время начала для расчёта затраченного времени устанавливается в момент вызова этого метода, поэтому процедура, которую необходимо мониторить, должна быть запущена сразу после этого вызова. |

### Примечания

Эта реализация представляет собой простое решение для простых сценариев. Она требует часто получать и проверять системное время, поэтому может в некоторой степени негативно влиять на производительность.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SystemTimeInterruptMonitorDemo
    {
        public static void SystemTimeInterruptMonitorExample()
        {
            // Создайте экземпляр SystemTimeInterruptMonitor с параметром terminateWithoutException, установленным в false
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // Создайте LoadOptions и установите InterruptMonitor в созданный монитор
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // Начните мониторинг с ограничением времени в 1000 миллисекунд (1 секунда)
            monitor.StartMonitor(1000);

            try
            {
                // Загрузите книгу с указанными LoadOptions
                Workbook wb = new Workbook("Large.xlsx", lopts);

                // Если время загрузки файла шаблона превышает одну секунду, потребуется прерывание, и здесь будет выброшено исключение
                // В противном случае начните мониторить процедуру сохранения с новым ограничением времени
                monitor.StartMonitor(1500); // time limit is 1.5 seconds

                // Сохраните книгу
                wb.Save("SystemTimeInterruptMonitorExample.xlsx");
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

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


