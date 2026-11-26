---
title: "DBConnection.CommandType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DBConnection. Указывает тип команды OLE DB. 1. Запрос указывает имя куба 2. Запрос указывает SQL‑оператор 3. Запрос указывает имя таблицы 4. Запрос указывает, что предоставлена информация по умолчанию, и интерпретация зависит от провайдера 5. Запрос направлен к веб‑ориентированному поставщику List Data Provider"
type: docs
url: /ru/net/aspose.cells.externalconnections/dbconnection/commandtype/
---
## DBConnection.CommandType property

Указывает тип команды OLE DB. 1. Запрос указывает имя куба 2. Запрос указывает SQL‑оператор 3. Запрос указывает имя таблицы 4. Запрос указывает, что предоставлена информация по умолчанию, и интерпретация зависит от поставщика. 5. Запрос направлен к веб‑ориентированному List Data Provider.

```csharp
public override OLEDBCommandType CommandType { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;

    public class DBConnectionPropertyCommandTypeDemo
    {
        public static void Run()
        {
            // Инициализировать рабочую книгу (пустую или из файла, который может содержать соединения)
            Workbook workbook = new Workbook();

            try
            {
                // Получите доступ к коллекции внешних соединений
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Найдите первое DBConnection в коллекции (если есть)
                DBConnection dbConn = null;
                foreach (ExternalConnection conn in connections)
                {
                    if (conn is DBConnection dbConnection)
                    {
                        dbConn = dbConnection;
                        break;
                    }
                }

                if (dbConn == null)
                {
                    Console.WriteLine("No DBConnection objects found in the workbook.");
                }
                else
                {
                    // Отобразить текущее значение CommandType
                    Console.WriteLine("Original CommandType: " + dbConn.CommandType);

                    // Продемонстрировать установку CommandType (свойство чтения‑записи)
                    dbConn.CommandType = OLEDBCommandType.SqlStatement;
                    Console.WriteLine("Updated CommandType: " + dbConn.CommandType);
                }

                // Сохранить рабочую книгу (даже если она не изменена), чтобы проиллюстрировать полный процесс
                workbook.Save("CommandTypeDemo.xlsx");
                Console.WriteLine("Workbook saved as CommandTypeDemo.xlsx");
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

* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


