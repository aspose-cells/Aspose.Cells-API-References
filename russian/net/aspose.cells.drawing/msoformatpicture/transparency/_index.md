---
title: "MsoFormatPicture.Transparency"
second_title: "Справочник API Aspose.Cells для .NET"
description: "MsoFormatPicture property. Возвращает или задает степень прозрачности области значением от 0.0 (непрозрачный) до 1.0 (полностью прозрачный)"
type: docs
url: /ru/net/aspose.cells.drawing/msoformatpicture/transparency/
---
## MsoFormatPicture.Transparency property

Возвращает или задает степень прозрачности области значением от 0.0 (непрозрачный) до 1.0 (прозрачный).

```csharp
public double Transparency { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyTransparencyDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить две картинки на лист
            int index1 = worksheet.Pictures.Add(0, 0, "image1.png");
            int index2 = worksheet.Pictures.Add(2, 0, "image2.png");

            // Установить прозрачность для картинок
            worksheet.Pictures[index1].FormatPicture.Transparency = 0.5;
            worksheet.Pictures[index2].FormatPicture.Transparency = 0.69;

            // Сохранить и перезагрузить книгу, чтобы проверить настройки прозрачности
            string outputPath = "output.xlsx";
            workbook.Save(outputPath);
            
            Workbook loadedWorkbook = new Workbook(outputPath);
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];

            // Вывести значения прозрачности в консоль
            Console.WriteLine("Picture 1 Transparency: " + loadedWorksheet.Pictures[0].FormatPicture.Transparency);
            Console.WriteLine("Picture 2 Transparency: " + loadedWorksheet.Pictures[1].FormatPicture.Transparency);
        }
    }
}
```

### См. также

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


