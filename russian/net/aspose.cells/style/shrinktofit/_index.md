---
title: "Style.ShrinkToFit"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Определяет, сжимается ли текст автоматически, чтобы поместиться в доступную ширину столбца"
type: docs
url: /ru/net/aspose.cells/style/shrinktofit/
---
## Style.ShrinkToFit property

Представляет, автоматически ли текст уменьшается, чтобы поместиться в доступную ширину столбца.

```csharp
public bool ShrinkToFit { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyShrinkToFitDemo
    {
        public static void Run()
        {
            // Создать объект рабочей книги
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Доступ к коллекции cells
            Cells cells = worksheet.Cells;
            
            // Установить в ячейку A1 текст, который длиннее ширины столбца
            cells["A1"].PutValue("This is a long text that needs shrinking to fit");
            
            // Установить ширину столбца меньше длины текста
            cells.SetColumnWidth(0, 10);
            
            // Получить стиль ячейки A1
            Style style = cells["A1"].GetStyle();
            
            // Установить ShrinkToFit в true
            style.ShrinkToFit = true;
            
            // Применить стиль к ячейке A1
            cells["A1"].SetStyle(style);
            
            // Сохраните книгу
            workbook.Save("ShrinkToFitDemo.xlsx");
            
            Console.WriteLine("ShrinkToFit demo completed successfully.");
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


