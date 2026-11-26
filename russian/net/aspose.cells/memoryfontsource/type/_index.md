---
title: "MemoryFontSource.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MemoryFontSource. Возвращает тип источника шрифта"
type: docs
url: /ru/net/aspose.cells/memoryfontsource/type/
---
## MemoryFontSource.Type property

Возвращает тип источника шрифтов.

```csharp
public override FontSourceType Type { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class MemoryFontSourcePropertyTypeDemo
    {
        public static void Run()
        {
            // Загрузить файл шрифта TrueType в память
            byte[] fontData = File.ReadAllBytes("arial.ttf");

            // Создать экземпляр MemoryFontSource с данными шрифта
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);

            // Отобразить текущее значение Type
            Console.WriteLine("MemoryFontSource Type: " + memoryFontSource.Type);

            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить источники шрифтов с помощью FontConfigs
            FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });

            // Проверить, что тип источника шрифта — MemoryFont
            if (memoryFontSource.Type == FontSourceType.MemoryFont)
            {
                // Использовать шрифт в ячейке
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].PutValue("Text using memory font source");

                // Добавить информацию о типе источника шрифта
                worksheet.Cells["A2"].PutValue("Font source type: " + memoryFontSource.Type);
            }

            // Сохраните книгу
            workbook.Save("MemoryFontSourceTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [FontSourceType](../../fontsourcetype/)
* class [MemoryFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


