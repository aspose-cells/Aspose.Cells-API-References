---
title: "Style.Custom"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Представляет строку пользовательского числового формата этого объекта стиля. Если пользовательский числовой формат не установлен, например будет возвращён builtin числовой формат"
type: docs
url: /ru/net/aspose.cells/style/custom/
---
## Style.Custom property

Представляет строку пользовательского числового формата этого объекта стиля. Если пользовательский числовой формат не задан (например, числовой формат встроенный), будет возвращена пустая строка "".

```csharp
public string Custom { get; set; }
```

### Примечания

Возвращаемая пользовательская строка не зависит от культуры.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyCustomDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создать и применить пользовательский формат даты
            Style style = workbook.CreateStyle();
            style.Custom = "d-mmm-yy";
            
            cells["A1"].PutValue(new DateTime(2023, 10, 15));
            cells["A1"].SetStyle(style);

            // Отобразить отформатированное значение
            Console.WriteLine("Formatted value: " + cells["A1"].StringValue);
            
            // Сохраните книгу
            workbook.Save("StylePropertyCustomDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


