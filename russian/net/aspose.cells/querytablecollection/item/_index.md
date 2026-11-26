---
title: "QueryTableCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство QueryTableCollection. Получает querytable по указанному индексу"
type: docs
url: /ru/net/aspose.cells/querytablecollection/item/
---
## QueryTableCollection indexer

Получает querytable по указанному индексу.

```csharp
public QueryTable this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс. |

### Возвращаемое значение

Querytable

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTableCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить доступ к QueryTableCollection
            QueryTableCollection queryTables = worksheet.QueryTables;

            try
            {
                // Проверьте, есть ли какие‑либо QueryTables
                if (queryTables.Count > 0)
                {
                    // Получите доступ к первой QueryTable, используя свойство Item
                    QueryTable firstQueryTable = queryTables[0];
                    Console.WriteLine("First QueryTable accessed successfully.");

                    // Отобразить некоторые свойства QueryTable
                    Console.WriteLine("QueryTable Name: " + firstQueryTable.Name);
                }
                else
                {
                    Console.WriteLine("No QueryTables found in the worksheet.");
                }

                // Сохраните книгу
                workbook.Save("QueryTableItemDemo.xlsx");
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

* class [QueryTable](../../querytable/)
* class [QueryTableCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


