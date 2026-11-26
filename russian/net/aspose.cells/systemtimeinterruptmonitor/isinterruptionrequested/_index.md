---
title: "SystemTimeInterruptMonitor.IsInterruptionRequested"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SystemTimeInterruptMonitor. Эта реализация просто проверяет, превышает ли затраченное время от момента запуска этого монитора до текущего момента пользовательский заданный предел"
type: docs
url: /ru/net/aspose.cells/systemtimeinterruptmonitor/isinterruptionrequested/
---
## SystemTimeInterruptMonitor.IsInterruptionRequested property

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

    public class SystemTimeInterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать экземпляр SystemTimeInterruptMonitor
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);
            
            // Начать мониторинг с ограничением времени в 5 секунд
            monitor.StartMonitor(5000);

            // Отобразить начальное значение IsInterruptionRequested
            Console.WriteLine("Initial IsInterruptionRequested: " + monitor.IsInterruptionRequested);

            // Смоделировать длительную операцию
            Console.WriteLine("Starting long operation...");
            for (int i = 0; i < 100000; i++)
            {
                worksheet.Cells[i, 0].Value = i;
                
                // Проверить, было ли запрошено прерывание
                if (monitor.IsInterruptionRequested)
                {
                    Console.WriteLine("Operation interrupted after time limit!");
                    break;
                }
            }

            // Отобразить конечное значение IsInterruptionRequested
            Console.WriteLine("Final IsInterruptionRequested: " + monitor.IsInterruptionRequested);

            // Сохранить результат
            workbook.Save("PropertyIsInterruptionRequestedDemo.xlsx");
        }
    }
}
```

### См. также

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


