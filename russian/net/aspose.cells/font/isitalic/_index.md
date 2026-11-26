---
title: "Font.IsItalic"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Font. Получает или задает значение, указывающее, является ли шрифт курсивным"
type: docs
url: /ru/net/aspose.cells/font/isitalic/
---
## Font.IsItalic property

Получает или задает значение, указывающее, является ли шрифт курсивом.

```csharp
public bool IsItalic { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsItalicDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к стилю по умолчанию
            Style style = workbook.DefaultStyle;
            
            // Установить свойства шрифта, включая IsItalic
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.Font.IsItalic = true;
            
            // Применить стиль к ячейке A1
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Italic Text Example");
            
            // Сохраните книгу
            workbook.Save("FontPropertyIsItalicDemo.xlsx");
            
            // Проверить свойство курсивности
            Console.WriteLine("Font is italic: " + cell.GetStyle().Font.IsItalic);
        }
    }
}
```

### См. также

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


