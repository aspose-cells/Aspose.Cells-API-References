---
title: "AbstractInterruptMonitor.IsInterruptionRequested"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AbstractInterruptMonitor. Указывает, запрошено ли прерывание текущей операции. Если true, то текущая операция будет прервана. Реализация должна выполнять здесь быструю и эффективную проверку, иначе это может стать ещё одним узким местом процедуры."
type: docs
url: /ru/net/aspose.cells/abstractinterruptmonitor/isinterruptionrequested/
---
## AbstractInterruptMonitor.IsInterruptionRequested property

Указывает, запрошено ли прерывание текущей операции. Если true, то текущая операция будет прервана. Реализация должна выполнять здесь быструю и эффективную проверку, иначе это может стать узким местом процедуры.

```csharp
public abstract bool IsInterruptionRequested { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Threading;
    using System.Threading.Tasks;

    public class AbstractInterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать монитор прерываний и назначить его рабочей книге
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;

            // Отобразить начальное значение
            Console.WriteLine("Initial IsInterruptionRequested: " + monitor.IsInterruptionRequested);

            // Запустить задачу прерывания
            Task.Run(() =>
            {
                Thread.Sleep(1000); // Wait 1 seconds
                Console.WriteLine("\nTriggering interruption...");
                monitor.Interrupt();
            });

            // Моделирование длительной операции
            Console.WriteLine("Starting data generation...");
            try
            {
                for (int i = 0; i < 500000000; i++)
                {
                    if (monitor.IsInterruptionRequested)
                    {
                        Console.WriteLine($"\nInterrupted at row {i}");
                        break;
                    }

                    worksheet.Cells[i, 0].Value = $"Data {i}";
                    
                    // Смоделировать время обработки
                    if (i % 1000 == 0) 
                        Console.Write(".");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine("\nError: " + ex.Message);
            }

            // Сохранить результат
            workbook.Save("InterruptionDemoOutput.xlsx");

            Console.WriteLine("\nWorkbook saved with partial data.");
        }
    }
}
```

### См. также

* class [AbstractInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


