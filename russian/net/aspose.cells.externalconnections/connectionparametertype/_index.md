---
title: "Enum ConnectionParameterType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.ExternalConnections.ConnectionParameterType. Указывает тип параметра внешнего соединения"
type: docs
url: /ru/net/aspose.cells.externalconnections/connectionparametertype/
---
## ConnectionParameterType enumeration

Указывает тип параметра внешнего соединения

```csharp
public enum ConnectionParameterType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Cell | `0` | Получайте значение параметра из ячейки при каждом обновлении. |
| Prompt | `1` | Запрашивайте у пользователя значение параметра при каждом обновлении. |
| Value | `2` | Используйте постоянное значение для параметра при каждом обновлении. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassConnectionParameterTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Продемонстрировать создание и использование значений перечисления ConnectionParameterType
                ConnectionParameterType cellParam = ConnectionParameterType.Cell;
                ConnectionParameterType promptParam = ConnectionParameterType.Prompt;
                ConnectionParameterType valueParam = ConnectionParameterType.Value;

                // Отобразить значения перечисления
                Console.WriteLine("Connection Parameter Types:");
                Console.WriteLine($"Cell: {cellParam}");
                Console.WriteLine($"Prompt: {promptParam}");
                Console.WriteLine($"Value: {valueParam}");

                // Продемонстрировать использование в операторе switch
                ConnectionParameterType testParam = ConnectionParameterType.Prompt;
                switch (testParam)
                {
                    case ConnectionParameterType.Cell:
                        Console.WriteLine("Parameter will get value from a cell");
                        break;
                    case ConnectionParameterType.Prompt:
                        Console.WriteLine("Parameter will prompt user for value");
                        break;
                    case ConnectionParameterType.Value:
                        Console.WriteLine("Parameter will use constant value");
                        break;
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating ConnectionParameterType: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


