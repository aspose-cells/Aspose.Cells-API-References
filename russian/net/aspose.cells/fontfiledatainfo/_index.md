---
title: "Класс FontFileDataInfo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.FontFileDataInfo. Представляет информацию о данных файла шрифта"
type: docs
url: /ru/net/aspose.cells/fontfiledatainfo/
---
## FontFileDataInfo class

Представляет информационные данные файла шрифта.

```csharp
public class FontFileDataInfo
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Data](../../aspose.cells/fontfiledatainfo/data/) { get; } | Получает двоичные данные файла шрифта. |
| [FormatType](../../aspose.cells/fontfiledatainfo/formattype/) { get; } | Получает тип формата файла шрифта. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsClassFontFileDataInfoDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Пример: загрузка данных файла шрифта
            string fontFilePath = "arial.ttf";
            byte[] fontData = File.ReadAllBytes(fontFilePath);

            // Примечание: FontFileDataInfo нельзя напрямую создать, так как у него нет публичного конструктора
            // и его свойства только для чтения. В реальном сценарии вы бы получили экземпляр
            // из другого метода API (например FontConfigs.GetFontFileDataInfo())
            FontFileDataInfo fontInfo = null; // Would be populated by API call in real scenario

            // Продемонстрировать, как свойства использовались бы, если бы у нас был экземпляр
            if (fontInfo != null)
            {
                Console.WriteLine("Font format type: " + fontInfo.FormatType);
                Console.WriteLine("Font data length: " + (fontInfo.Data != null ? fontInfo.Data.Length.ToString() : "null"));
            }

            // Продемонстрировать интеграцию с Workbook
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text with custom font");

            // Сохраните книгу
            workbook.Save("FontFileDataInfoDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


