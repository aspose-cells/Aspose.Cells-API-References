---
title: "AdvancedFilter.ListRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AdvancedFilter. Возвращает диапазон списка этого расширенного фильтра"
type: docs
url: /ru/net/aspose.cells/advancedfilter/listrange/
---
## AdvancedFilter.ListRange property

Получает диапазон списка этого расширенного фильтра.

```csharp
public string ListRange { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AdvancedFilterPropertyListRangeDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Заполнить примерными данными
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Age");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue("Person " + (i-1));
                sheet.Cells["B" + i].PutValue(20 + i);
            }

            // Настройте расширенный фильтр
            AdvancedFilter filter = sheet.GetAdvancedFilter();
            // ListRange является только для чтения и устанавливается автоматически при создании фильтра
            // Мы можем только читать его, но не устанавливать напрямую
            
            // Отобразить диапазон списка (будет показан автоматически определённый диапазон)
            Console.WriteLine("Advanced Filter List Range: " + filter.ListRange);
            
            // Сохраните книгу
            workbook.Save("AdvancedFilterDemo.xlsx");
        }
    }
}
```

### См. также

* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


