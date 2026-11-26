---
title: "ExternalConnection.ConnectionFile"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalConnection. Obtiene el archivo de conexión"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/connectionfile/
---
## ExternalConnection.ConnectionFile property

Obtiene el archivo de conexión.

```csharp
public virtual string ConnectionFile { get; }
```

### Ejemplos

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

### Ver también

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


