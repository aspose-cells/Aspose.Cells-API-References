---
title: "ExternalConnection.SourceFile"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalConnection. Используется, когда внешний источник данных основан на файле. Когда соединение с таким источником данных не удаётся, приложение таблицы пытается подключиться напрямую к этому файлу. Может быть указано в виде URI или системно-специфической нотации пути к файлу."
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnection/sourcefile/
---
## ExternalConnection.SourceFile property

Используется, когда внешний источник данных основан на файле. Когда соединение с таким источником данных не удаётся, приложение таблиц пытается подключиться напрямую к этому файлу. Может быть указано в виде URI или системно‑специфической нотации пути к файлу.

```csharp
public string SourceFile { get; set; }
```

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertySourceFileDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook("input.xlsx");
            ExternalConnectionCollection connections = workbook.DataConnections;

            foreach (ExternalConnection connection in connections)
            {
                if (!string.IsNullOrEmpty(connection.SourceFile))
                    connection.SourceFile = connection.SourceFile.Replace("C:\\", "D:\\");
            }

            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


