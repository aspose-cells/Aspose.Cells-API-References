---
title: "Style.IsNumberFormatApplied"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Указывает, следует ли применять числовое форматирование"
type: docs
url: /ru/net/aspose.cells/style/isnumberformatapplied/
---
## Style.IsNumberFormatApplied property

Указывает, следует ли применять числовое форматирование.

```csharp
public bool IsNumberFormatApplied { get; set; }
```

### Примечания

Только для именованного стиля.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsNumberFormatAppliedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать стиль с числовым форматом
            Style style = workbook.CreateStyle();
            style.Number = 14; // Format as "m/d/yyyy"
            style.IsNumberFormatApplied = true;
            
            // Применить стиль к ячейке
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            // Проверить, что числовой формат применён
            Console.WriteLine("IsNumberFormatApplied: " + style.IsNumberFormatApplied);
            Console.WriteLine("Cell value format: " + cell.GetDisplayStyle().Number);
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


