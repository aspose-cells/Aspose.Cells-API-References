---
title: "Класс DataModelRelationship"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.DataModels.DataModelRelationship. Представляет одну связь в модели данных электронной таблицы"
type: docs
url: /ru/net/aspose.cells.datamodels/datamodelrelationship/
---
## DataModelRelationship class

Представляет отдельную связь в модели данных электронной таблицы.

```csharp
public class DataModelRelationship
```

## Свойства

| Имя | Описание |
| --- | --- |
| [ForeignKeyColumn](../../aspose.cells.datamodels/datamodelrelationship/foreignkeycolumn/) { get; } | Получает имя столбца внешнего ключа таблицы для этой связи. |
| [ForeignKeyTable](../../aspose.cells.datamodels/datamodelrelationship/foreignkeytable/) { get; } | Получает имя таблицы внешнего ключа для этой связи. |
| [PrimaryKeyColumn](../../aspose.cells.datamodels/datamodelrelationship/primarykeycolumn/) { get; } | Получает имя столбца первичного ключа таблицы для этой связи. |
| [PrimaryKeyTable](../../aspose.cells.datamodels/datamodelrelationship/primarykeytable/) { get; } | Получает имя таблицы первичного ключа для этой связи. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelsClassDataModelRelationshipDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать примерные данные для демонстрации
            worksheet.Cells["A1"].PutValue("Orders");
            worksheet.Cells["A2"].PutValue("OrderID");
            worksheet.Cells["A3"].PutValue("CustomerID");
            worksheet.Cells["A4"].PutValue("OrderDate");
            
            worksheet.Cells["C1"].PutValue("Customers");
            worksheet.Cells["C2"].PutValue("CustomerID");
            worksheet.Cells["C3"].PutValue("CustomerName");
            worksheet.Cells["C4"].PutValue("ContactName");

            // Это демонстрирует доступ к свойствам существующей связи
            // В реальном сценарии вы бы получили это из DataModel
            DataModelRelationship relationship = workbook.DataModel?.Relationships?[0];
            if (relationship != null)
            {
                // Отобразить свойства отношений (только для чтения)
                Console.WriteLine("Sample Data Model Relationship Properties:");
                Console.WriteLine("Primary Key Table: " + relationship.PrimaryKeyTable);
                Console.WriteLine("Primary Key Column: " + relationship.PrimaryKeyColumn);
                Console.WriteLine("Foreign Key Table: " + relationship.ForeignKeyTable);
                Console.WriteLine("Foreign Key Column: " + relationship.ForeignKeyColumn);
            }
            else
            {
                Console.WriteLine("No data model relationships found");
            }

            // Сохраните книгу
            workbook.Save("DataModelRelationshipDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


