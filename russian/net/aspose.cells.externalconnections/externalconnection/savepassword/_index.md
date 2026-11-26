---
title: "ExternalConnection.SavePassword"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalConnection. True, если пароль должен сохраняться как часть строки подключения, иначе False"
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnection/savepassword/
---
## ExternalConnection.SavePassword property

True, если пароль должен сохраняться как часть строки соединения; иначе — False.

```csharp
public bool SavePassword { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySavePasswordDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            try
            {
                // Получить доступ к первому внешнему соединению (при условии, что оно существует)
                ExternalConnection connection = workbook.DataConnections[0];

                // Отобразить текущее значение SavePassword
                Console.WriteLine("Initial SavePassword value: " + connection.SavePassword);

                // Продемонстрировать установку свойства (поскольку оно доступно для чтения и записи).
                connection.SavePassword = !connection.SavePassword;
                Console.WriteLine("Updated SavePassword value: " + connection.SavePassword);

                // Переключить значение, чтобы продемонстрировать возможность установки
                connection.SavePassword = !connection.SavePassword;
                Console.WriteLine("Toggled SavePassword value: " + connection.SavePassword);

                // Сохранить книгу с изменёнными настройками соединения
                workbook.Save("SavePasswordDemo.xlsx");
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


