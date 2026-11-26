---
title: "Cells.MultiThreadReading"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Получает или задает, должна ли модель данных ячеек поддерживать многопоточное чтение. Значение по умолчанию этого свойства — false"
type: docs
url: /ru/net/aspose.cells/cells/multithreadreading/
---
## Cells.MultiThreadReading property

Получает или задает, должна ли модель данных ячеек поддерживать многопоточное чтение. Значение по умолчанию этого свойства — false.

```csharp
public bool MultiThreadReading { get; set; }
```

### Примечания

Если несколько потоков одновременно читают объекты Row/Cell в этой коллекции, это свойство следует установить в true, иначе могут возникнуть неожиданные результаты. Поддержка многопоточного чтения может ухудшить производительность доступа к объектам Row/Cell из этой коллекции. Обратите внимание, что некоторые функции не поддерживают многопоточное чтение, например форматирование значений (по [`StringValue`](../../cell/stringvalue/), [`DisplayStringValue`](../../cell/displaystringvalue/), и т.д.). Поэтому даже при установке этого свойства в true указанные API могут давать неожиданные результаты при многопоточном чтении.

### Примеры

```csharp
using System;
using System.Threading;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMultiThreadReadingDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Включить многопоточное чтение
            cells.MultiThreadReading = true;

            // Настроить стиль для первого столбца
            Style style = wb.CreateStyle();
            style.Custom = "yyyy-mm-dd";
            StyleFlag sf = new StyleFlag();
            sf.All = true;
            cells.Columns[0].ApplyStyle(style, sf);

            // Заполните ячейки примерными данными
            int rowCount = 1000;
            for (int i = 0; i < rowCount; i++)
            {
                cells[i, 0].PutValue(DateTime.Now.AddDays(i).ToOADate());
            }

            // Создать потоки для чтения значений ячеек
            int threadCount = 5;
            int cellsPerThread = rowCount / threadCount;
            int[] finishedCount = new int[1];
            System.Text.StringBuilder errors = new System.Text.StringBuilder();

            for (int i = 0; i < threadCount; i++)
            {
                int start = i * cellsPerThread;
                int end = (i == threadCount - 1) ? rowCount : start + cellsPerThread;
                
                Thread t = new Thread(() => 
                {
                    try
                    {
                        for (int row = start; row < end; row++)
                        {
                            object value = cells[row, 0].Value;
                            Console.WriteLine($"Thread {Thread.CurrentThread.ManagedThreadId}: Cell[{row},0] = {value}");
                        }
                        Interlocked.Increment(ref finishedCount[0]);
                    }
                    catch (Exception ex)
                    {
                        lock (errors)
                        {
                            errors.AppendLine($"Thread {Thread.CurrentThread.ManagedThreadId} error: {ex.Message}");
                        }
                    }
                });
                t.Start();
            }

            // Ожидать завершения всех потоков
            while (finishedCount[0] < threadCount)
            {
                Thread.Sleep(200);
            }

            if (errors.Length > 0)
            {
                Console.WriteLine("Errors occurred:");
                Console.WriteLine(errors.ToString());
            }
            else
            {
                Console.WriteLine("All threads completed successfully");
            }
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


