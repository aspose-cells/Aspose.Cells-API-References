---
title: "Font.Underline"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Font. Получает или задает тип подчеркивания шрифта"
type: docs
url: /ru/net/aspose.cells/font/underline/
---
## Font.Underline property

Получает или задает тип подчеркивания шрифта.

```csharp
public FontUnderlineType Underline { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyUnderlineDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Получить доступ к ячейке и установить стиль подчеркивания
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Sample Underlined Text");
            
            // Получить стиль и изменить свойства шрифта
            Style style = cell.GetStyle();
            style.Font.Underline = FontUnderlineType.Single;
            cell.SetStyle(style);

            // Сохраните книгу
            workbook.Save("FontUnderlineDemo.xlsx");
        }
    }
}
```

### См. также

* enum [FontUnderlineType](../../fontunderlinetype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


