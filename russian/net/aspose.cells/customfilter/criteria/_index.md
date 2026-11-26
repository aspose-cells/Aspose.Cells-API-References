---
title: "CustomFilter.Criteria"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CustomFilter. Получает и задаёт критерий"
type: docs
url: /ru/net/aspose.cells/customfilter/criteria/
---
## CustomFilter.Criteria property

Получает и задает критерий.

```csharp
public object Criteria { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomFilterPropertyCriteriaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Numbers");
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["A4"].PutValue(5);
            worksheet.Cells["A5"].PutValue(9);
            worksheet.Cells["A6"].PutValue(3);

            // Применить автофильтр
            worksheet.AutoFilter.Range = "A1:A6";
            AutoFilter autoFilter = worksheet.AutoFilter;
            
            // Добавить пользовательский фильтр
            int fieldIndex = 0;
            autoFilter.Custom(fieldIndex, FilterOperatorType.GreaterOrEqual, 5);
            
            // Получить столбец фильтра и отобразить критерий
            FilterColumn fc = autoFilter.FilterColumns[fieldIndex];
            CustomFilter cf = ((CustomFilterCollection)fc.Filter)[0];
            Console.WriteLine("Filter Criteria: " + cf.Criteria);
            
            // Обновить фильтр
            autoFilter.Refresh();
            
            // Сохраните книгу
            workbook.Save("CustomFilterExample.xlsx");
        }
    }
}
```

### См. также

* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


