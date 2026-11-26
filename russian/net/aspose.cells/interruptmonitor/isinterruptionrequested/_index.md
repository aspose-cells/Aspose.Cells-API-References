---
title: "InterruptMonitor.IsInterruptionRequested"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство InterruptMonitor. Помечает монитор как запрашивающий прерывание"
type: docs
url: /ru/net/aspose.cells/interruptmonitor/isinterruptionrequested/
---
## InterruptMonitor.IsInterruptionRequested property

Отметьте монитор как запрашивающий прерывание

```csharp
public override bool IsInterruptionRequested { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class InterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите доступ к её первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте монитор прерываний и назначьте его книге
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;

            // Отобразите начальное состояние IsInterruptionRequested
            Console.WriteLine("Initial IsInterruptionRequested value: " + monitor.IsInterruptionRequested);

            // Смоделируйте длительную операцию обработки данных
            Console.WriteLine("Starting data processing...");
            for (int rowIdx = 0; rowIdx < 10000; rowIdx++)
            {
                // Запросите прерывание после обработки 500 строк
                if (rowIdx == 500)
                {
                    monitor.Interrupt();
                    Console.WriteLine("Interrupt requested. IsInterruptionRequested: " + monitor.IsInterruptionRequested);
                }

                // Проверьте наличие запроса на прерывание
                if (monitor.IsInterruptionRequested)
                {
                    Console.WriteLine($"Processing interrupted at row {rowIdx}");
                    break;
                }

                // Смоделируйте обработку данных
                worksheet.Cells[rowIdx, 0].Value = $"Row {rowIdx} data";
            }

            // Сохранить изменённую книгу
            workbook.Save("InterruptionDemoOutput.xlsx");
            Console.WriteLine("File saved with partial data due to interruption.");
        }
    }
}
```

### См. также

* class [InterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


