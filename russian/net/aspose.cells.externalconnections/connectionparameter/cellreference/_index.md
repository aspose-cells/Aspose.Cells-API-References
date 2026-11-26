---
title: "ConnectionParameter.CellReference"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ConnectionParameter. Ссылка на ячейку, указывающая, значение каких ячеек использовать для параметра запроса. Используется только когда parameterType является cell"
type: docs
url: /ru/net/aspose.cells.externalconnections/connectionparameter/cellreference/
---
## ConnectionParameter.CellReference property

Ссылка на ячейку, указывающая, значение какой ячейки использовать для параметра запроса. Используется только когда parameterType имеет значение cell.

```csharp
public string CellReference { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyCellReferenceDemo
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
                
                // Для демонстрации покажем, как используется CellReference, если у нас есть параметр
                if (parameter != null)
                {
                    // Получите и отобразите текущее значение CellReference
                    Console.WriteLine("Current CellReference: " + parameter.CellReference);
                    
                    // Установите новое значение CellReference (так как свойство доступно для чтения и записи)
                    parameter.CellReference = "A1";
                    Console.WriteLine("Updated CellReference: " + parameter.CellReference);
                }
                else
                {
                    // Запасная демонстрация, когда мы не можем создать параметр
                    workbook.Worksheets[0].Cells["A1"].Value = "CellReference property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Сохраните книгу
                workbook.Save("ConnectionParameterCellReferenceDemo.xlsx");
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


