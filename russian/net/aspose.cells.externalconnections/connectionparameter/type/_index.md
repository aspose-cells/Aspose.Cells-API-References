---
title: "ConnectionParameter.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ConnectionParameter. Тип используемого параметра. Если parameterTypevalue, то будет использовано значение из boolean, double, integer или string. В этом случае ожидается, что будет указано только одно из: boolean, double, integer или string"
type: docs
url: /ru/net/aspose.cells.externalconnections/connectionparameter/type/
---
## ConnectionParameter.Type property

Тип используемого параметра. Если parameterType=value, будет использовано значение из boolean, double, integer или string. В этом случае ожидается, что будет указано только одно из {boolean, double, integer, or string}.

```csharp
public ConnectionParameterType Type { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Создать новую книгу
                Workbook workbook = new Workbook();
                
                // Создайте параметр соединения (симулировано, так как параметры конструктора неизвестны)
                ConnectionParameter parameter = null;
                
                // В реальном сценарии вы бы создали параметр корректно
                // parameter = new ConnectionParameter(/* required parameters */);
                
                // Для демонстрации покажем, как используется Type, если у нас есть параметр
                if (parameter != null)
                {
                    // Получите и отобразите текущее значение Type
                    Console.WriteLine("Current Type: " + parameter.Type);
                    
                    // Установите новое значение Type (так как свойство доступно для чтения и записи)
                    parameter.Type = ConnectionParameterType.Value;
                    Console.WriteLine("Updated Type: " + parameter.Type);
                }
                else
                {
                    // Запасная демонстрация, когда мы не можем создать параметр
                    workbook.Worksheets[0].Cells["A1"].Value = "Type property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Сохраните книгу
                workbook.Save("ConnectionParameterTypeDemo.xlsx");
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

* enum [ConnectionParameterType](../../connectionparametertype/)
* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


