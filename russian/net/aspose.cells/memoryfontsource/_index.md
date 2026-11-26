---
title: "Класс MemoryFontSource"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.MemoryFontSource. Представляет один файл шрифта TrueType, хранящийся в памяти"
type: docs
url: /ru/net/aspose.cells/memoryfontsource/
---
## MemoryFontSource class

Представляет отдельный файл шрифта TrueType, хранящийся в памяти.

```csharp
public class MemoryFontSource : FontSourceBase
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [MemoryFontSource](memoryfontsource/)(byte[]) | Конструктор. |

## Свойства

| Имя | Описание |
| --- | --- |
| [FontData](../../aspose.cells/memoryfontsource/fontdata/) { get; } | Бинарные данные шрифта. |
| override [Type](../../aspose.cells/memoryfontsource/type/) { get; } | Возвращает тип источника шрифтов. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsClassMemoryFontSourceDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Загрузить файл шрифта TrueType в память
            byte[] fontData = File.ReadAllBytes("arial.ttf");

            // Создать экземпляр MemoryFontSource с данными шрифта
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);

            // Создать массив источников шрифтов, содержащий наш MemoryFontSource
            FontSourceBase[] fontSources = new FontSourceBase[] { memoryFontSource };

            // Установить источники шрифтов с помощью FontConfigs
            FontConfigs.SetFontSources(fontSources);

            // Использовать пользовательский шрифт в ячейке
            worksheet.Cells["A1"].PutValue("Text with custom font from memory");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            worksheet.Cells["A1"].SetStyle(style);

            // Сохраните книгу
            workbook.Save("MemoryFontSourceDemo.xlsx");
        }
    }
}
```

### См. также

* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


