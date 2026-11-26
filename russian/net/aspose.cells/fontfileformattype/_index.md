---
title: "Enum FontFileFormatType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.FontFileFormatType enum. Представляет тип формата шрифта"
type: docs
url: /ru/net/aspose.cells/fontfileformattype/
---
## FontFileFormatType enumeration

Представляет тип формата шрифта.

```csharp
public enum FontFileFormatType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Unknown | `0` | Неизвестный тип формата шрифта. |
| Ttf | `1` | Тип формата шрифта TTF. |
| Otf | `2` | Тип формата шрифта OTF. |
| Ttc | `3` | Тип формата шрифта TTC. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassFontFileFormatTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получите доступ к ячейке и задайте её стиль
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Font Format Type Demo");
            Style style = cell.GetStyle();

            // Продемонстрировать использование FontFileFormatType
            FontFileFormatType fontFormat = FontFileFormatType.Ttf;
            Console.WriteLine("Selected font format: " + fontFormat.ToString());

            // Применить настройки шрифта
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            cell.SetStyle(style);

            // Проверить совместимость формата шрифта
            if (fontFormat == FontFileFormatType.Ttf)
            {
                Console.WriteLine("Using TrueType font format");
            }

            // Сохраните книгу
            workbook.Save("FontFileFormatTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


