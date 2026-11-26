---
title: "StyleFlag.Indent"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Параметр уровня отступа будет применён"
type: docs
url: /ru/net/aspose.cells/styleflag/indent/
---
## StyleFlag.Indent property

Настройка уровня отступа будет применена.

```csharp
public bool Indent { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyIndentDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте стиль с уровнем отступа
            Style style = workbook.CreateStyle();
            style.IndentLevel = 2;
            style.HorizontalAlignment = TextAlignmentType.Left;

            // Создайте флаг стиля с установленным свойством Indent
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Indent = true;

            // Примените данные к ячейкам
            for (int row = 0; row < 5; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    worksheet.Cells[row, col].PutValue($"Cell {row},{col}");
                }
            }

            // Примените стиль с отступом к диапазону
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 5, 5);
            range.ApplyStyle(style, styleFlag);

            // Проверьте, что стиль был применён
            Cell cell = worksheet.Cells["A1"];
            Style appliedStyle = cell.GetStyle();
            Console.WriteLine($"Indent Level: {appliedStyle.IndentLevel}");
            Console.WriteLine($"Alignment: {appliedStyle.HorizontalAlignment}");

            // Сохраните книгу
            workbook.Save("IndentStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


