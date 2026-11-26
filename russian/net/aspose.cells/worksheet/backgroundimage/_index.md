---
title: "Worksheet.BackgroundImage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Получает и задаёт фоновое изображение листа"
type: docs
url: /ru/net/aspose.cells/worksheet/backgroundimage/
---
## Worksheet.BackgroundImage property

Получает и задает фоновое изображение рабочего листа.

```csharp
public byte[] BackgroundImage { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyBackgroundImageDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить первый лист
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Путь к файлу изображения
            string imagePath = "background.jpg";
            
            // Прочитайте файл изображения в массив байтов
            byte[] imageData = File.ReadAllBytes(imagePath);
            
            // Установите фоновое изображение для листа
            worksheet.BackgroundImage = imageData;
            
            // Сохраните книгу
            workbook.Save("WorksheetWithBackground.xlsx");
            
            Console.WriteLine("Worksheet background image set successfully.");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


