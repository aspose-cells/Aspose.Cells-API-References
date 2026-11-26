---
title: "Класс AbstractInterruptMonitor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.AbstractInterruptMonitor. Монитор запросов прерывания во всех длительных операциях"
type: docs
url: /ru/net/aspose.cells/abstractinterruptmonitor/
---
## AbstractInterruptMonitor class

Мониторинг запросов на прерывание во всех длительных операциях.

```csharp
public abstract class AbstractInterruptMonitor
```

## Свойства

| Имя | Описание |
| --- | --- |
| abstract [IsInterruptionRequested](../../aspose.cells/abstractinterruptmonitor/isinterruptionrequested/) { get; } | Указывает, запрошено ли прерывание текущей операции. Если true, то текущая операция будет прервана. Реализация должна выполнять здесь быструю и эффективную проверку, иначе это может стать узким местом процедуры. |
| virtual [TerminateWithoutException](../../aspose.cells/abstractinterruptmonitor/terminatewithoutexception/) { get; } | Когда процедура прерывается, следует ли завершать процедуру тихо или бросать исключение. По умолчанию false, то есть когда [`IsInterruptionRequested`](./isinterruptionrequested/) истинно, будет выброшено [`CellsException`](../cellsexception/) с кодом Interrupted. |

### Примеры

```csharp
using Aspose.Cells;
using System;
using System.Reflection.Metadata.Ecma335;

namespace AsposeCellsExamples
{
    // Пользовательская реализация AbstractInterruptMonitor
    public class CustomInterruptMonitor : AbstractInterruptMonitor
    {
        //результирующий файл корректен
        public override bool IsInterruptionRequested
        {
            get
            {
                Console.WriteLine("Get the return value of whether to interrupt the program===");
                // Логика определения, запрошено ли прерывание
                return false; // Change this based on your logic
            }
        }

        public override bool TerminateWithoutException
        {
            get => false; // Change this based on your logic
        }

        //// результатный файл падает
        //public override bool IsInterruptionRequested
        //{
        //    get
        //    {
        //        Console.WriteLine(\"Get the return value of whether to interrupt the program===\");
        //        // Логика определения, запрошено ли прерывание
        //        //return false; // Измените это в соответствии с вашей логикой
        //        return true;
        //    }
        //}

        //public override bool TerminateWithoutException
        //{
        //    get => true; // Измените это в соответствии с вашей логикой
        //}
    }

    public class InterruptMonitorDemo
    {
        public static void RunDemo()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].Formula = "=A1+A2";

            // Создайте экземпляр CustomInterruptMonitor
            CustomInterruptMonitor monitor = new CustomInterruptMonitor();

            // Установите параметры загрузки с пользовательским монитором прерываний
            LoadOptions loadOptions = new LoadOptions
            {
                InterruptMonitor = monitor
            };

            // Загрузите рабочую книгу с указанными параметрами
            workbook = new Workbook("Sample.xlsx", loadOptions);

            // Выполните вычисления
            workbook.CalculateFormula();

            // Сохраните книгу
            workbook.Save("InterruptMonitorDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


