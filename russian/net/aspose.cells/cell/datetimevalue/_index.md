---
title: "Cell.DateTimeValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Получает значение DateTime, содержащееся в ячейке"
type: docs
url: /ru/net/aspose.cells/cell/datetimevalue/
---
## Cell.DateTimeValue property

Получает значение DateTime, содержащееся в ячейке.

```csharp
public DateTime DateTimeValue { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyDateTimeValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установите значение DateTime в ячейку A1
            DateTime testDate = new DateTime(2023, 12, 25);
            cells["A1"].PutValue(testDate);

            // Отформатируйте ячейку для отображения даты
            Style style = cells["A1"].GetStyle();
            style.Custom = "yyyy-MM-dd";
            cells["A1"].SetStyle(style);

            // Получите и проверьте DateTimeValue
            DateTime retrievedDate = cells["A1"].DateTimeValue;
            Console.WriteLine("Original DateTime: " + testDate.ToString("yyyy-MM-dd"));
            Console.WriteLine("Retrieved DateTime: " + retrievedDate.ToString("yyyy-MM-dd"));

            // Установите другое значение DateTime в ячейку B1
            DateTime anotherDate = new DateTime(2024, 1, 1);
            cells["B1"].PutValue(anotherDate);

            // Отобразите DateTimeValue из B1
            Console.WriteLine("B1 DateTime: " + cells["B1"].DateTimeValue.ToString("yyyy-MM-dd"));
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


