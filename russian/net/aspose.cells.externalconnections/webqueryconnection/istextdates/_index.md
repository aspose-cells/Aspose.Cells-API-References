---
title: "WebQueryConnection.IsTextDates"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebQueryConnection. Флаг, указывающий, следует ли импортировать даты в ячейки листа в виде текста, а не как даты"
type: docs
url: /ru/net/aspose.cells.externalconnections/webqueryconnection/istextdates/
---
## WebQueryConnection.IsTextDates property

Флаг, указывающий, следует ли импортировать даты в ячейки листа как текст, а не как даты.

```csharp
public bool IsTextDates { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsTextDatesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Получить доступ к первому листу
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Создайте соединение веб‑запроса, загрузив его из существующего файла
                // или получив доступ к существующему соединению
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Отобразите начальное значение IsTextDates
                    Console.WriteLine("Initial IsTextDates value: " + connection.IsTextDates);
                    
                    // Установите IsTextDates в true
                    connection.IsTextDates = true;
                    Console.WriteLine("Updated IsTextDates value: " + connection.IsTextDates);
                    
                    // Установите IsTextDates обратно в false
                    connection.IsTextDates = false;
                    Console.WriteLine("Final IsTextDates value: " + connection.IsTextDates);
                    
                    // Сохраните книгу с подключением веб‑запроса
                    workbook.Save("WebQueryConnectionIsTextDatesDemo.xlsx");
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


