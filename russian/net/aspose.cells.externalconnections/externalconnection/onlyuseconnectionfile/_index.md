---
title: "ExternalConnection.OnlyUseConnectionFile"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalConnection. Указывает, должна ли приложение электронных таблиц всегда и только использовать информацию о соединении из внешнего файла соединения, указанного атрибутом odcFile, при обновлении соединения. Если ложь, то приложение должно следовать процедуре, указанной атрибутом reconnectionMethod."
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/
---
## ExternalConnection.OnlyUseConnectionFile property

Указывает, должно ли приложение электронных таблиц всегда и исключительно использовать информацию о соединении из внешнего файла соединения, указанного атрибутом odcFile, при обновлении соединения. Если false, то приложение должно следовать процедуре, указанной атрибутом reconnectionMethod.

```csharp
public bool OnlyUseConnectionFile { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyOnlyUseConnectionFileDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Получить доступ к первому внешнему соединению (при условии, что оно существует)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Отобразить текущее значение OnlyUseConnectionFile
                Console.WriteLine("Initial OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
                
                // Установить новое значение OnlyUseConnectionFile (поскольку оно доступно для чтения и записи)
                connection.OnlyUseConnectionFile = true;
                Console.WriteLine("Updated OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
                
                // Переключить значение, чтобы продемонстрировать возможность установки
                connection.OnlyUseConnectionFile = !connection.OnlyUseConnectionFile;
                Console.WriteLine("Toggled OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
                
                // Сохранить книгу с изменёнными настройками соединения
                workbook.Save("OnlyUseConnectionFileDemo.xlsx");
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


