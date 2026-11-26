---
title: "ExternalConnection.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalConnection. Получает или задает тип внешнего источника данных DataSource."
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnection/type/
---
## ExternalConnection.Type property

Получает или задаёт тип внешнего соединения DataSource.

```csharp
[Obsolete("Use ExternalConnection.SourceType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ConnectionDataSourceType Type { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство ExternalConnection.SourceType. Это свойство будет удалено через 12 месяцев, начиная с октября 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Получить доступ к первому внешнему соединению (при условии, что оно существует)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Отобразить текущее значение Type (операция чтения)
                Console.WriteLine("Initial Type value: " + connection.Type);
                
                // Установить новое значение Type (поскольку оно доступно для чтения и записи)
                connection.Type = ConnectionDataSourceType.OLEDBBasedSource;
                Console.WriteLine("Updated Type value: " + connection.Type);
                
                // Перебрать возможные значения, чтобы продемонстрировать возможность установки
                foreach (ConnectionDataSourceType type in Enum.GetValues(typeof(ConnectionDataSourceType)))
                {
                    if ((int)type != 102) // Skip duplicate enum value
                    {
                        connection.Type = type;
                        Console.WriteLine($"Type set to: {type}");
                    }
                }
                
                // Сохранить книгу с изменёнными настройками соединения
                workbook.Save("TypeDemo.xlsx");
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

* enum [ConnectionDataSourceType](../../connectiondatasourcetype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


