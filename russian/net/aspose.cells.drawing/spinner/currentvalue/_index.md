---
title: "Spinner.CurrentValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Spinner. Получает или задает текущее значение"
type: docs
url: /ru/net/aspose.cells.drawing/spinner/currentvalue/
---
## Spinner.CurrentValue property

Получает или задает текущее значение.

```csharp
public int CurrentValue { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyCurrentValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить элемент управления Spinner
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Spinner, 1, 1, 0, 0, 20, 20);
            Spinner spinner = (Spinner)shape;

            // Установите свойства Spinner
            spinner.LinkedCell = "A1";
            spinner.Min = 1;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;
            spinner.CurrentValue = 10; // Using CurrentValue property directly

            // Проверить и вывести текущее значение
            Console.WriteLine("Spinner CurrentValue: " + spinner.CurrentValue);

            // Сохраните книгу
            workbook.Save("SpinnerDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


