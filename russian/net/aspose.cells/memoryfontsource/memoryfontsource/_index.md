---
title: "MemoryFontSource.MemoryFontSource"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор MemoryFontSource. Ctor"
type: docs
url: /ru/net/aspose.cells/memoryfontsource/memoryfontsource/
---
## MemoryFontSource constructor

Конструктор.

```csharp
public MemoryFontSource(byte[] fontData)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fontData | Byte[] | Бинарные данные шрифта. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class MemoryFontSourceMethodCtorWithByteArrayDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Загрузить файл TrueType шрифта в массив байтов
                byte[] fontData = File.ReadAllBytes("arial.ttf");
                
                // Вызвать метод #ctor с параметром массив байтов
                MemoryFontSource fontSource = new MemoryFontSource(fontData);
                
                // Установить источники шрифтов с помощью статического класса FontConfigs
                FontConfigs.SetFontSources(new FontSourceBase[] { fontSource });
                
                // Проверить свойства источника шрифта
                Console.WriteLine($"Font source type: {fontSource.Type}");
                Console.WriteLine($"Font data length: {fontSource.FontData.Length} bytes");
                
                // Использовать шрифт в ячейке
                Worksheet worksheet = workbook.Worksheets[0];
                var style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                worksheet.Cells["A1"].PutValue("Text with custom font");
                worksheet.Cells["A1"].SetStyle(style);
                
                Console.WriteLine("MemoryFontSource constructor executed successfully with byte array parameter");
            }
            catch (FileNotFoundException ex)
            {
                Console.WriteLine($"Error: Font file not found. {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing MemoryFontSource constructor: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("MemoryFontSourceCtorDemo.xlsx");
        }
    }
}
```

### См. также

* class [MemoryFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


