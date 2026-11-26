---
title: "ScrollBar.IncrementalChange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ScrollBar. Получает или задает величину, на которую полоса прокрутки или спиннер увеличивается при прокрутке на одну строку"
type: docs
url: /ru/net/aspose.cells.drawing/scrollbar/incrementalchange/
---
## ScrollBar.IncrementalChange property

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
    public class ScrollBarPropertyIncrementalChangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте полосу прокрутки в лист
            ScrollBar scrollBar = worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Задайте свойства полосы прокрутки
            scrollBar.Min = 0;
            scrollBar.Max = 100;
            scrollBar.CurrentValue = 50;
            scrollBar.IncrementalChange = 5; // This is the key property we're demonstrating
            scrollBar.PageChange = 20;

            // Отобразите свойства полосы прокрутки
            Console.WriteLine("Scroll Bar Properties:");
            Console.WriteLine("Min: " + scrollBar.Min);
            Console.WriteLine("Max: " + scrollBar.Max);
            Console.WriteLine("Current Value: " + scrollBar.CurrentValue);
            Console.WriteLine("Incremental Change: " + scrollBar.IncrementalChange);
            Console.WriteLine("Page Change: " + scrollBar.PageChange);

            // Измените приращение
            scrollBar.IncrementalChange = 10;
            Console.WriteLine("\nModified Incremental Change: " + scrollBar.IncrementalChange);

            // Сохраните книгу
            workbook.Save("ScrollBarDemo.xlsx");
        }
    }
}
```

### См. также

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


