---
title: "DynamicFilter.DynamicFilterType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DynamicFilter. Получает и задает тип этого динамического фильтра"
type: docs
url: /ru/net/aspose.cells/dynamicfilter/dynamicfiltertype/
---
## DynamicFilter.DynamicFilterType property

Получает и задает тип этого динамического фильтра.

```csharp
public DynamicFilterType DynamicFilterType { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterPropertyDynamicFilterTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные с датами
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 20));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 10));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 5));

            try
            {
                // Создать автофильтр
                worksheet.AutoFilter.Range = "A1:A5";

                // Применить динамический фильтр для дат марта
                worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);

                // Получить экземпляр DynamicFilter
                DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

                // Отобразить текущее значение DynamicFilterType
                Console.WriteLine("Current DynamicFilterType: " + filter.DynamicFilterType);

                // Изменить тип фильтра, чтобы показать даты апреля
                filter.DynamicFilterType = DynamicFilterType.April;

                // Отобразить обновленное значение DynamicFilterType
                Console.WriteLine("Updated DynamicFilterType: " + filter.DynamicFilterType);

                // Применить фильтр
                worksheet.AutoFilter.Refresh();

                // Сохранить результат
                workbook.Save("DynamicFilterTypeDemo.xlsx");
                Console.WriteLine("DynamicFilterType has been demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [DynamicFilterType](../../dynamicfiltertype/)
* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


