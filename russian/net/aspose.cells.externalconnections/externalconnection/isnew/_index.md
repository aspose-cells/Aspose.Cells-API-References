---
title: "ExternalConnection.IsNew"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalConnection. Истина, если соединение ещё не было обновлено впервые, иначе ложь. Такое состояние может возникнуть, когда пользователь сохраняет файл до завершения выполнения запроса."
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnection/isnew/
---
## ExternalConnection.IsNew property

True, если соединение ещё не было обновлено впервые; иначе false. Такое состояние может возникнуть, когда пользователь сохраняет файл до завершения выполнения запроса.

```csharp
public bool IsNew { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyIsNewDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Получите первое внешнее соединение (ново‑созданные соединения обычно имеют статус "IsNew").
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Отобразите начальное значение IsNew.
                Console.WriteLine("Initial IsNew value: " + connection.IsNew);
                
                // Поскольку IsNew доступен для чтения и записи, продемонстрируйте его установку.
                connection.IsNew = false;
                Console.WriteLine("Updated IsNew value: " + connection.IsNew);
                
                // Сохранить книгу с изменёнными настройками соединения
                workbook.Save("IsNewDemo.xlsx");
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


