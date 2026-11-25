---
title: "ExternalConnection.ConnectionFile"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. Ottiene il file di connessione"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/connectionfile/
---
## ExternalConnection.ConnectionFile property

Ottiene il file di connessione.

```csharp
public virtual string ConnectionFile { get; }
```

### Esempi

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

### Vedi anche

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


