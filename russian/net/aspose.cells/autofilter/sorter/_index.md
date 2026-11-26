---
title: "AutoFilter.Sorter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AutoFilter. Возвращает сортировщик данных"
type: docs
url: /ru/net/aspose.cells/autofilter/sorter/
---
## AutoFilter.Sorter property

Получает сортировщик данных.

```csharp
public DataSorter Sorter { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertySorterDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("C");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["B3"].PutValue(10);
            worksheet.Cells["A4"].PutValue("B");
            worksheet.Cells["B4"].PutValue(20);

            // Создать диапазон автофильтра
            worksheet.AutoFilter.Range = "A1:B4";

            // Получить автофильтр
            AutoFilter filter = worksheet.AutoFilter;

            // Применить фильтр
            filter.Filter(1, "10");

            // Сортировать, используя свойство Sorter
            filter.Sorter.Sort();

            // Сохраните книгу
            workbook.Save("AutoFilterPropertySorterDemo.xlsx");
        }
    }
}
```

### См. также

* class [DataSorter](../../datasorter/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


