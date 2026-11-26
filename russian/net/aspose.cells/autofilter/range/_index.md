---
title: "AutoFilter.Range"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AutoFilter. Представляет диапазон, к которому применяется указанный автофильтр"
type: docs
url: /ru/net/aspose.cells/autofilter/range/
---
## AutoFilter.Range property

Представляет диапазон, к которому применяется указанный AutoFilter.

```csharp
public string Range { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertyRangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("Header");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["A4"].PutValue("Item3");
            sheet.Cells["A5"].PutValue("Item4");

            // Примените автофильтр к диапазону A1:A5
            sheet.AutoFilter.Range = "A1:A5";

            // Отобразить диапазон автофильтра
            Console.WriteLine("AutoFilter Range: " + sheet.AutoFilter.Range);

            // Сохраните книгу
            workbook.Save("AutoFilterRangeDemo.xlsx");
        }
    }
}
```

### См. также

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


