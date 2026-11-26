---
title: "StyleFlag.VerticalAlignment"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Настройка вертикального выравнивания будет применена"
type: docs
url: /ru/net/aspose.cells/styleflag/verticalalignment/
---
## StyleFlag.VerticalAlignment property

Настройка вертикального выравнивания будет применена.

```csharp
public bool VerticalAlignment { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyVerticalAlignmentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Создайте стиль с вертикальным выравниванием
            Style style = workbook.CreateStyle();
            style.VerticalAlignment = TextAlignmentType.Center;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.Font.Color = Color.Blue;

            // Создайте флаг стиля, чтобы применять только вертикальное выравнивание и цвет шрифта
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.VerticalAlignment = true;
            styleFlag.FontColor = true;

            // Примените стиль к первой строке с помощью флага стиля
            Row row = sheet.Cells.Rows[0];
            row.ApplyStyle(style, styleFlag);

            // Установите некоторый текст в ячейках, чтобы увидеть эффект
            sheet.Cells["A1"].PutValue("Vertically Centered");
            sheet.Cells["B1"].PutValue("Blue Text");

            // Сохраните книгу
            workbook.Save("VerticalAlignmentDemo.xlsx");
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


