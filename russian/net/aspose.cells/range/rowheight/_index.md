---
title: "Range.RowHeight"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Range. Устанавливает или получает высоту строк в этом диапазоне"
type: docs
url: /ru/net/aspose.cells/range/rowheight/
---
## Range.RowHeight property

Устанавливает или получает высоту строк в этом диапазоне

```csharp
public double RowHeight { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyRowHeightDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установите некоторые данные в первой строке
            worksheet.Cells["A1"].PutValue("This is a test");
            worksheet.Cells["B1"].PutValue("to demonstrate");
            worksheet.Cells["C1"].PutValue("RowHeight property");

            // Получите начальную высоту строки
            double initialHeight = worksheet.Cells.CreateRange("1:1").RowHeight;
            Console.WriteLine("Initial row height: " + initialHeight);

            // Автоподгонка строки
            worksheet.AutoFitRow(0);

            // Получите новую высоту строки после автоподгонки
            double newHeight = worksheet.Cells.CreateRange("1:1").RowHeight;
            Console.WriteLine("Row height after auto-fit: " + newHeight);

            // Вручную установите новую высоту строки
            worksheet.Cells.CreateRange("1:1").RowHeight = 30;
            Console.WriteLine("Row height after manual set: " + worksheet.Cells.CreateRange("1:1").RowHeight);
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


