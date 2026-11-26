---
title: "ReferredArea.StartRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ReferredArea. Начальная строка области"
type: docs
url: /ru/net/aspose.cells/referredarea/startrow/
---
## ReferredArea.StartRow property

Начальная строка области.

```csharp
public int StartRow { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyStartRowDemo
    {
        public static void Run()
        {
            // Создайте книгу и лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить некоторыми примерными данными
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);

            // Создать именованный диапазон, который ссылается на A2:A4
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$2:$A$4";

            // Получить ссылочную область с параметром пересчёта
            ReferredArea area = name.GetReferredAreas(false)[0];

            // Продемонстрировать свойство StartRow
            Console.WriteLine("Start Row: " + area.StartRow); // Should output 1 (0-based)
            Console.WriteLine("End Row: " + area.EndRow);     // Should output 3 (0-based)
            Console.WriteLine("Row Count: " + (area.EndRow - area.StartRow + 1)); // Should output 3

            // Итерировать по ссылочной области, используя StartRow и EndRow
            for (int row = area.StartRow; row <= area.EndRow; row++)
            {
                Cell cell = worksheet.Cells[row, 0]; // Column 0 is A
                Console.WriteLine("Value at row " + row + ": " + cell.Value);
            }
        }
    }
}
```

### См. также

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


