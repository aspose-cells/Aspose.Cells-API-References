---
title: "Picture.IsLink"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Picture. Возвращает true, если изображение связано с файлом"
type: docs
url: /ru/net/aspose.cells.drawing/picture/islink/
---
## Picture.IsLink property

Возвращает true, если картинка связана с файлом.

```csharp
public bool IsLink { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyIsLinkDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить связанное изображение
            int linkedPictureIndex = worksheet.Pictures.Add(0, 0, "https://example.com/image.jpg");
            Picture linkedPicture = worksheet.Pictures[linkedPictureIndex];

            // Добавить встроенное изображение (используя пример данных)
            byte[] embeddedImageData = new byte[] { 0x01, 0x02, 0x03 }; // Sample image data
            using (MemoryStream stream = new MemoryStream(embeddedImageData))
            {
                int embeddedPictureIndex = worksheet.Pictures.Add(0, 5, stream);
                Picture embeddedPicture = worksheet.Pictures[embeddedPictureIndex];

                // Продемонстрировать свойство IsLink
                Console.WriteLine("Linked picture IsLink: " + linkedPicture.IsLink);
                Console.WriteLine("Embedded picture IsLink: " + embeddedPicture.IsLink);

                // Показать различное поведение в зависимости от IsLink
                Console.WriteLine("\nLinked picture data is null: " + (linkedPicture.Data == null));
                Console.WriteLine("Embedded picture data length: " + embeddedPicture.Data.Length);
            }
        }
    }
}
```

### См. также

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


