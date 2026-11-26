---
title: "ShapeTextAlignment.NumberOfColumns"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShapeTextAlignment. Получает и задает количество колонок текста в ограничивающем прямоугольнике"
type: docs
url: /ru/net/aspose.cells.drawing.texts/shapetextalignment/numberofcolumns/
---
## ShapeTextAlignment.NumberOfColumns property

Получает и задает количество столбцов текста в ограничивающем прямоугольнике.

```csharp
public int NumberOfColumns { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyNumberOfColumnsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму на лист
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);
            
            // Установите текст для формы
            shape.Text = "This is sample text\nin multiple columns";
            
            // Получите выравнивание текста и установите количество колонок
            shape.TextBody.TextAlignment.NumberOfColumns = 2;
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            // Проверить свойство
            Console.WriteLine("Number of columns: " + 
                worksheet.Shapes[0].TextBody.TextAlignment.NumberOfColumns);
        }
    }
}
```

### См. также

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


