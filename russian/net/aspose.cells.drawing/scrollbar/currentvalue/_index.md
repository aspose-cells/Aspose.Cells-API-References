---
title: "ScrollBar.CurrentValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ScrollBar. Получает или задает текущее значение"
type: docs
url: /ru/net/aspose.cells.drawing/scrollbar/currentvalue/
---
## ScrollBar.CurrentValue property

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
    public class ScrollBarPropertyCurrentValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте полосу прокрутки в лист
            Aspose.Cells.Drawing.ScrollBar scrollBar = (Aspose.Cells.Drawing.ScrollBar)worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Задайте свойства полосы прокрутки, используя правильные имена свойств
            scrollBar.Min = 0;
            scrollBar.Max = 100;
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 20;

            // Задайте и продемонстрируйте свойство CurrentValue
            scrollBar.CurrentValue = 50;
            Console.WriteLine("ScrollBar CurrentValue: " + scrollBar.CurrentValue);

            // Измените текущее значение
            scrollBar.CurrentValue = 75;
            Console.WriteLine("Updated ScrollBar CurrentValue: " + scrollBar.CurrentValue);

            // Сохраните книгу
            workbook.Save("ScrollBarCurrentValueDemo.xlsx");
        }
    }
}
```

### См. также

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


