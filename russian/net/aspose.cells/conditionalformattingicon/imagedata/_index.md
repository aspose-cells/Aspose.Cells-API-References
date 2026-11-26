---
title: "ConditionalFormattingIcon.ImageData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ConditionalFormattingIcon. Получает данные набора значков"
type: docs
url: /ru/net/aspose.cells/conditionalformattingicon/imagedata/
---
## ConditionalFormattingIcon.ImageData property

Получает данные набора значков.

```csharp
public byte[] ImageData { get; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingIconPropertyImageDataDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные и условное форматирование
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // Получите результат условного форматирования
            var conditionalFormattingResult = worksheet.Cells["A1"].GetConditionalFormattingResult();
            if (conditionalFormattingResult != null)
            {
                ConditionalFormattingIcon icon = conditionalFormattingResult.ConditionalFormattingIcon;
                if (icon != null)
                {
                    // Получите данные изображения значка
                    byte[] imageData = icon.ImageData;
                    
                    // Проверьте и отобразите информацию об изображении
                    if (imageData != null && imageData.Length > 0)
                    {
                        Console.WriteLine($"Icon data length: {imageData.Length} bytes");
                    }
                }
            }
        }
    }
}
```

### См. также

* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


