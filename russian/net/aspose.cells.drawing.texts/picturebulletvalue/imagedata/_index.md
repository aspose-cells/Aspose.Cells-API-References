---
title: "PictureBulletValue.ImageData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PictureBulletValue. Получает и задает данные изображения маркера"
type: docs
url: /ru/net/aspose.cells.drawing.texts/picturebulletvalue/imagedata/
---
## PictureBulletValue.ImageData property

Получает и задает данные изображения маркера.

```csharp
public byte[] ImageData { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;
    using System.IO;

    public class PictureBulletValuePropertyImageDataDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Создайте экземпляр PictureBulletValue
                PictureBulletValue bulletValue = new PictureBulletValue();
                
                // Продемонстрировать установку и получение ImageData
                byte[] sampleImageData = new byte[] { 0x01, 0x02, 0x03 }; // Sample data
                bulletValue.ImageData = sampleImageData;
                
                // Отобразить значение свойства ImageData
                Console.WriteLine("ImageData length: " + (bulletValue.ImageData?.Length ?? 0) + " bytes");
                
                // Показать свойство Type (только для чтения)
                Console.WriteLine("Bullet Type: " + bulletValue.Type);
                
                // Сохраните книгу
                workbook.Save("PictureBulletValueImageDataDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [PictureBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


