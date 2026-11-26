---
title: "DataModel.Relationships"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataModel. Получает все связи таблиц в модели данных"
type: docs
url: /ru/net/aspose.cells.datamodels/datamodel/relationships/
---
## DataModel.Relationships property

Получает все связи таблиц в модели данных.

```csharp
public DataModelRelationshipCollection Relationships { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelPropertyRelationshipsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            try
            {
                // Получите доступ к DataModel из книги
                DataModel dataModel = workbook.DataModel;

                // Отобразите текущее значение свойства Relationships (только для чтения)
                Console.WriteLine("Number of relationships in DataModel: " + dataModel.Relationships.Count);

                // Итерируйте по связям, если они существуют
                foreach (DataModelRelationship relationship in dataModel.Relationships)
                {
                    Console.WriteLine("Relationship found: " + relationship);
                }

                // Сохраните книгу
                workbook.Save("RelationshipsDemo.xlsx");
                Console.WriteLine("Relationships demonstration completed successfully.");
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

* class [DataModelRelationshipCollection](../../datamodelrelationshipcollection/)
* class [DataModel](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


