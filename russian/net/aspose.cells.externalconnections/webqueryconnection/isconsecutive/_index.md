---
title: "WebQueryConnection.IsConsecutive"
second_title: "Справочник API Aspose.Cells для .NET"
description: "WebQueryConnection property. Флаг, указывающий, следует ли рассматривать последовательные разделители как один разделитель"
type: docs
url: /ru/net/aspose.cells.externalconnections/webqueryconnection/isconsecutive/
---
## WebQueryConnection.IsConsecutive property

Флаг, указывающий, следует ли рассматривать последовательные разделители как один разделитель.

```csharp
public bool IsConsecutive { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsConsecutiveDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Создать соединение веб‑запроса, получив первое соединение
            // (при условии, что доступно хотя бы одно соединение)
            WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
            
            try
            {
                // Отобразить начальное значение IsConsecutive (по умолчанию)
                Console.WriteLine("Initial IsConsecutive value: " + connection.IsConsecutive);
                
                // Установить IsConsecutive в true
                connection.IsConsecutive = true;
                Console.WriteLine("Updated IsConsecutive value: " + connection.IsConsecutive);
                
                // Установить IsConsecutive обратно в false
                connection.IsConsecutive = false;
                Console.WriteLine("Final IsConsecutive value: " + connection.IsConsecutive);
                
                // Сохраните книгу с подключением веб‑запроса
                workbook.Save("WebQueryConnectionIsConsecutiveDemo.xlsx");
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


