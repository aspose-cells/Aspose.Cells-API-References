---
title: "Style.HorizontalAlignment"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Style property. Получает или задает тип горизонтального выравнивания текста в ячейке"
type: docs
url: /ru/net/aspose.cells/style/horizontalalignment/
---
## Style.HorizontalAlignment property

Получает или задает тип горизонтального выравнивания текста в ячейке.

```csharp
public TextAlignmentType HorizontalAlignment { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установить текст в ячейках
            cells["A1"].PutValue("Left Aligned");
            cells["A2"].PutValue("Center Aligned");
            cells["A3"].PutValue("Right Aligned");

            // Получить объекты стиля
            Style styleLeft = cells["A1"].GetStyle();
            Style styleCenter = cells["A2"].GetStyle();
            Style styleRight = cells["A3"].GetStyle();

            // Установить горизонтальное выравнивание
            styleLeft.HorizontalAlignment = TextAlignmentType.Left;
            styleCenter.HorizontalAlignment = TextAlignmentType.Center;
            styleRight.HorizontalAlignment = TextAlignmentType.Right;

            // Применить стили к ячейкам
            cells["A1"].SetStyle(styleLeft);
            cells["A2"].SetStyle(styleCenter);
            cells["A3"].SetStyle(styleRight);

            // Сохраните книгу
            workbook.Save("HorizontalAlignmentDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


