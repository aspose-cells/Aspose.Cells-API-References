---
title: "ListObject.AutoFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListObject. Получает автофильтр этой таблицы"
type: docs
url: /ru/net/aspose.cells.tables/listobject/autofilter/
---
## ListObject.AutoFilter property

Получает автофильтр этой таблицы.

```csharp
public AutoFilter AutoFilter { get; }
```

### Примечания

Работает только когда [`HasAutoFilter`](../hasautofilter/) равно false.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyAutoFilterDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Mary");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Peter");
            worksheet.Cells["B4"].PutValue(35);

            // Создать ListObject
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject listObject = worksheet.ListObjects[index];

            // Изменить размер объекта списка, чтобы включить все данные
            listObject.Resize(0, 0, 4, 2, true);

            // Получить доступ и продемонстрировать функциональность AutoFilter
            if (listObject.AutoFilter != null)
            {
                // Применить фильтр к столбцу Age (столбец 2)
                listObject.AutoFilter.Filter(1, "25");
                
                // Показать отфильтрованные данные
                Console.WriteLine("Filtered Data:");
                for (int row = 1; row <= 4; row++)
                {
                    if (!worksheet.Cells.Rows[row].IsHidden)
                    {
                        Console.WriteLine($"{worksheet.Cells[row, 0].StringValue} - {worksheet.Cells[row, 1].IntValue}");
                    }
                }

                // Очистить фильтр
                listObject.AutoFilter.RemoveFilter(1);
            }

            // Сохраните книгу
            workbook.Save("ListObjectAutoFilterDemo.xlsx");
        }
    }
}
```

### См. также

* class [AutoFilter](../../../aspose.cells/autofilter/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


