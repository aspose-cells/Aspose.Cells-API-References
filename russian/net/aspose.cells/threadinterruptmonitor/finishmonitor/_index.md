---
title: "ThreadInterruptMonitor.FinishMonitor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ThreadInterruptMonitor. Завершает монитор для одной процедуры"
type: docs
url: /ru/net/aspose.cells/threadinterruptmonitor/finishmonitor/
---
## ThreadInterruptMonitor.FinishMonitor method

Завершает монитор для одной процедуры.

```csharp
public void FinishMonitor()
```

### Примечания

Вызов этого метода после мониторируемой процедуры может освободить поток монитора раньше, особенно когда для неё нет прерывания (время выполнения этой процедуры меньше указанного предела).

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadInterruptMonitorMethodFinishMonitorDemo
    {
        public static void Run()
        {
            // Создайте экземпляр ThreadInterruptMonitor
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);

            // Создайте LoadOptions и установите InterruptMonitor
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // Начните мониторинг с тайм-аутом 1 секунды
            monitor.StartMonitor(1000);

            try
            {
                // Смоделируйте длительную операцию
                for (int i = 0; i < 5; i++)
                {
                    System.Threading.Thread.Sleep(200);
                    Console.WriteLine($"Processing step {i + 1}");
                }

                // Завершите мониторинг операции
                monitor.FinishMonitor();
                Console.WriteLine("Operation completed successfully");
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

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


