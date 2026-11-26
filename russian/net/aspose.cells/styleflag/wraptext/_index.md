---
title: "StyleFlag.WrapText"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Настройка переноса текста будет применена"
type: docs
url: /ru/net/aspose.cells/styleflag/wraptext/
---
## StyleFlag.WrapText property

Настройка переноса текста будет применена.

```csharp
public bool WrapText { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyWrapTextDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте стиль с включённым переносом текста
            Style style = workbook.CreateStyle();
            style.IsTextWrapped = true;

            // Создайте флаг стиля и включите флаг WrapText
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;

            // Примените стиль к ячейке A1 с указанными флагами
            worksheet.Cells["A1"].PutValue("This is a long text that should wrap in the cell");
            worksheet.Cells.ApplyStyle(style, flag);

            // Автоматически подгоните высоту строки, чтобы увидеть переносимый текст
            worksheet.AutoFitRow(0);

            // Сохраните книгу
            workbook.Save("WrapTextDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


