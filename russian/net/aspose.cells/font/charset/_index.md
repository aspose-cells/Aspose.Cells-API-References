---
title: "Font.Charset"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Font. Представляет набор символов"
type: docs
url: /ru/net/aspose.cells/font/charset/
---
## Font.Charset property

Представляет набор символов.

```csharp
public int Charset { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyCharsetDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте стиль с конкретными свойствами шрифта, включая набор символов
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.Charset = 1; // ANSI_CHARSET

            // Применить стиль к ячейке
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Text with ANSI charset");

            // Создайте другой стиль с другим набором символов
            Style style2 = workbook.CreateStyle();
            style2.Font.Name = "Times New Roman";
            style2.Font.Size = 12;
            style2.Font.Charset = 2; // DEFAULT_CHARSET

            // Примените второй стиль к другой ячейке
            Cell cell2 = worksheet.Cells["A2"];
            cell2.SetStyle(style2);
            cell2.PutValue("Text with DEFAULT charset");

            // Сохраните книгу
            workbook.Save("FontCharsetDemo.xlsx");

            // Проверьте свойства набора символов
            Console.WriteLine("Cell A1 Font Charset: " + cell.GetStyle().Font.Charset);
            Console.WriteLine("Cell A2 Font Charset: " + cell2.GetStyle().Font.Charset);
        }
    }
}
```

### См. также

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


