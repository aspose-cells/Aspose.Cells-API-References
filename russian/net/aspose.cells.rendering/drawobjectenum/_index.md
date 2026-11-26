---
title: "Перечисление DrawObjectEnum"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Rendering.DrawObjectEnum. Указывает, является ли DrawObject ячейкой или изображением"
type: docs
url: /ru/net/aspose.cells.rendering/drawobjectenum/
---
## DrawObjectEnum enumeration

Указывает ячейку или изображение DrawObject.

```csharp
public enum DrawObjectEnum
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Image | `0` | Указывает, что DrawObject является изображением |
| Cell | `1` | указывает, что DrawObject является ячейкой |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassDrawObjectEnumDemo
    {
        public static void Run()
        {
            // Создайте рабочую книгу и добавьте примерные данные
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Cell");

            // Создайте объект PdfSaveOptions
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Создайте пользовательский DrawObjectEventHandler
            saveOptions.DrawObjectEventHandler = new CustomDrawObjectEventHandler();

            // Сохраните рабочую книгу в PDF с помощью пользовательского обработчика
            workbook.Save("output.pdf", saveOptions);
        }
    }

    public class CustomDrawObjectEventHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            // Проверьте, является ли объект рисования ячейкой
            if (drawObject.Type == DrawObjectEnum.Cell)
            {
                Cell cell = drawObject.Cell;
                
                // Выведите информацию о ячейке
                Console.WriteLine($"Drawing Cell - Row: {cell.Row}, Column: {cell.Column}");
                Console.WriteLine($"Position: ({x}, {y}), Size: {width}x{height}");
                
                // Особая обработка ячейки A1
                if (cell.Row == 0 && cell.Column == 0)
                {
                    Console.WriteLine("This is cell A1");
                }
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


