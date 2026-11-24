---
title: "ExternalConnection.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalConnection-Eigenschaft. Gibt den Namen der Verbindung an. Jede Verbindung muss einen eindeutigen Namen haben"
type: docs
url: /de/net/aspose.cells.externalconnections/externalconnection/name/
---
## ExternalConnection.Name property

Gibt den Namen der Verbindung an. Jede Verbindung muss einen eindeutigen Namen haben.

```csharp
public string Name { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook("example.xlsm");

            foreach (ExternalConnection connection in workbook.DataConnections)
            {
                Console.WriteLine("Connection Name: " + connection.Name);
            }

            workbook.Save("output.xlsm");
        }
    }
}
```

### Siehe auch

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


