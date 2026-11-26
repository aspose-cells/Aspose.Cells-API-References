---
title: "ListObject.QueryTable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ListObject. Возвращает связанный QueryTable"
type: docs
url: /ru/net/aspose.cells.tables/listobject/querytable/
---
## ListObject.QueryTable property

Получает связанную QueryTable.

```csharp
public QueryTable QueryTable { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListObjectPropertyQueryTableDemo
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
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Создать объект списка
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[index];

            try
            {
                // Получить доступ к свойству QueryTable (только для чтения)
                QueryTable queryTable = listObject.QueryTable;

                if (queryTable != null)
                {
                    // Отобразить свойства QueryTable
                    Console.WriteLine("QueryTable Name: " + queryTable.Name);
                    Console.WriteLine("Connection ID: " + queryTable.ConnectionId);
                    Console.WriteLine("Preserve Formatting: " + queryTable.PreserveFormatting);
                    Console.WriteLine("Adjust Column Width: " + queryTable.AdjustColumnWidth);

                    // Получить доступ к диапазону результата, если он доступен
                    if (queryTable.ResultRange != null)
                    {
                        Console.WriteLine("Result Range Address: " + queryTable.ResultRange.Name);
                    }
                }
                else
                {
                    Console.WriteLine("No QueryTable associated with this ListObject");
                }

                // Сохраните книгу
                workbook.Save("QueryTableDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [QueryTable](../../../aspose.cells/querytable/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


