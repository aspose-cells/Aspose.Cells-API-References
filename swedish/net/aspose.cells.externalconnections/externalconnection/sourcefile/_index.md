---
title: "ExternalConnection.SourceFile"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection egenskap. Används när den externa datakällan är filbaserad. När en anslutning till en sådan datakälla misslyckas försöker kalkylprogrammet ansluta direkt till den här filen. Kan uttryckas som URI eller systemspecifik filsökvägsnotation"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/sourcefile/
---
## ExternalConnection.SourceFile property

Används när den externa datakällan är filbaserad. När en anslutning till en sådan datakälla misslyckas försöker kalkylbladsapplikationen ansluta direkt till den här filen. Kan uttryckas i URI‑ eller systemspecifik filsökvägsnotation.

```csharp
public string SourceFile { get; set; }
```

### Exempel

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

### Se även

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


