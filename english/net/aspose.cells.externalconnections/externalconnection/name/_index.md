---
title: ExternalConnection.Name
second_title: Aspose.Cells for .NET API Reference
description: ExternalConnection property. Specifies the name of the connection. Each connection must have a unique name
type: docs
url: /net/aspose.cells.externalconnections/externalconnection/name/
---
## ExternalConnection.Name property

Specifies the name of the connection. Each connection must have a unique name.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine("connection: " + externalConnection.Name);
public void ExternalConnection_Property_Name()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsm");

    for (int i = 0; i < workbook.DataConnections.Count; i++)
    {
        Aspose.Cells.ExternalConnections.ExternalConnection externalConnection = workbook.DataConnections[i];
        Console.WriteLine("connection: " + externalConnection.Name);
        PrintTables(workbook, externalConnection);
        Console.WriteLine();
    }
    workbook.Save(Constants.destPath + "example.xlsm");
}
```

### See Also

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


