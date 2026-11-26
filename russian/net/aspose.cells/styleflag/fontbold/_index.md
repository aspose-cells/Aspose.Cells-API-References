---
title: "StyleFlag.FontBold"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Будет применена настройка полужирного шрифта"
type: docs
url: /ru/net/aspose.cells/styleflag/fontbold/
---
## StyleFlag.FontBold property

Настройка полужирного шрифта будет применена.

```csharp
public bool FontBold { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontBoldDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать полужирный стиль
            Style boldStyle = workbook.CreateStyle();
            boldStyle.Font.IsBold = true;

            // Применить полужирный стиль к строке 2 с StyleFlag только для FontBold
            worksheet.Cells.ApplyRowStyle(1, boldStyle, new StyleFlag { FontBold = true });

            // Поместить значение в ячейку, чтобы продемонстрировать стиль
            worksheet.Cells[1, 0].PutValue("Bold Text");

            // Сохраните книгу
            workbook.Save("output.xlsx");

            Console.WriteLine("FontBold property demo completed successfully.");
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


