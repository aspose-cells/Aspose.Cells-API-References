---
title: "Перечисление MirrorType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.MirrorType. Представляет тип зеркального отражения заливки текстурой"
type: docs
url: /ru/net/aspose.cells.drawing/mirrortype/
---
## MirrorType enumeration

Представляет тип зеркального отражения текстурной заливки.

```csharp
public enum MirrorType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Нет |
| Horizonal | `1` | Горизонтальный |
| Vertical | `2` | Вертикальный |
| Both | `3` | Оба |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassMirrorTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму для демонстрации MirrorType
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 200);

            // Установить заливку текстурой с различными типами зеркального отражения
            shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.Horizonal;
            shape = worksheet.Shapes.AddRectangle(2, 0, 1, 100, 100, 200);
            shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.Vertical;
            shape = worksheet.Shapes.AddRectangle(3, 0, 1, 100, 100, 200);
            shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.Both;
            shape = worksheet.Shapes.AddRectangle(4, 0, 1, 100, 100, 200);
            shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.None;

            // Сохранить результат
            workbook.Save("MirrorTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


