---
title: "Style.IndentLevel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Представляет уровень отступа для ячейки или диапазона. Может быть только целым числом от 0 до 250"
type: docs
url: /ru/net/aspose.cells/style/indentlevel/
---
## Style.IndentLevel property

Представляет уровень отступа для ячейки или диапазона. Может быть только целым числом от 0 до 250.

```csharp
public int IndentLevel { get; set; }
```

### Примечания

Если тип горизонтального выравнивания текста установлен в значение, отличное от left или right, уровень отступа будет сброшен до нуля.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIndentLevelDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установите разные уровни отступа для ячеек
            for (int i = 0; i < 16; i++)
            {
                Cell cell = cells[i, 0];
                Style style = cell.GetStyle();
                style.IndentLevel = i;
                style.HorizontalAlignment = TextAlignmentType.Left;
                cell.SetStyle(style);
                cell.PutValue($"Indent Level {i}");
            }

            // Сохраните книгу
            workbook.Save("IndentLevelDemo.xlsx");
            Console.WriteLine("Workbook saved with different indent levels.");
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


