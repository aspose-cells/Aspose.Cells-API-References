---
title: "ExternalConnection.IsDeleted"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalConnection. Указывает, удалено ли связанное соединение книги. true, если соединение удалено, иначе false"
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnection/isdeleted/
---
## ExternalConnection.IsDeleted property

Указывает, было ли удалено связанное соединение книги. true, если соединение удалено; иначе false.

```csharp
public bool IsDeleted { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyIsDeletedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Получить доступ к первому внешнему соединению (при условии, что оно существует)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Отобразить начальное значение IsDeleted
                Console.WriteLine("Initial IsDeleted value: " + connection.IsDeleted);
                
                // Переключить значение IsDeleted (поскольку оно доступно для чтения и записи)
                connection.IsDeleted = !connection.IsDeleted;
                Console.WriteLine("Updated IsDeleted value: " + connection.IsDeleted);
                
                // Сохранить книгу с изменёнными настройками соединения
                workbook.Save("IsDeletedDemo.xlsx");
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


