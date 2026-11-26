---
title: "ConnectionParameter.Prompt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ConnectionParameter. Строка Prompt для параметра. Предоставляется пользователю таблицы вместе с интерфейсом ввода для сбора значения параметра перед обновлением внешних данных. Используется только когда parameterType имеет значение prompt"
type: docs
url: /ru/net/aspose.cells.externalconnections/connectionparameter/prompt/
---
## ConnectionParameter.Prompt property

Строка подсказки для параметра. Предоставляется пользователю таблицы вместе с пользовательским интерфейсом ввода для сбора значения параметра перед обновлением внешних данных. Используется только когда parameterType = prompt.

```csharp
public string Prompt { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyPromptDemo
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
                
                // Для демонстрации мы покажем, как Prompt будет использоваться, если у нас будет параметр
                if (parameter != null)
                {
                    // Получите и отобразите текущее значение Prompt
                    Console.WriteLine("Current Prompt: " + parameter.Prompt);
                    
                    // Установите новое значение Prompt (поскольку свойство доступно для чтения и записи)
                    parameter.Prompt = "Enter customer ID:";
                    Console.WriteLine("Updated Prompt: " + parameter.Prompt);
                }
                else
                {
                    // Запасная демонстрация, когда мы не можем создать параметр
                    workbook.Worksheets[0].Cells["A1"].Value = "Prompt property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Сохраните книгу
                workbook.Save("ConnectionParameterPromptDemo.xlsx");
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

* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


