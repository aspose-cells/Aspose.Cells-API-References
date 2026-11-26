---
title: "ScrollBar.IsHorizontal"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ScrollBar. Указывает, является ли это горизонтальной полосой прокрутки"
type: docs
url: /ru/net/aspose.cells.drawing/scrollbar/ishorizontal/
---
## ScrollBar.IsHorizontal property

Указывает, является ли это горизонтальной полосой прокрутки.

```csharp
public bool IsHorizontal { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyIsHorizontalDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить горизонтальную полосу прокрутки
            Shape scrollBarShape = worksheet.Shapes.AddScrollBar(1, 0, 1, 0, 100, 20);
            ScrollBar scrollBar = (ScrollBar)scrollBarShape;
            scrollBar.IsHorizontal = true;

            // Добавьте вертикальную полосу прокрутки для сравнения
            Shape verticalScrollBarShape = worksheet.Shapes.AddScrollBar(1, 0, 1, 30, 20, 100);
            ScrollBar verticalScrollBar = (ScrollBar)verticalScrollBarShape;
            verticalScrollBar.IsHorizontal = false;

            // Продемонстрируйте свойство IsHorizontal
            Console.WriteLine("Horizontal Scroll Bar IsHorizontal: " + scrollBar.IsHorizontal);
            Console.WriteLine("Vertical Scroll Bar IsHorizontal: " + verticalScrollBar.IsHorizontal);

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


