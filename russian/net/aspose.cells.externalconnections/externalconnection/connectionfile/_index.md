---
title: "ExternalConnection.ConnectionFile"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalConnection. Получает файл соединения"
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnection/connectionfile/
---
## ExternalConnection.ConnectionFile property

Получает файл соединения.

```csharp
public virtual string ConnectionFile { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyConnectionFileDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook("example.xlsx");
            ExternalConnection conn = workbook.Worksheets[0].PivotTables[0].GetSourceDataConnections()[0];
            
            Console.WriteLine("ConnectionFile: " + conn.ConnectionFile);
            
            workbook.Save("output.xlsx");
            
            Workbook reloadedWorkbook = new Workbook("output.xlsx");
            ExternalConnection reloadedConn = reloadedWorkbook.Worksheets[0].PivotTables[0].GetSourceDataConnections()[0];
            Console.WriteLine("ConnectionFile after reload: " + reloadedConn.ConnectionFile);
        }
    }
}
```

### См. также

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


