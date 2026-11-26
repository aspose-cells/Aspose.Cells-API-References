---
title: "DataModelRelationship.PrimaryKeyTable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataModelRelationship. Возвращает имя таблицы первичного ключа для этой связи"
type: docs
url: /ru/net/aspose.cells.datamodels/datamodelrelationship/primarykeytable/
---
## DataModelRelationship.PrimaryKeyTable property

Получает имя таблицы первичного ключа для этой связи.

```csharp
public string PrimaryKeyTable { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelRelationshipPropertyPrimaryKeyTableDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для создания осмысленного контекста
            worksheet.Cells["A1"].PutValue("Orders");
            worksheet.Cells["A2"].PutValue("OrderID");
            worksheet.Cells["A3"].PutValue("CustomerID");

            worksheet.Cells["C1"].PutValue("Customers");
            worksheet.Cells["C2"].PutValue("CustomerID");
            worksheet.Cells["C3"].PutValue("CustomerName");

            try
            {
                // Получить доступ к первой связи, если она существует
                DataModelRelationship relationship = workbook.DataModel?.Relationships?[0];

                if (relationship != null)
                {
                    // Отобразить значение свойства PrimaryKeyTable (только для чтения)
                    Console.WriteLine("Primary Key Table: " + relationship.PrimaryKeyTable);
                }
                else
                {
                    Console.WriteLine("No relationships found in the data model.");
                }

                // Сохраните книгу
                workbook.Save("PrimaryKeyTableDemo.xlsx");
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

* class [DataModelRelationship](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


