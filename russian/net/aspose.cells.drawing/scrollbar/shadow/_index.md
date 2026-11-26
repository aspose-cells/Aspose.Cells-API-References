---
title: "ScrollBar.Shadow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ScrollBar. Указывает, имеет ли фигура 3D‑теневание"
type: docs
url: /ru/net/aspose.cells.drawing/scrollbar/shadow/
---
## ScrollBar.Shadow property

Указывает, имеет ли фигура 3‑D затенение.

```csharp
public bool Shadow { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyShadowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить горизонтальную полосу прокрутки
            ScrollBar scrollBar = worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);
            
            // Задайте свойства полосы прокрутки
            scrollBar.Min = 0;
            scrollBar.Max = 100;
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 20;
            scrollBar.CurrentValue = 50;
            scrollBar.IsHorizontal = true;
            
            // Продемонстрировать свойство Shadow
            scrollBar.Shadow = true; // Enable 3D shadow effect
            
            // Создайте еще одну полосу прокрутки для сравнения
            ScrollBar scrollBar2 = worksheet.Shapes.AddScrollBar(1, 2, 1, 1, 100, 20);
            scrollBar2.Shadow = false; // No shadow
            
            // Сохраните книгу
            workbook.Save("ScrollBarShadowDemo.xlsx");
            
            Console.WriteLine("ScrollBar Shadow demo completed. Check output file.");
        }
    }
}
```

### См. также

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


