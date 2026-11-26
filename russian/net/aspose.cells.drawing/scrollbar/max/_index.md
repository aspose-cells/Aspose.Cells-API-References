---
title: "ScrollBar.Max"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ScrollBar. Получает или задает максимальное значение диапазона полосы прокрутки или спиннера"
type: docs
url: /ru/net/aspose.cells.drawing/scrollbar/max/
---
## ScrollBar.Max property

Получает или задает максимальное значение диапазона полосы прокрутки или спиннера.

```csharp
public int Max { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyMaxDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте полосу прокрутки в лист
            Aspose.Cells.Drawing.ScrollBar scrollBar = (Aspose.Cells.Drawing.ScrollBar)worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Задайте свойства полосы прокрутки
            scrollBar.Min = 0;
            scrollBar.Max = 100; // Demonstrating Max property usage
            scrollBar.CurrentValue = 50;
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 10;

            // Сохраните книгу
            workbook.Save("ScrollBarMaxDemo.xlsx");

            // Отобразите информацию
            Console.WriteLine("ScrollBar created with Max value: " + scrollBar.Max.ToString());
            Console.WriteLine("File saved successfully.");
        }
    }
}
```

### См. также

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


