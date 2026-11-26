---
title: "Picture.OriginalWidth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Picture. Получает исходную ширину изображения"
type: docs
url: /ru/net/aspose.cells.drawing/picture/originalwidth/
---
## Picture.OriginalWidth property

Получает исходную ширину картинки.

```csharp
public int OriginalWidth { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalWidthDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить изображение на лист
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Aspose.Cells.Drawing.Picture pic = worksheet.Pictures[imgIndex];

            // Получить и отобразить исходную ширину изображения
            int originalWidth = pic.OriginalWidth;
            Console.WriteLine("Original width of the picture: " + originalWidth + " pixels");

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


