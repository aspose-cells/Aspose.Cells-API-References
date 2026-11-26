---
title: "ConditionalFormattingIcon.GetIconImageData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ConditionalFormattingIcon. Получить данные набора значков"
type: docs
url: /ru/net/aspose.cells/conditionalformattingicon/geticonimagedata/
---
## ConditionalFormattingIcon.GetIconImageData method

Получить данные набора значков

```csharp
public static byte[] GetIconImageData(IconSetType type, int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | IconSetType | тип значка |
| индекс | Int32 | индекс значка |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class ConditionalFormattingIconMethodGetIconImageDataWithIconSetTypeInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Не требуется создавать экземпляр, так как GetIconImageData является статическим
            
            try
            {
                // Вызвать GetIconImageData с IconSetType.Arrows3 и индексом 0
                byte[] imageData = ConditionalFormattingIcon.GetIconImageData(IconSetType.Arrows3, 0);
                
                Console.WriteLine("Method executed successfully. Image data length: " + imageData.Length);
                
                // Сохранить данные изображения в файл для демонстрации
                File.WriteAllBytes("icon_image.png", imageData);
                Console.WriteLine("Icon image saved to icon_image.png");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetIconImageData method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("ConditionalFormattingIconGetIconImageDataDemo.xlsx");
        }
    }
}
```

### См. также

* enum [IconSetType](../../iconsettype/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


