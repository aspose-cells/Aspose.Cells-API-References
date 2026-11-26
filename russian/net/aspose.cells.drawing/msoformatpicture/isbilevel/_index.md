---
title: "MsoFormatPicture.IsBiLevel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "MsoFormatPicture property. Указывает, должно ли это изображение отображаться в двухцветном черно‑белом режиме"
type: docs
url: /ru/net/aspose.cells.drawing/msoformatpicture/isbilevel/
---
## MsoFormatPicture.IsBiLevel property

Указывает, должно ли это изображение отображаться в двухцветном черно-белом режиме.

```csharp
public bool IsBiLevel { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyIsBiLevelDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить изображение на лист
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[index];
            
            // Установить изображение в двуцветный режим (черно‑белый)
            picture.FormatPicture.IsBiLevel = true;
            
            // Проверьте и выведите значение свойства IsBiLevel
            Console.WriteLine("Picture is bi-level: " + picture.FormatPicture.IsBiLevel);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


