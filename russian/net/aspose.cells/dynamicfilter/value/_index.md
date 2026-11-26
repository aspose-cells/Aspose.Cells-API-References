---
title: "DynamicFilter.Value"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DynamicFilter. Получает и задаёт значение динамического фильтра"
type: docs
url: /ru/net/aspose.cells/dynamicfilter/value/
---
## DynamicFilter.Value property

Получает и задает значение динамического фильтра.

```csharp
public object Value { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterPropertyValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 20));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 10));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 5));

            // Создать автофильтр
            worksheet.AutoFilter.Range = "A1:A5";
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);
            DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

            // Отобразите текущее значение фильтра
            Console.WriteLine("Current DynamicFilter Value: " + filter.Value);

            // Измените значение фильтра, чтобы показать даты апреля
            filter.Value = new DateTime(2023, 4, 1);
            filter.DynamicFilterType = DynamicFilterType.April;

            // Применить фильтр
            worksheet.AutoFilter.Refresh();

            // Сохранить результат
            workbook.Save("DynamicFilterValueDemo.xlsx");
        }
    }
}
```

### См. также

* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


