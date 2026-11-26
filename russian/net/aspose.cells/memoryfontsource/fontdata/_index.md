---
title: "MemoryFontSource.FontData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MemoryFontSource. Двоичные данные шрифта"
type: docs
url: /ru/net/aspose.cells/memoryfontsource/fontdata/
---
## MemoryFontSource.FontData property

Бинарные данные шрифта.

```csharp
public byte[] FontData { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class MemoryFontSourcePropertyFontDataDemo
    {
        public static void Run()
        {
            // Загрузить файл шрифта TrueType в память
            byte[] fontBytes = File.ReadAllBytes("arial.ttf");

            // Создать экземпляр MemoryFontSource с данными шрифта
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontBytes);

            // Отобразить текущее значение FontData (первые 10 байт для демонстрации)
            Console.WriteLine("FontData length: " + memoryFontSource.FontData.Length);
            Console.Write("First 10 bytes: ");
            for (int i = 0; i < 10 && i < memoryFontSource.FontData.Length; i++)
            {
                Console.Write(memoryFontSource.FontData[i].ToString("X2") + " ");
            }
            Console.WriteLine();

            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать настройки шрифта и добавить наш источник шрифта в памяти
            FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });

            // Применить конфигурацию шрифтов глобально (не только для конкретной книги)
            FontConfigs.DefaultFontName = "Arial";
            FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });

            // Создать стиль с пользовательским шрифтом
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;

            // Применить стиль к ячейке
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text using memory font source");

            // Сохраните книгу
            workbook.Save("MemoryFontSourceDemo.xlsx");
        }
    }
}
```

### См. также

* class [MemoryFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


