---
title: "ExternalConnection.SSOId"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalConnection. Идентификатор Single Sign On (SSO), используемый для аутентификации между промежуточным сервером spreadsheetML и внешним источником данных."
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnection/ssoid/
---
## ExternalConnection.SSOId property

Идентификатор для Single Sign On (SSO), используемый для аутентификации между промежуточным сервером spreadsheetML и внешним источником данных.

```csharp
public string SSOId { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySSOIdDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Получите первое внешнее соединение.
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Отобразите начальное значение SSOId (вероятно null для нового соединения).
                Console.WriteLine("Initial SSOId value: " + connection.SSOId);
                
                // Установите новое значение SSOId (поскольку оно доступно для чтения и записи).
                connection.SSOId = "sso-12345";
                Console.WriteLine("Updated SSOId value: " + connection.SSOId);
                
                // Очистите SSOId.
                connection.SSOId = null;
                Console.WriteLine("Cleared SSOId value: " + connection.SSOId);
                
                // Сохранить книгу с изменёнными настройками соединения
                workbook.Save("SSOIdDemo.xlsx");
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


