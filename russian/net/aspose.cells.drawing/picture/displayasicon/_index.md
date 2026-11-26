---
title: "Picture.DisplayAsIcon"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Picture. True, если указанный объект отображается как значок и изображение не будет автоматически изменено"
type: docs
url: /ru/net/aspose.cells.drawing/picture/displayasicon/
---
## Picture.DisplayAsIcon property

True, если указанный объект отображается как значок и изображение не будет автоматически изменено.

```csharp
public bool DisplayAsIcon { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyDisplayAsIconDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить изображение на лист
            int pictureIndex = worksheet.Pictures.Add(1, 1, "example.ico");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Установить свойство DisplayAsIcon в true
            picture.DisplayAsIcon = true;
            
            // Установить другие свойства изображения
            picture.Name = "IconDisplay";
            picture.Height = 100;
            picture.Width = 100;

            // Сохраните книгу
            workbook.Save("DisplayAsIconDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Workbook saved with icon display picture.");
        }
    }
}
```

### См. также

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


