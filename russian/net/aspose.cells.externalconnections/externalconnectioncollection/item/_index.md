---
title: "ExternalConnectionCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalConnectionCollection. Возвращает элемент ExternalConnection по указанному индексу"
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnectioncollection/item/
---
## ExternalConnectionCollection indexer (1 of 2)

Возвращает элемент [`ExternalConnection`](../../externalconnection/) по указанному индексу.

```csharp
public ExternalConnection this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс элемента, начиная с нуля. |

### Возвращаемое значение

Элемент по указанному индексу.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            try
            {
                // Получить доступ к коллекции внешних подключений
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Проверьте, есть ли какие-либо подключения
                if (connections.Count > 0)
                {
                    // Продемонстрировать доступ к элементу по индексу (операция чтения)
                    ExternalConnection connection = connections[0];

                    // Отобразите информацию о соединении
                    Console.WriteLine($"Connection Name: {connection.Name}");
                    Console.WriteLine($"Connection Type: {connection.Type}");
                    Console.WriteLine($"Connection ID: {connection.ConnectionId}");
                }
                else
                {
                    Console.WriteLine("No external connections available to demonstrate Item property");
                }

                // Сохраните книгу
                workbook.Save("ExternalConnectionItemDemo.xlsx");
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

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)

---

## ExternalConnectionCollection indexer (2 of 2)

Возвращает элемент [`ExternalConnection`](../../externalconnection/) с указанным именем.

```csharp
public ExternalConnection this[string connectionName] { get; }
```

| Параметр | Описание |
| --- | --- |
| connectionName | имя соединения данных |

### Возвращаемое значение

Элемент с указанным именем.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Получить доступ к коллекции внешних подключений
                ExternalConnectionCollection connections = workbook.DataConnections;
                
                // Добавьте пример подключения (если необходимо для демонстрации)
                // Это предполагает, что коллекция позволяет добавлять подключения
                // connections.Add(new ExternalConnection());
                
                // Продемонстрировать доступ к элементу по имени (операция чтения)
                // Примечание: В реальном сценарии вам понадобятся реальные имена подключений
                if (connections.Count > 0)
                {
                    // Получить первое имя подключения (если доступно)
                    string connectionName = connections[0].Name;
                    
                    // Получить доступ к свойству Item
                    ExternalConnection connection = connections[connectionName];
                    
                    // Отобразите информацию о соединении
                    Console.WriteLine($"Connection Name: {connection.Name}");
                    Console.WriteLine($"Connection Type: {connection.Type}");
                }
                else
                {
                    Console.WriteLine("No external connections available to demonstrate Item property");
                }
                
                // Сохраните книгу
                workbook.Save("ExternalConnectionDemo.xlsx");
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

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


