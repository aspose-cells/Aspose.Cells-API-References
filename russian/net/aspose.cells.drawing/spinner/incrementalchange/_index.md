---
title: "Spinner.IncrementalChange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Spinner. Получает или задает величину, на которую увеличивается полоса прокрутки или Spinner при прокрутке на одну строку"
type: docs
url: /ru/net/aspose.cells.drawing/spinner/incrementalchange/
---
## Spinner.IncrementalChange property

Получает или задает величину, на которую полоса прокрутки или спиннер увеличивается при прокрутке на одну строку.

```csharp
public int IncrementalChange { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyIncrementalChangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать элемент управления спиннером
            Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 100);

            // Установите свойства Spinner
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.CurrentValue = 50;
            spinner.IncrementalChange = 5; // Demonstrate IncrementalChange property

            // Проверить и вывести значение IncrementalChange
            Console.WriteLine("Spinner IncrementalChange: " + spinner.IncrementalChange);

            // Изменить и снова проверить
            spinner.IncrementalChange = 10;
            Console.WriteLine("Modified IncrementalChange: " + spinner.IncrementalChange);

            // Сохраните книгу
            workbook.Save("SpinnerIncrementalChangeDemo.xlsx");
        }
    }
}
```

### См. также

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


