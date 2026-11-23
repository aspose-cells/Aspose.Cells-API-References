---
title: "ExternalConnection.ConnectionFile"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalConnection. Obtient le fichier de connexion"
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnection/connectionfile/
---
## ExternalConnection.ConnectionFile property

Obtient le fichier de connexion.

```csharp
public virtual string ConnectionFile { get; }
```

### Exemples

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

### Voir aussi

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


