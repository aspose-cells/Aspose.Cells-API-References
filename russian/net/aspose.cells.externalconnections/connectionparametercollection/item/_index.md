---
title: "ConnectionParameterCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ConnectionParameterCollection. Получает элемент ConnectionParameter по указанному индексу"
type: docs
url: /ru/net/aspose.cells.externalconnections/connectionparametercollection/item/
---
## ConnectionParameterCollection indexer (1 of 2)

Получает элемент [`ConnectionParameter`](../../connectionparameter/) по указанному индексу.

```csharp
public ConnectionParameter this[int index] { get; }
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

    public class ConnectionParameterCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Получить первое внешнее соединение
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Получить коллекцию параметров
                ConnectionParameterCollection parameters = connection.Parameters;
                
                // Проверьте, есть ли параметры перед доступом
                if (parameters.Count > 0)
                {
                    // Продемонстрировать чтение свойства Item
                    ConnectionParameter firstParam = parameters[0];
                    Console.WriteLine($"Parameter type: {firstParam.GetType().Name}");
                }
                else
                {
                    Console.WriteLine("No parameters in collection");
                }
                
                // Сохраните книгу
                workbook.Save("ConnectionParameterItemDemo.xlsx");
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

* class [ConnectionParameter](../../connectionparameter/)
* class [ConnectionParameterCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)

---

## ConnectionParameterCollection indexer (2 of 2)

Получает элемент [`ConnectionParameter`](../../connectionparameter/) с указанным именем.

```csharp
public ConnectionParameter this[string connParamName] { get; }
```

| Параметр | Описание |
| --- | --- |
| connParamName | имя параметра соединения |

### Возвращаемое значение

Элемент с указанным именем.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Получить первое внешнее соединение
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Получить коллекцию параметров
                ConnectionParameterCollection parameters = connection.Parameters;
                
                // Проверьте, существуют ли параметры для демонстрации свойства Item
                if (parameters.Count == 0)
                {
                    Console.WriteLine("No parameters in collection to demonstrate Item property");
                    return;
                }
                
                // Получить имя первого параметра для демонстрации
                string firstParamName = parameters[0].Name;
                
                // Продемонстрировать чтение свойства Item по имени
                ConnectionParameter retrievedParam = parameters[firstParamName];
                
                if (retrievedParam != null)
                {
                    Console.WriteLine($"Retrieved parameter name: {retrievedParam.Name}");
                }
                else
                {
                    Console.WriteLine("Parameter not found");
                }
                
                // Сохраните книгу
                workbook.Save("ConnectionParameterItemDemo.xlsx");
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

* class [ConnectionParameter](../../connectionparameter/)
* class [ConnectionParameterCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


