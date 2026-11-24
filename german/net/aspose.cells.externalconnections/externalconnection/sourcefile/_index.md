---
title: "ExternalConnection.SourceFile"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalConnection-Eigenschaft. Wird verwendet, wenn die externe Datenquelle dateibasiert ist. Wenn eine Verbindung zu einer solchen Datenquelle fehlschlägt, versucht die Tabellenkalkulationsanwendung, direkt auf diese Datei zuzugreifen. Kann als URI oder in systemabhängiger Dateipfadnotation angegeben werden."
type: docs
url: /de/net/aspose.cells.externalconnections/externalconnection/sourcefile/
---
## ExternalConnection.SourceFile property

Wird verwendet, wenn die externe Datenquelle dateibasiert ist. Wenn eine Verbindung zu einer solchen Datenquelle fehlschlägt, versucht die Tabellenkalkulationsanwendung, direkt zu dieser Datei zu verbinden. Kann als URI oder systemabhängige Dateipfadnotation angegeben werden.

```csharp
public string SourceFile { get; set; }
```

### Beispiele

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

### Siehe auch

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


