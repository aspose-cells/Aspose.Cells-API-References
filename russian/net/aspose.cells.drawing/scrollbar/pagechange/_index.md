---
title: "ScrollBar.PageChange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ScrollBar. Получает или задает изменение страницы"
type: docs
url: /ru/net/aspose.cells.drawing/scrollbar/pagechange/
---
## ScrollBar.PageChange property

Получает или задает изменение страницы

```csharp
public int PageChange { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyPageChangeDemo
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
            scrollBar.IncrementalChange = 1;
            scrollBar.PageChange = 10; // Demonstrate PageChange property
            scrollBar.LinkedCell = "A1";

            // Сохраните книгу
            workbook.Save("ScrollBarPropertyPageChangeDemo.xlsx");

            // Загрузите сохранённую книгу, чтобы проверить свойства
            Workbook verifyWorkbook = new Workbook("ScrollBarPropertyPageChangeDemo.xlsx");
            ScrollBar verifyScrollBar = (ScrollBar)verifyWorkbook.Worksheets[0].Shapes[0];

            // Выведите значение свойства PageChange, чтобы продемонстрировать, что оно было сохранено/загружено корректно
            Console.WriteLine("ScrollBar PageChange value: " + verifyScrollBar.PageChange);
        }
    }
}
```

### См. также

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


