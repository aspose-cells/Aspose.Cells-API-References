---
title: "ExternalConnection.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalConnection. Spécifie le nom de la connexion. Chaque connexion doit avoir un nom unique"
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnection/name/
---
## ExternalConnection.Name property

Spécifie le nom de la connexion. Chaque connexion doit avoir un nom unique.

```csharp
public string Name { get; set; }
```

### Exemples

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

### Voir aussi

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


