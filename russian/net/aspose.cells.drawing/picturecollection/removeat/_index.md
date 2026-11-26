---
title: "PictureCollection.RemoveAt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PictureCollection. Удаляет формы по указанному индексу"
type: docs
url: /ru/net/aspose.cells.drawing/picturecollection/removeat/
---
## PictureCollection.RemoveAt method

Удалить фигуры по конкретному индексу

```csharp
public void RemoveAt(int index)
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить несколько изображений в лист
            int index1 = worksheet.Pictures.Add(1, 1, "image1.png");
            int index2 = worksheet.Pictures.Add(5, 1, "image2.png");
            int index3 = worksheet.Pictures.Add(10, 1, "image3.png");

            Console.WriteLine("Number of pictures before removal: " + worksheet.Pictures.Count);

            // Удалить изображение по указанному индексу
            worksheet.Pictures.RemoveAt(index2);

            Console.WriteLine("Number of pictures after removal: " + worksheet.Pictures.Count);
        }
    }
}
```

### См. также

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


