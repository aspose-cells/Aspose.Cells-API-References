---
title: "ExternalConnection.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalConnection. Especifica el nombre de la conexión. Cada conexión debe tener un nombre único"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/name/
---
## ExternalConnection.Name property

Especifica el nombre de la conexión. Cada conexión debe tener un nombre único.

```csharp
public string Name { get; set; }
```

### Ejemplos

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

### Ver también

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


