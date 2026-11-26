---
title: "Worksheet.Pictures"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Возвращает коллекцию Picture"
type: docs
url: /ru/net/aspose.cells/worksheet/pictures/
---
## Worksheet.Pictures property

Возвращает коллекцию [`Picture`](../../../aspose.cells.drawing/picture/).

```csharp
public PictureCollection Pictures { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyPicturesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить изображение на лист
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Установить свойства изображения
            picture.Placement = PlacementType.FreeFloating;
            picture.BorderLineColor = System.Drawing.Color.Blue;
            picture.BorderWeight = 1;

            // Сохраните книгу
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // Загрузите сохранённую книгу для проверки
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Number of pictures: " + loadedWorkbook.Worksheets[0].Pictures.Count);
        }
    }
}
```

### См. также

* class [PictureCollection](../../../aspose.cells.drawing/picturecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


