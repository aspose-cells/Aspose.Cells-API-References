---
title: "FillFormat.PictureFormatType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FillFormat. Получает и задает тип формата изображения"
type: docs
url: /ru/net/aspose.cells.drawing/fillformat/pictureformattype/
---
## FillFormat.PictureFormatType property

Получает и задает тип формата изображения.

```csharp
public FillPictureType PictureFormatType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyPictureFormatTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте форму, чтобы продемонстрировать заливку изображения
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            // Установить свойства заливки изображением
            shape.Fill.Type = FillType.Texture;
            shape.Fill.Texture = TextureType.BlueTissuePaper;
            shape.Fill.PictureFormatType = FillPictureType.Stretch;

            // Сохраните книгу
            workbook.Save("FillFormatPictureTypeDemo.xlsx");

            // Загрузите сохранённую книгу, чтобы проверить свойства
            Workbook verifyWorkbook = new Workbook("FillFormatPictureTypeDemo.xlsx");
            Shape verifyShape = verifyWorkbook.Worksheets[0].Shapes[0];

            // Выведите PictureFormatType, чтобы продемонстрировать его использование
            Console.WriteLine("PictureFormatType: " + verifyShape.Fill.PictureFormatType);
        }
    }
}
```

### См. также

* enum [FillPictureType](../../fillpicturetype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


