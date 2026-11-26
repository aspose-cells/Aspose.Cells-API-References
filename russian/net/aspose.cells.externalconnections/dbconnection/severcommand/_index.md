---
title: "DBConnection.SeverCommand"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DBConnection. Указывает вторую строку текста команды, которая сохраняется при использовании полей страниц PivotTable на основе сервера. Для ODBC‑соединений serverCommand обычно представляет более широкий запрос, чем command, в первом нет условия WHERE. На основе этих двух команд Command и ServerCommand пользовательский интерфейс параметров может быть заполнен, и могут быть построены параметризованные запросы."
type: docs
url: /ru/net/aspose.cells.externalconnections/dbconnection/severcommand/
---
## DBConnection.SeverCommand property

Указывает вторую строку команды, которая сохраняется, когда используются полевые элементы PivotTable на основе сервера. Для ODBC‑подключений serverCommand обычно представляет более широкий запрос, чем command (в первом нет предложения WHERE). На основе этих двух команд (Command и ServerCommand) можно заполнить пользовательский интерфейс параметров и построить параметризованные запросы.

```csharp
[Obsolete("Use ExternalConnection.SecondCommand property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string SeverCommand { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство ExternalConnection.SecondCommand. Этот метод будет удалён через 12 месяцев, начиная с октября 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class DBConnectionPropertySeverCommandDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook("input.xlsx");
            ExternalConnectionCollection connections = workbook.DataConnections;

            foreach (ExternalConnection connection in connections)
            {
                if (connection is DBConnection dbConn)
                {
                    dbConn.Name = dbConn.Name.Replace("c:\\", "d:\\");
                    dbConn.SourceFile = dbConn.SourceFile.Replace("c:\\", "d:\\");
                    dbConn.ConnectionInfo = dbConn.ConnectionInfo.Replace("c:\\", "d:\\").Replace("C:\\", "d:\\");
                    dbConn.Command = dbConn.Command.Replace("c:\\", "d:\\");
                    
                    if (!string.IsNullOrEmpty(dbConn.SeverCommand))
                        dbConn.SeverCommand = dbConn.SeverCommand.Replace("c:\\", "d:\\");
                }
            }

            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


