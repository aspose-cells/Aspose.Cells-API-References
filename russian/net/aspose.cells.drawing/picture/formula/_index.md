---
title: "Picture.Formula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Picture свойство. Получает и задает данные формулы"
type: docs
url: /ru/net/aspose.cells.drawing/picture/formula/
---
## Picture.Formula property

Получает и задает данные формулы.

```csharp
public string Formula { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyFormulaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить изображение на лист
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Установите формулу для картинки
            picture.Formula = "A1:A3";
            Console.WriteLine("Picture Formula: " + picture.Formula);

            // Измените формулу
            picture.Formula = "B1:B3";
            Console.WriteLine("Updated Picture Formula: " + picture.Formula);

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


