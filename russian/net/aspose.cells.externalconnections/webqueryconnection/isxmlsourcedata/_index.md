---
title: "WebQueryConnection.IsXmlSourceData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebQueryConnection. Флаг, указывающий, что XML‑данные источника должны импортироваться вместо самой HTML‑таблицы"
type: docs
url: /ru/net/aspose.cells.externalconnections/webqueryconnection/isxmlsourcedata/
---
## WebQueryConnection.IsXmlSourceData property

Флаг, указывающий, что данные источника XML должны быть импортированы вместо самой HTML‑таблицы.

```csharp
public bool IsXmlSourceData { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXmlSourceDataDemo
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
                    // Отобразите начальное значение IsXmlSourceData
                    Console.WriteLine("Initial IsXmlSourceData value: " + connection.IsXmlSourceData);
                    
                    // Установите IsXmlSourceData в true
                    connection.IsXmlSourceData = true;
                    Console.WriteLine("Updated IsXmlSourceData value: " + connection.IsXmlSourceData);
                    
                    // Установите IsXmlSourceData обратно в false
                    connection.IsXmlSourceData = false;
                    Console.WriteLine("Final IsXmlSourceData value: " + connection.IsXmlSourceData);
                    
                    // Сохраните книгу
                    workbook.Save("WebQueryConnectionIsXmlSourceDataDemo.xlsx");
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


