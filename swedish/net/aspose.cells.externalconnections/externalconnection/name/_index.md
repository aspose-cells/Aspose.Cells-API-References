---
title: "ExternalConnection.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection-egenskap. Anger anslutningens namn. Varje anslutning måste ha ett unikt namn"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/name/
---
## ExternalConnection.Name property

Anger namnet på anslutningen. Varje anslutning måste ha ett unikt namn.

```csharp
public string Name { get; set; }
```

### Exempel

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

### Se även

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


