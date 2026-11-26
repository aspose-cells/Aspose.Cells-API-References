---
title: "DataModelRelationshipCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataModelRelationshipCollection. Получает связь"
type: docs
url: /ru/net/aspose.cells.datamodels/datamodelrelationshipcollection/item/
---
## DataModelRelationshipCollection indexer

Получает отношение.

```csharp
public DataModelRelationship this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelRelationshipCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создайте новую книгу (пустая модель данных)
            Workbook workbook = new Workbook();

            try
            {
                // Получите DataModelRelationshipCollection из книги (может быть null, если нет модели данных)
                DataModelRelationshipCollection relationships = workbook.DataModel?.Relationships;

                if (relationships == null)
                {
                    Console.WriteLine("The workbook does not contain a data model.");
                }
                else if (relationships.Count == 0)
                {
                    Console.WriteLine("The data model exists but contains no relationships.");
                }
                else
                {
                    // Прочитайте первую связь, используя свойство Item (индексатор)
                    DataModelRelationship firstRelationship = relationships[0]; // Item property getter
                    Console.WriteLine("First relationship retrieved via Item property:");
                    Console.WriteLine(firstRelationship);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while accessing Item property: {ex.Message}");
            }

            // Сохраните книгу (необязательно, только чтобы продемонстрировать, что код работает от начала до конца)
            workbook.Save("ItemPropertyDemo.xlsx");
        }
    }
}
```

### См. также

* class [DataModelRelationship](../../datamodelrelationship/)
* class [DataModelRelationshipCollection](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


