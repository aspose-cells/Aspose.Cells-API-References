---
title: "ExternalConnection.SourceFile"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. Utilizzata quando la fonte dati esterna è basata su file. Quando una connessione a tale fonte dati fallisce, l'applicazione di foglio di calcolo tenta di connettersi direttamente a questo file. Può essere espressa in formato URI o notazione di percorso file specifica del sistema"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/sourcefile/
---
## ExternalConnection.SourceFile property

Utilizzato quando la fonte di dati esterna è basata su file. Quando una connessione a tale fonte di dati fallisce, l'applicazione di foglio di calcolo tenta di connettersi direttamente a questo file. Può essere espresso in formato URI o notazione di percorso file specifica del sistema.

```csharp
public string SourceFile { get; set; }
```

### Esempi

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

### Vedi anche

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


