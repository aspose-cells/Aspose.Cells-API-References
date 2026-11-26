---
title: "Spinner.Min"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Spinner. Получает или задает минимальное значение диапазона полосы прокрутки или Spinner"
type: docs
url: /ru/net/aspose.cells.drawing/spinner/min/
---
## Spinner.Min property

Получает или задает минимальное значение диапазона полосы прокрутки или спиннера

```csharp
public int Min { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyMinDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить элемент управления Spinner с правильными размерами
            Spinner spinner = worksheet.Shapes.AddSpinner(1, 1, 1, 1, 100, 20);

            // Установить свойства Spinner, включая Min
            spinner.Min = 10;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;
            spinner.CurrentValue = 15;

            // Проверить и вывести свойство Min
            Console.WriteLine("Spinner Min Value: " + spinner.Min);

            // Сохраните книгу
            workbook.Save("SpinnerPropertyMinDemo.xlsx");
        }
    }
}
```

### См. также

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


