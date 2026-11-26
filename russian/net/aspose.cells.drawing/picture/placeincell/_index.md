---
title: "Picture.PlaceInCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Picture метод. Поместите эту картинку в ячейку"
type: docs
url: /ru/net/aspose.cells.drawing/picture/placeincell/
---
## Picture.PlaceInCell method

Поместите эту картинку в ячейку

```csharp
[Obsolete("Use Picture.IsPlacedInCell property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void PlaceInCell()
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого, пожалуйста, используйте свойство Picture.IsPlacedInCell. Это свойство будет удалено через 12 месяцев, начиная с января 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureMethodPlaceInCellDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить изображение на лист
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Поместите картинку в ячейку A1
            picture.PlaceInCell();

            // Проверьте, что картинка помещена в ячейку
            Cell cell = worksheet.Cells["A1"];
            byte[] imageData = cell.EmbeddedImage;
            Console.WriteLine("Image placed in cell A1. Image data length: " + imageData.Length);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


