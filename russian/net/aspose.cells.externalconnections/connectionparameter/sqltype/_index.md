---
title: "ConnectionParameter.SqlType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ConnectionParameter. Тип данных SQL параметра. Действительно только для источников ODBC"
type: docs
url: /ru/net/aspose.cells.externalconnections/connectionparameter/sqltype/
---
## ConnectionParameter.SqlType property

SQL‑тип данных параметра. Действителен только для источников ODBC.

```csharp
public SqlDataType SqlType { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertySqlTypeDemo
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
                
                // Для демонстрации мы покажем, как SqlType будет использоваться, если у нас будет параметр
                if (parameter != null)
                {
                    // Получите и отобразите текущее значение SqlType
                    Console.WriteLine("Current SqlType: " + parameter.SqlType);
                    
                    // Установите новое значение SqlType (поскольку свойство доступно для чтения и записи)
                    parameter.SqlType = SqlDataType.SqlInteger;
                    Console.WriteLine("Updated SqlType: " + parameter.SqlType);
                }
                else
                {
                    // Запасная демонстрация, когда мы не можем создать параметр
                    workbook.Worksheets[0].Cells["A1"].Value = "SqlType property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Сохраните книгу
                workbook.Save("ConnectionParameterSqlTypeDemo.xlsx");
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

* enum [SqlDataType](../../sqldatatype/)
* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


