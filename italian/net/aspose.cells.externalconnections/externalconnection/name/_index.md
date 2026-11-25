---
title: "ExternalConnection.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. Specifica il nome della connessione. Ogni connessione deve avere un nome univoco"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/name/
---
## ExternalConnection.Name property

Specifica il nome della connessione. Ogni connessione deve avere un nome univoco.

```csharp
public string Name { get; set; }
```

### Esempi

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

### Vedi anche

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


