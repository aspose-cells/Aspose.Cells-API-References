---
title: "Picture.SourceFullName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Picture. Получает или задает путь и имя исходного файла для связанного изображения"
type: docs
url: /ru/net/aspose.cells.drawing/picture/sourcefullname/
---
## Picture.SourceFullName property

Получает или задает путь и имя исходного файла для связанного изображения.

```csharp
public string SourceFullName { get; set; }
```

### Примечания

Значение по умолчанию — пустая строка. Если SourceFullName не является пустой строкой, изображение связывается. Если SourceFullName не является пустой строкой, но Data равно null, тогда изображение связывается и не сохраняется в файле.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertySourceFullNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить связанное изображение в лист
            string imagePath = "example.png";
            Picture picture = worksheet.Shapes.AddLinkedPicture(0, 0, 100, 100, imagePath);

            // Продемонстрировать свойство SourceFullName
            Console.WriteLine("Picture SourceFullName: " + picture.SourceFullName);
            Console.WriteLine("Is linked picture: " + picture.IsLink);

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


