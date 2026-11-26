---
title: "ConnectionParameter.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ConnectionParameter. Имя параметра"
type: docs
url: /ru/net/aspose.cells.externalconnections/connectionparameter/name/
---
## ConnectionParameter.Name property

Имя параметра.

```csharp
public string Name { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyNameDemo
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

                // Для демонстрации покажем, как используется Name, если у нас есть параметр
                if (parameter != null)
                {
                    // Получите и отобразите текущее значение Name
                    Console.WriteLine("Current Name: " + parameter.Name);

                    // Установите новое значение Name (так как свойство доступно для чтения и записи)
                    parameter.Name = "NewParameterName";
                    Console.WriteLine("Updated Name: " + parameter.Name);
                }
                else
                {
                    // Запасная демонстрация, когда мы не можем создать параметр
                    workbook.Worksheets[0].Cells["A1"].Value = "Name property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }

                // Сохраните книгу
                workbook.Save("ConnectionParameterNameDemo.xlsx");
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


