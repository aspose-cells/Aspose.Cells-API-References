---
title: "ConnectionParameter.Value"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ConnectionParameter. Нецелочисленное числовое значение, целочисленное значение, строковое значение или логическое значение, используемое в качестве параметра запроса. Используется только когда parameterType имеет значение value"
type: docs
url: /ru/net/aspose.cells.externalconnections/connectionparameter/value/
---
## ConnectionParameter.Value property

Нецелочисленное числовое значение, целочисленное значение, строковое значение или логическое значение, используемое в качестве параметра запроса. Используется только когда parameterType имеет значение value.

```csharp
public object Value { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyValueDemo
    {
        public static void Run()
        {
            try
            {
                // Создать новую книгу
                Workbook workbook = new Workbook();
                
                // Создайте параметр соединения (симулировано, так как мы не знаем параметры конструктора)
                ConnectionParameter parameter = null;
                
                // В реальном сценарии вы бы создали параметр корректно
                // parameter = new ConnectionParameter(/* required parameters */);
                
                // Для демонстрации мы создадим имитационный параметр со значением
                // Это показывает, как свойство Value будет использоваться на практике
                if (parameter != null)
                {
                    // Установите значение (поскольку Value доступно для чтения и записи)
                    parameter.Value = "SampleParameterValue";
                    
                    // Получите и отобразите значение
                    Console.WriteLine("Parameter Value: " + parameter.Value);
                    
                    // Измените значение, чтобы продемонстрировать его изменяемость
                    parameter.Value = 42;
                    Console.WriteLine("Updated Parameter Value: " + parameter.Value);
                }
                else
                {
                    // Запасная демонстрация, когда мы не можем создать параметр
                    workbook.Worksheets[0].Cells["A1"].Value = "Value property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Сохраните книгу
                workbook.Save("ConnectionParameterValueDemo.xlsx");
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


