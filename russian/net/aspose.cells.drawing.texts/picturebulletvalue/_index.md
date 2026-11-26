---
title: "Класс PictureBulletValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.Texts.PictureBulletValue. Представляет значение графического маркера"
type: docs
url: /ru/net/aspose.cells.drawing.texts/picturebulletvalue/
---
## PictureBulletValue class

Представляет значение изображённого маркера.

```csharp
public class PictureBulletValue : BulletValue
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PictureBulletValue](picturebulletvalue/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [ImageData](../../aspose.cells.drawing.texts/picturebulletvalue/imagedata/) { get; set; } | Получает и задает данные изображения маркера. |
| override [Type](../../aspose.cells.drawing.texts/picturebulletvalue/type/) { get; } | Получает тип значения маркера. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;
    using System.IO;

    public class TextsClassPictureBulletValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Создайте экземпляр класса PictureBulletValue
                PictureBulletValue bulletValue = new PictureBulletValue();
                
                // Загрузите примерные данные изображения (замените реальным путем к изображению)
                string imagePath = "sample.png";
                if (File.Exists(imagePath))
                {
                    bulletValue.ImageData = File.ReadAllBytes(imagePath);
                    
                    // Отобразить базовую информацию
                    Console.WriteLine($"PictureBulletValue created with Type: {bulletValue.Type}");
                    Console.WriteLine($"Image data length: {bulletValue.ImageData?.Length ?? 0} bytes");
                }
                else
                {
                    Console.WriteLine("Sample image not found, using empty bullet value");
                }
                
                // Сохраните книгу
                workbook.Save("PictureBulletValueDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PictureBulletValue: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


