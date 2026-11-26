---
title: "ScrollBar.Min"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ScrollBar. Получает или задает минимальное значение диапазона полосы прокрутки или спиннера"
type: docs
url: /ru/net/aspose.cells.drawing/scrollbar/min/
---
## ScrollBar.Min property

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
    public class ScrollBarPropertyMinDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте полосу прокрутки в лист
            Aspose.Cells.Drawing.ScrollBar scrollBar = (Aspose.Cells.Drawing.ScrollBar)worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Задайте свойства полосы прокрутки
            scrollBar.Min = 10;
            scrollBar.Max = 100;
            scrollBar.CurrentValue = 50;  // Changed from Value to CurrentValue
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 20;

            // Отобразите значение свойства Min
            Console.WriteLine("ScrollBar Min Value: " + scrollBar.Min);

            // Сохраните книгу
            workbook.Save("ScrollBarMinDemo.xlsx");
        }
    }
}
```

### См. также

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


