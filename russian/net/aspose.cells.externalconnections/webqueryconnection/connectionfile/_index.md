---
title: "WebQueryConnection.ConnectionFile"
second_title: "Справочник API Aspose.Cells для .NET"
description: "WebQueryConnection property. Возвращает файл соединения"
type: docs
url: /ru/net/aspose.cells.externalconnections/webqueryconnection/connectionfile/
---
## WebQueryConnection.ConnectionFile property

Получает файл соединения.

```csharp
public override string ConnectionFile { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyConnectionFileDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Создать пример листа с данными веб‑запроса
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Sample Web Query Data";
                
                // Получить первое существующее соединение веб‑запроса (если есть)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Отобразить значение ConnectionFile (свойство только для чтения)
                    Console.WriteLine("ConnectionFile value: " + connection.ConnectionFile);
                    
                    // Сохраните книгу
                    workbook.Save("WebQueryConnectionFileDemo.xlsx");
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

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


