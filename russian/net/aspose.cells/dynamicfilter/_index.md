---
title: "Класс DynamicFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.DynamicFilter. Представляет динамический фильтр"
type: docs
url: /ru/net/aspose.cells/dynamicfilter/
---
## DynamicFilter class

Представляет динамический фильтр.

```csharp
public class DynamicFilter
```

## Свойства

| Имя | Описание |
| --- | --- |
| [DynamicFilterType](../../aspose.cells/dynamicfilter/dynamicfiltertype/) { get; set; } | Получает и задает тип этого динамического фильтра. |
| [MaxValue](../../aspose.cells/dynamicfilter/maxvalue/) { get; set; } | Получает и задает максимальное значение динамического фильтра. |
| [Value](../../aspose.cells/dynamicfilter/value/) { get; set; } | Получает и задает значение динамического фильтра. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassDynamicFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Создать книгу и лист (необязательно для контекста)
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Name = "DemoSheet";

                // Заполнить примерными числовыми данными
                worksheet.Cells["A1"].PutValue("Numbers");
                worksheet.Cells["A2"].PutValue(10);
                worksheet.Cells["A3"].PutValue(20);
                worksheet.Cells["A4"].PutValue(30);
                worksheet.Cells["A5"].PutValue(40);
                worksheet.Cells["A6"].PutValue(50);

                // Определить диапазон автофильтра
                worksheet.AutoFilter.Range = "A1:A6";

                // Применить динамический фильтр (AboveAverage) к первому столбцу
                worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.AboveAverage);

                // Получить экземпляр DynamicFilter, созданный AutoFilter
                DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

                // Установите дополнительные свойства, если необходимо
                filter.Value = 25;      // Example custom value
                filter.MaxValue = 45;   // Example max value

                // Отобразить заданные свойства
                Console.WriteLine($"DynamicFilterType: {filter.DynamicFilterType}");
                Console.WriteLine($"Value: {filter.Value}");
                Console.WriteLine($"MaxValue: {filter.MaxValue}");

                // Обновите фильтр, чтобы применить изменения
                worksheet.AutoFilter.Refresh();

                // Сохранить книгу (отфильтрованные данные будут сохранены)
                workbook.Save("DynamicFilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DynamicFilter: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


