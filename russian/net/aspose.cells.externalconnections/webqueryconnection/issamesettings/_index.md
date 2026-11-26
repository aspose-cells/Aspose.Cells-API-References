---
title: "WebQueryConnection.IsSameSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebQueryConnection. Флаг, указывающий, следует ли разбирать все таблицы внутри блока PRE с теми же настройками ширины, что и первая строка"
type: docs
url: /ru/net/aspose.cells.externalconnections/webqueryconnection/issamesettings/
---
## WebQueryConnection.IsSameSettings property

Флаг, указывающий, следует ли разбирать все таблицы внутри блока PRE с теми же настройками ширины, что и первая строка.

```csharp
public bool IsSameSettings { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsSameSettingsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Получить первое существующее соединение веб‑запроса, если оно доступно
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Отобразить начальное значение IsSameSettings
                    Console.WriteLine("Initial IsSameSettings value: " + connection.IsSameSettings);
                    
                    // Установить IsSameSettings в true (поскольку он доступен для чтения и записи)
                    connection.IsSameSettings = true;
                    Console.WriteLine("Updated IsSameSettings value: " + connection.IsSameSettings);
                    
                    // Установить IsSameSettings обратно в false
                    connection.IsSameSettings = false;
                    Console.WriteLine("Final IsSameSettings value: " + connection.IsSameSettings);
                    
                    // Сохраните книгу
                    workbook.Save("WebQueryConnectionIsSameSettingsDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connection found in the workbook.");
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


