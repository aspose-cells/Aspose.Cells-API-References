---
title: "ListObject.HasAutoFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListObject. Указывает, применяется ли автофильтр к этой таблице"
type: docs
url: /ru/net/aspose.cells.tables/listobject/hasautofilter/
---
## ListObject.HasAutoFilter property

Указывает, применён ли автофильтр к этой таблице.

```csharp
public bool HasAutoFilter { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Tables;

    public class ListObjectPropertyHasAutoFilterDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить таблицу образцовыми данными
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("Alice");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Bob");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Charlie");
            worksheet.Cells["B4"].PutValue(78);

            try
            {
                // Добавить ListObject (таблицу), охватывающую диапазон данных
                int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
                ListObject listObject = worksheet.ListObjects[tableIndex];

                // Убедиться, что таблица изменена по размеру, чтобы включать все строки
                listObject.Resize(0, 0, 4, 2, true);

                // Прочитать и отобразить значение свойства HasAutoFilter
                bool hasFilter = listObject.HasAutoFilter;
                Console.WriteLine("HasAutoFilter: " + hasFilter);

                // Объект AutoFilter можно получить через свойство AutoFilter
                // Продемонстрировать, что он не равен null, когда HasAutoFilter истинно
                if (hasFilter && listObject.AutoFilter != null)
                {
                    // Применить простой фильтр к столбцу "Score" (индекс 1), чтобы показать строки с Score >= 80
                    listObject.AutoFilter.Filter(1, ">=80");

                    Console.WriteLine("Filtered rows (Score >= 80):");
                    for (int row = 1; row <= 4; row++)
                    {
                        // Использовать Cells.Rows, чтобы проверить, скрыта ли строка
                        if (!worksheet.Cells.Rows[row].IsHidden)
                        {
                            Console.WriteLine($"{worksheet.Cells[row, 0].StringValue} - {worksheet.Cells[row, 1].IntValue}");
                        }
                    }

                    // Очистить фильтр
                    listObject.AutoFilter.RemoveFilter(1);
                }

                // Сохраните книгу (необязательно)
                workbook.Save("HasAutoFilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### См. также

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


