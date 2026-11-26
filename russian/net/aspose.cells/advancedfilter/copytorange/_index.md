---
title: "AdvancedFilter.CopyToRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AdvancedFilter. Возвращает диапазон, в который копируется результат этого расширенного фильтра"
type: docs
url: /ru/net/aspose.cells/advancedfilter/copytorange/
---
## AdvancedFilter.CopyToRange property

Получает диапазон, в который копируется результат этого расширенного фильтра.

```csharp
public string CopyToRange { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AdvancedFilterPropertyCopyToRangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить первый лист
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1.5);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(0.8);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(1.2);

            // Добавить диапазон критериев
            worksheet.Cells["D1"].PutValue("Product");
            worksheet.Cells["D2"].PutValue("Apple");

            try
            {
                // Получите экземпляр AdvancedFilter из листа
                AdvancedFilter advancedFilter = worksheet.GetAdvancedFilter();

                // Отобразить значение свойства CopyToRange
                Console.WriteLine("CopyToRange value: " + advancedFilter.CopyToRange);

                // Сохраните книгу
                workbook.Save("CopyToRangeDemo.xlsx");
                Console.WriteLine("CopyToRange demonstration completed successfully.");
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

* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


