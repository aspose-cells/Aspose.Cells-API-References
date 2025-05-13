---
title: DBConnection.PowerQueryFormula
second_title: Aspose.Cells for .NET API Reference
description: DBConnection property. Gets the definition of power query formula
type: docs
url: /net/aspose.cells.externalconnections/dbconnection/powerqueryformula/
---
## DBConnection.PowerQueryFormula property

Gets the definition of power query formula.

```csharp
public override PowerQueryFormula PowerQueryFormula { get; }
```

### Examples

```csharp
// Called: var powerQueryFormula = connection.PowerQueryFormula;
public void DBConnection_Property_PowerQueryFormula()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    var externalConnections = workbook.DataConnections;

    foreach (var externalConnection in externalConnections)
    {
        var connection = (DBConnection)externalConnection;
        var powerQueryFormula = connection.PowerQueryFormula;
    }
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [PowerQueryFormula](../../../aspose.cells.querytables/powerqueryformula/)
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


