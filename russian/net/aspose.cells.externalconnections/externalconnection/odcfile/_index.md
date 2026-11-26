---
title: "ExternalConnection.OdcFile"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalConnection. Указывает полный путь к файлу внешнего соединения, из которого было создано это соединение. Если соединение не удаётся во время попытки обновить данные и reconnectionMethod1, то приложение таблицы попробует снова, используя информацию из файла внешнего соединения вместо объекта соединения, встроенного в книгу."
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnection/odcfile/
---
## ExternalConnection.OdcFile property

Указывает полный путь к файлу внешнего соединения, из которого было создано данное соединение. Если соединение не удаётся во время попытки обновления данных, и reconnectionMethod=1, то приложение электронных таблиц попробует снова, используя информацию из файла внешнего соединения вместо объекта соединения, встроенного в книгу.

```csharp
public string OdcFile { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyOdcFileDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Получить доступ к первому внешнему соединению (при условии, что оно существует)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Отобразить текущее значение OdcFile
                Console.WriteLine("Initial OdcFile value: " + connection.OdcFile);
                
                // Установить новое значение OdcFile (поскольку оно доступно для чтения и записи)
                connection.OdcFile = @"C:\Connections\ExternalData.odc";
                Console.WriteLine("Updated OdcFile value: " + connection.OdcFile);
                
                // Очистить значение OdcFile
                connection.OdcFile = string.Empty;
                Console.WriteLine("Cleared OdcFile value: " + connection.OdcFile);
                
                // Сохранить книгу с изменёнными настройками соединения
                workbook.Save("OdcFileDemo.xlsx");
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


