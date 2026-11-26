---
title: "Picture.OriginalHeight"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Picture. Возвращает исходную высоту изображения"
type: docs
url: /ru/net/aspose.cells.drawing/picture/originalheight/
---
## Picture.OriginalHeight property

Получает исходную высоту картинки.

```csharp
public int OriginalHeight { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalHeightDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить изображение на лист
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Picture pic = worksheet.Pictures[imgIndex];

            // Получить и отобразить исходную высоту изображения
            int originalHeight = pic.OriginalHeight;
            Console.WriteLine("Original height of the picture: " + originalHeight + " pixels");

            // Сохраните книгу
            workbook.Save("result.xlsx");
        }
    }
}
```

### См. также

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


