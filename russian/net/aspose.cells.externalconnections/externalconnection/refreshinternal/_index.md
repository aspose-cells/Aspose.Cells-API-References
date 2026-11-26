---
title: "ExternalConnection.RefreshInternal"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalConnection. Указывает количество минут между автоматическими обновлениями соединения"
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnection/refreshinternal/
---
## ExternalConnection.RefreshInternal property

Указывает количество минут между автоматическими обновлениями соединения.

```csharp
public int RefreshInternal { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyRefreshInternalDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные, чтобы пример имел смысл
            worksheet.Cells["A1"].Value = "Connection Demo";
            
            try
            {
                // Создайте соединение данных (используя базовый класс ExternalConnection)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Установите и отобразите свойство RefreshInternal
                connection.RefreshInternal = 30; // Refresh every 30 minutes
                Console.WriteLine("RefreshInternal value: " + connection.RefreshInternal);
                
                // Измените интервал обновления
                connection.RefreshInternal = 60;
                Console.WriteLine("Updated RefreshInternal value: " + connection.RefreshInternal);
                
                // Сохраните книгу с настройками соединения
                workbook.Save("RefreshInternalDemo.xlsx");
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


