---
title: "OleObject.ImageSourceFullName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OleObject. Получает или задаёт путь и имя исходного файла для связанного изображения"
type: docs
url: /ru/net/aspose.cells.drawing/oleobject/imagesourcefullname/
---
## OleObject.ImageSourceFullName property

Получает или задает путь и имя исходного файла для связанного изображения.

```csharp
public string ImageSourceFullName { get; set; }
```

### Примечания

Значение по умолчанию — пустая строка. Если SourceFullName не является пустой строкой, изображение связывается. Если SourceFullName не является пустой строкой, но Data равно null, тогда изображение связывается и не сохраняется в файле.

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyImageSourceFullNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Пример PDF‑файла для встраивания
            byte[] pdfBytes = File.ReadAllBytes("example.pdf");

            // Добавить OleObject в worksheet
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, pdfBytes);
            OleObject oleObj = worksheet.OleObjects[oleIndex];

            // Установите свойства OleObject, включая ImageSourceFullName
            oleObj.DisplayAsIcon = false;
            oleObj.FileFormatType = FileFormatType.Pdf;
            oleObj.ImageSourceFullName = "sample_image.png"; // Demonstrating ImageSourceFullName usage
            oleObj.IsAutoSize = false;
            oleObj.IsLink = false;
            oleObj.ProgID = "Acrobat.Document.DC";

            // Сохраните книгу
            workbook.Save("OleObjectDemo.xlsx");
        }
    }
}
```

### См. также

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


