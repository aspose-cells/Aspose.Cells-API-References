---
title: "ExternalConnection.RefreshOnLoad"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalConnection. Истина, если это соединение должно быть обновлено при открытии файла, иначе ложь"
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnection/refreshonload/
---
## ExternalConnection.RefreshOnLoad property

True, если это соединение должно обновляться при открытии файла; иначе — false.

```csharp
public bool RefreshOnLoad { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyRefreshOnLoadDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Получите доступ к первому внешнему соединению (книга поставляется с соединениями по умолчанию)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Отобразить начальное значение RefreshOnLoad
                Console.WriteLine("Initial RefreshOnLoad value: " + connection.RefreshOnLoad);
                
                // Продемонстрировать установку свойства (поскольку оно доступно для чтения и записи).
                connection.RefreshOnLoad = !connection.RefreshOnLoad;
                Console.WriteLine("Updated RefreshOnLoad value: " + connection.RefreshOnLoad);
                
                // Сохранить книгу с изменёнными настройками соединения
                workbook.Save("RefreshOnLoadDemo.xlsx");
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


