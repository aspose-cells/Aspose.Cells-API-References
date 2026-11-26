---
title: "Класс PicFormatOption"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.PicFormatOption. Представляет параметры формата изображения."
type: docs
url: /ru/net/aspose.cells.drawing/picformatoption/
---
## PicFormatOption class

Представляет параметр формата изображения.

```csharp
public class PicFormatOption
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PicFormatOption](picformatoption/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Bottom](../../aspose.cells.drawing/picformatoption/bottom/) { get; set; } | Получает или задаёт смещение снизу для растягивания изображения. |
| [Left](../../aspose.cells.drawing/picformatoption/left/) { get; set; } | Получает или задаёт смещение слева для растягивания изображения. |
| [Right](../../aspose.cells.drawing/picformatoption/right/) { get; set; } | Получает или задаёт смещение справа для растягивания изображения. |
| [Scale](../../aspose.cells.drawing/picformatoption/scale/) { get; set; } | Получает или задаёт количество, с которым изображение складывается и масштабируется. |
| [Top](../../aspose.cells.drawing/picformatoption/top/) { get; set; } | Получает или задаёт смещение сверху для растягивания изображения. |
| [Type](../../aspose.cells.drawing/picformatoption/type/) { get; set; } | Получает или задаёт тип заливки изображения. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.IO;

    public class DrawingClassPicFormatOptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте форму и задайте заливку изображением
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 200, 200);
            // Свойство FillType удалено из доступа MsoFillFormat
            shape.FillFormat.ImageData = File.ReadAllBytes("aspose-logo.png");

            // Настройте параметры формата изображения
            PicFormatOption picFormat = new PicFormatOption
            {
                Type = FillPictureType.Stretch,
                Left = 0.15,
                Right = 0.15,
                Top = 0.15,
                Bottom = 0.15,
                Scale = 0.8
            };

            // Добавьте вторую форму с мозаичным изображением
            Shape tiledShape = worksheet.Shapes.AddRectangle(5, 210, 0, 0, 200, 200);
            // Свойство FillType удалено из доступа MsoFillFormat
            tiledShape.FillFormat.ImageData = File.ReadAllBytes("aspose-logo.png");
            
            PicFormatOption tileFormat = new PicFormatOption
            {
                Type = FillPictureType.Stack,
                Scale = 1.5
            };

            workbook.Save("PicFormatOptionDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


