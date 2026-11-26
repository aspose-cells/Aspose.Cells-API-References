---
title: "WebQueryConnection.ClassType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebQueryConnection. Возвращает тип этого объекта ExternalConnection"
type: docs
url: /ru/net/aspose.cells.externalconnections/webqueryconnection/classtype/
---
## WebQueryConnection.ClassType property

Возвращает тип этого [`ExternalConnection`](../../externalconnection/) объекта.

```csharp
public override ExternalConnectionClassType ClassType { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyClassTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Получите существующее подключение веб‑запроса или создайте его через правильную инициализацию
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Отобразите значение ClassType (свойство только для чтения)
                    Console.WriteLine("WebQueryConnection ClassType: " + connection.ClassType);
                    
                    // Проверьте ожидаемое перечислимое значение для веб‑запроса
                    Console.WriteLine("Expected WebQuery enum value: " + 
                        (connection.ClassType == ExternalConnectionClassType.WebQuery ? "Match" : "Mismatch"));
                    
                    // Сохраните книгу
                    workbook.Save("WebQueryConnectionClassTypeDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connections found in the workbook.");
                }
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

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


