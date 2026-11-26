---
title: "Style.IsDateTime"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Указывает, является ли числовой формат датой"
type: docs
url: /ru/net/aspose.cells/style/isdatetime/
---
## Style.IsDateTime property

Указывает, является ли числовой формат датой.

```csharp
public bool IsDateTime { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsDateTimeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Установить числовое значение
            cells["A1"].PutValue(1230);
            
            // Получить и изменить стиль ячейки
            Style style = cells["A1"].GetStyle();
            
            // Установить в формат даты (15 — встроенный формат даты)
            style.Number = 15;
            Console.WriteLine("IsDateTime after setting Number=15: " + style.IsDateTime);
            
            // Установить пользовательский формат даты
            style.Custom = "yyyy-mm-dd";
            Console.WriteLine("IsDateTime after setting custom date format: " + style.IsDateTime);
            
            // Применить изменённый стиль к ячейке
            cells["A1"].SetStyle(style);
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


