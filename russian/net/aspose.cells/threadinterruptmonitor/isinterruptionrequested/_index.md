---
title: "ThreadInterruptMonitor.IsInterruptionRequested"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreadInterruptMonitor. Эта реализация просто проверяет, превышает ли затраченное время с момента запуска этого монитора до текущего момента пользовательский лимит."
type: docs
url: /ru/net/aspose.cells/threadinterruptmonitor/isinterruptionrequested/
---
## ThreadInterruptMonitor.IsInterruptionRequested property

Эта реализация просто проверяет, превышает ли затраченное время (от момента запуска этого монитора до текущего момента) заданное пользователем ограничение.

```csharp
public override bool IsInterruptionRequested { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Threading;

    public class ThreadInterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте экземпляр ThreadInterruptMonitor
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(terminateWithoutException: false);

            // Начните мониторинг с ограничением в 2 секунды
            monitor.StartMonitor(2000);

            // Смоделируйте длительную операцию
            Console.WriteLine("Starting long operation...");
            for (int i = 0; i < 100; i++)
            {
                // Проверить, было ли запрошено прерывание
                if (monitor.IsInterruptionRequested)
                {
                    Console.WriteLine("Operation was interrupted!");
                    break;
                }

                // Смоделируйте работу
                Thread.Sleep(100);
                worksheet.Cells[i, 0].Value = $"Processed row {i}";
                Console.WriteLine($"Processed row {i}");
            }

            // Завершите мониторинг
            monitor.FinishMonitor();

            // Сохранить результат
            workbook.Save("ThreadInterruptionDemo.xlsx");
        }
    }
}
```

### См. также

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


