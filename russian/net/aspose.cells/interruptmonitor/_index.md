---
title: "Класс InterruptMonitor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.InterruptMonitor. Представляет все операторы, связанные с прерыванием"
type: docs
url: /ru/net/aspose.cells/interruptmonitor/
---
## InterruptMonitor class

Представляет все операторы, связанные с прерыванием.

```csharp
public class InterruptMonitor : AbstractInterruptMonitor
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [InterruptMonitor](interruptmonitor/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/interruptmonitor/isinterruptionrequested/) { get; } | Отметьте монитор как запрашивающий прерывание |
| virtual [TerminateWithoutException](../../aspose.cells/abstractinterruptmonitor/terminatewithoutexception/) { get; } | Когда процедура прерывается, следует ли тихо завершать её или бросать исключение. По умолчанию false, то есть когда [`IsInterruptionRequested`](../abstractinterruptmonitor/isinterruptionrequested/) истинно, будет выброшено [`CellsException`](../cellsexception/) с кодом Interrupted. (Наследуется от [`AbstractInterruptMonitor`](../abstractinterruptmonitor/).) |

## Методы

| Имя | Описание |
| --- | --- |
| [Interrupt](../../aspose.cells/interruptmonitor/interrupt/)() | Прервать текущий оператор. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassInterruptMonitorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте некоторые образцы данных.
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Создайте и назначьте монитор прерываний
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;
            
            try
            {
                Console.WriteLine("Starting save operation...");
                
                // Смоделируйте прерывание операции
                monitor.Interrupt();
                
                // Попробуйте сохранить (должно быть прервано)
                workbook.Save("output.pdf", SaveFormat.Pdf);
                Console.WriteLine("Save completed successfully.");
            }
            catch (CellsException e)
            {
                if (e.Code == ExceptionType.Interrupted)
                {
                    Console.WriteLine("Operation was successfully interrupted.");
                }
                else
                {
                    Console.WriteLine("Error occurred: " + e.Message);
                }
            }
        }
    }
}
```

### См. также

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


