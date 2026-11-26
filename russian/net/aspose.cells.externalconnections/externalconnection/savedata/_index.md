---
title: "ExternalConnection.SaveData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalConnection. Истина, если внешние данные, полученные через соединение для заполнения таблицы, должны быть сохранены в книге, иначе ложь"
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnection/savedata/
---
## ExternalConnection.SaveData property

True, если внешние данные, полученные через соединение для заполнения таблицы, должны сохраняться вместе с книгой; иначе — false.

```csharp
public bool SaveData { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySaveDataDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Получить доступ к первому внешнему соединению (при условии, что оно существует)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Отобразить текущее значение SaveData
                Console.WriteLine("Initial SaveData value: " + connection.SaveData);
                
                // Продемонстрировать установку свойства (поскольку оно доступно для чтения и записи).
                connection.SaveData = !connection.SaveData;
                Console.WriteLine("Updated SaveData value: " + connection.SaveData);
                
                // Сохранить книгу с изменёнными настройками соединения
                workbook.Save("SaveDataDemo.xlsx");
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


