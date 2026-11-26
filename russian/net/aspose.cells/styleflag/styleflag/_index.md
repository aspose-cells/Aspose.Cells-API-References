---
title: "StyleFlag.StyleFlag"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор StyleFlag. Создаёт объект со всеми флагами, установленными в false"
type: docs
url: /ru/net/aspose.cells/styleflag/styleflag/
---
## StyleFlag constructor

Создаёт объект со всеми флагами, установленными в false.

```csharp
public StyleFlag()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagMethodCtorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать полужирный стиль
            Style boldStyle = workbook.CreateStyle();
            boldStyle.Font.IsBold = true;

            // Примените стиль к строке 9 с помощью конструктора StyleFlag
            worksheet.Cells.ApplyRowStyle(9, boldStyle, new StyleFlag { FontBold = true });

            // Поместите значение в ячейку и проверьте стиль
            worksheet.Cells[9, 0].PutValue("Bold Text");

            // Сохраните книгу
            workbook.Save("output.xlsx");

            Console.WriteLine("Style applied successfully using StyleFlag constructor.");
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


